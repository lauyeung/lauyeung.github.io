---
layout: post
title: "Beginner Vim Commands"
date: 2013-10-14 15:08
comments: true
categories: coding, vim, vim commands, vim cheatsheet
---

I'm new to [Vim](http://www.vim.org/) but I've been using [Sublime Text](http://www.sublimetext.com/) in vintage mode to practice. I've tried a few tutorials but I've found it more helpful to actually learn by using the commands while coding.

I wanted to share my starter set of commands and I hope I remember to add blog posts as I add to my repetoire.

<table>
  <th><strong>Shortcut</strong></th>
  <tr>
    <td>gg</td>
    <td>go to the top</td>
  </tr>
  <tr>
    <td>G</td>
    <td>go to the bottom</td>
  </tr>
  <tr>
    <td>i</td>
    <td>insert (puts cursor before marker location</td>
  </tr>
  <tr>
    <td>a</td>
    <td>append (puts cursor after marker location</td>
  </tr>
  <tr>
    <td>x</td>
    <td>deletes character above the cursor</td>
  </tr>
  <tr>
    <td>X</td>
    <td>deletes character before the cursor</td>
  </tr>
  <tr>
    <td>D</td>
    <td>delete from cursor to end of the line</td>
  </tr>
  <tr>
    <td>dd</td>
    <td>deletes a row</td>
  </tr>
  <tr>
    <td>diw</td>
    <td>deletes a word</td>
  </tr>
  <tr>
    <td>ciw</td>
    <td>deletes a word and goes to insert mode</td>
  </tr>
</table><br>

<strong>How to cut/copy and paste:</strong><br>
1. v (or V for whole lines) to highlight what you want to cut or copy<br>
2. d (for cut), y (for copy)<br>
3. p to paste after cursor (P for before the cursor)<br>
