---
layout: post
title: "Using ternary operators to store sessions in Rails"
date: 2013-09-24 12:09
comments: true
categories: coding, ruby, ruby on rails
---
Recently at [Launch Academy](http://www.launchacademy.com/), we learnt about sessions and cookies as a means to store data between requests. Using the ```session``` hash in Rails means we can persist data.

In our example, we stored a registration id to the ```session``` hash in the create controller action so that we could access it in subsequent visits to the new page. Since there isn't always necessarily a ```session``` available, we needed to make sure we wouldn't encouter exceptions when looking for the last ```session```.

Here are a 3 methods I tried:
```ruby
# GET /registrations/new

# Method 1
def new
  # Use find_by_id to try and locate a Registration with the last registration id
  # Using find_by_id instead of find since find_by_id returns nil when not found
  # (find throws an exception)
  @last_registration = Registration.find_by_id(session[:last_registration_id])
  @registration = Registration.new

  # Sets the registration email as the last registration email if it exists
  # (prepopulating the form would happen in the view)
  if @last_registration.present?
    @registration.email = @last_registration.email
  end
end

# Method 2
def new
  # Looks for last registration the same way as method 1
  @last_registration = Registration.find_by_id(session[:last_registration_id])
  @registration = Registration.new

  # Instead of using an if statement, use .try to pull the last registration email address
  # (results in nil instead of throwing an error if last registration email doesn't exist)
  @registration.email = @last_registration.try(:email)
end

# Method 3
def new
  # Here comes the ternary operator (condition ? if_true : if_false)
  # Use ternary operator to check if there is a session last registration id and
  # if there is, the last registration email is set to that
  # If there is no last registration id, last registration email is set to a blank string
  @last_registration_email = session[:last_registration_id] ? Registration.find_by_id(session[:last_registration_id]).email : ''
  @registration = Registration.new
end
```

The last method is definitely the most concise--and I think pretty expressive too.
