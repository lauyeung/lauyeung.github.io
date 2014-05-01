---
layout: post
title: "Notes from An Event Apart (Boston, April 2014)"
date: 2014-04-30 20:01
comments: true
categories: coding, ux, conference notes
---

<h2>Day 1</h2>
<h3>Understanding Web Design (Jeffrey Zeldman, Founder, Happy Cog and A List Apart)</h3>

- Anything that gets in the way of users doing what they want to do is bad web design
- Web design is more like type-face, architecture - it steps away and allows the user or content to produce the meaning
- Great websites makes interaction easy
- Guides you subtly toward your heart’s desire (looks passive, but it’s active)
- Can be invisible or in your face
- Great web design <em>delights</em>

<h3>Designing Using Data (Sarah Paramenter, Founder, You Know Who)</h3>

- Research and data helps back up decisions of why you are changing something (and in turn - helps to remove resistance to that change)
- Avoid vanity metrics (metrics that can’t be acted upon, e.g. hits, pageviews)
- Track users and their habits (identify, segment, track)
- Leverage Facebook to find out who interacts with your content (use ads and Facebook insights)
- Test phrasing ("See plans and pricing" performed better than "Free trial" for CTA because it was less commital)

Recommended Tools<br>
- [TrueSocialMetrics](http://www.truesocialmetrics.com/)<br>
- [Minimalytics](http://www.minimalytics.com/)<br>
- [Crazy Egg](http://www.crazyegg.com/)<br>
- [Optimizely](https://www.optimizely.com)<br>
- [BrowserStack](http://www.browserstack.com/)<br>


<h3>Responsive Design is Still Hard/Easy! Be Afraid/Don’t Worry! (Dan Mall, Founder & Design Director, SuperFriendly)</h3>

<strong>Inventory</strong>

- Content inventory: identify all pages on the site and what the page is supposed to do
- Pattern inventory: identify the atoms / molecules / organisms on the website (can do this in spreadsheet, photoshop, coded, etc, whatever’s fastest), check out [Pattern Lab](http://patternlab.io/about.html)

<strong>Sketch</strong>

- Lay everything out simply (use grey boxes)
- Number them & block them out on the page
- Easy to layout and make responsive
- Simple visualization allows for dialog about layout<br>
Check out [Sparkbox example](http://building.seesparkbox.com/content-prototype/index.php)

<strong>Assemble</strong>

- Create organisms
- Presets: list out all the <em>potential</em> organisms for each page
- Once organisms and presets are created/prepped (mise en place!), putting pages together should be easy
- Check out [Pattern Primer](http://patternprimer.adactio.com/)

<h3>Screen Time (Luke Wroblewski, CEO & Co-Founder of Input Factory Inc.)</h3>

- Know your screen (increasingly mobile)<br>
- Output (high resolution, widescreen aspect rations, media queries know more than width)<br>
- Input (support all inputs, communicate what’s possible, screen size is poor proxy but it’s all we’ve got)<br>
- Posture (design to human scale, environments, not to screen width, distance from device impacts interactions)<br>

Note: there is a need to optimize tablets for both horizontal and vertical orientations (because both orientations are used!)

<h3>Content/Communication (Kristina Halvorson, Author, Content Strategy for the Web)</h3>
- Principles: internally motivates us to do things that are good and right, unites us in our day-to-day work<br>
- Strategy: good strategy will provide constraints and keeps us accountable<br>
- Process: process should evolve (retrospectives to figure out what works and what doesn't), good process allows us to move together<br>
- Roles: roles give us a place, use the [RACI model](http://thebuildnetwork.com/leadership/management/raci-model/)<br>
- Perceptions: prevent crossed wires or communication issues, ask for clarification when needed, perceptions give way to perspective<br>

All this stuff is important because:<br>
"A study of over 350 people in 6 business units at a financial services company found that the greatest predictor of a team's achievement was how the members felt about one another."<br>
- Shawn Achor, The Happiness Advantage

<h3>UX Strategy Means Business (Jared Spool, Founder, User Interface Engineering)</h3>

Great content + Great design = Great UX

Business Strategy Priorities<br>
1. Increase revenue<br>
2. Decrease costs<br>
3. Increase new business<br>
4. Increase existing business<br>
5. Shareholder value<br>

The 5 strategic priorities are a tool for mapping our design intent into business objectives

Business Model Options<br>
- Metered paywalls<br>
- Repurposed content<br>
- Supporting product sales<br>
- In-app purchases<br>
- Alternate channel revenue<br>
- Content distribution<br>
- Advertising (ideally avoid this)<br>

Advertising: disruptive and corporate (doesn’t add value for the user)<br>
Experience: in the moment of what the user is doing

<h2>Day 2</h2>
<h3>The Long Web (Jeremy Keith, Maker of Websites)</h3>
<strong>Progressive Enhancement</strong>

- Start using html elements that are not universally supported and because of HTML error-handling, things will still work
- Not designing for the lowest common denominator but starting there (e.g. escalators are progressively enhanced stairs)
- Make sure you build a strong base
- JS doesn’t share the error-handling of HTML/CSS - what happens when JS doesn't load appropriately?
- Need to think long term and having a strong HTML base that is backwards compatible is the way to do it

<h3>Responsive Design Performance Budget (Paul Irish, Developer advocate, Google Chrome)</h3>

71% expect sites to load faster on their phone than on their laptop

Bandwidth: amount of information<br>
Latency: lag time
Latency on phones is high which is why it’s slow and the number of users with higher latency is going to increase (more people using mobile)

Aggressive, but good goals:<br>
1. Deliver a fast mobile web page load (show above-fold content in <1 second, serve above-fold content, including critical path CSS, in first 14KB of response)<br>
2. Speed index <1000<br>
3. Delight users<br>

Recommended Tools<br>
- [WebPageTest](http://www.webpagetest.org/)<br>
- [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/): can run URL through and provides recommendations<br>
- [PageSpeed Module](https://developers.google.com/speed/pagespeed/module): plugin for Apache or NGiNX <br>

<h3>The Chroma Zone: Engineering Color on the Web (Lea Verou, W3C CSS Working Group Invited Expert)</h3>
<ul>
  <li>Lightness is not a good deciding metric for whether you should put white or black text on top of color background - relative luminence instead?</li>
  <li>Variables in CSS coming (e.g. currentColor is currently available but limited)</li>
  <li>4-digit hex code (last for alpha)</li>
  <li>HWB = hue whiteness blackness</li>
</ul>

<h3>Mind the Gap: Designing in the Space Between Devices (Josh Clark, Principal, Global Moxie)</h3>
67% users start shopping on one device and continue on another and have to think about each device and also the gaps between

Sometimes don’t even need the internet to have device exchange:<br>
- WebSockets<br>
- WebRTC<br>
- Bluetooth LE<br>

Bridge the physical and the digital

Giving digital a physical presence and vice versa

Neat Examples<br>
- [Making devices happier together =)](https://github.com/houseoflegend/happytogether)<br>
- [Grab screen from tv and put it on the phone](https://github.com/aral/GrabMagic)<br>

<h3>Web+: Can the Web Win the War Against Native Without Losing its Soul? (Bruce Lawson, Developer Relations, Opera)</h3>
Reasons people prefer native vs. mobile web
- Device-specific functionality<br>
- Offline capability<br>
- Faster performance (local storage)<br>
- Familiar<br>
- Mobile users bookmark by downloading native app (vs. bookmarking in browser)<br>

10% of users bookmark a page (computer) and is less on mobile

For mobile users - installing IS bookmarking

On the web - the conversation can happen in real time (instant updates vs. downloading updates with a native app)

<h3>How to Champion Ideas Back at Work (Scott Berkun, Author, The Year Without Pants)</h3>
"The real designer is the person with the power to make decisions"<br><br>
1. Get idea<br>
2. Build it<br>
3. Ship it<br>

Between steps 1 & 2 - need to convince people to build and maybe between 2 & 3 - need to convince to ship (lots of convincing needs to happen)

Find ways to bring ideas while mitigating risk
