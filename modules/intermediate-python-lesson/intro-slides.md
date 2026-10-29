---
title: Introduction
type: slides
order: 1
author: Sander van Rijn
description: Introduction to the Intermediate Research Software Development in Python workshop
---

<!-- .slide: data-state="title" -->

# Intermediate Research Software Development in Python

note:

===

<!-- .slide: data-state="standard" -->

<style>

/* Blockquote main style */
.blockquote {
    position: relative;
    font-weight: 800;
    padding: 30px 0;
    width: 100%;
    max-width: 500px;
    z-index: 1;
    margin: 80px auto;
    align-self: center;
    border-top: solid 1px;
    border-bottom: solid 1px;
}

/* Blockquote header */
.blockquote h1 {
    position: relative;
    font-size: small;
    font-weight: 800;
    line-height: 1;
    margin: 0;
}

/* Blockquote right double quotes */
.blockquote:after {
    position: absolute;
    content: "”";
    font-size: 10rem;
    line-height: 0;
    bottom: -43px;
    right: 30px;
}

/* increase header size after 600px */
@media all and (min-width: 600px) {
    .blockquote h1 {
        font-size: 60px;
   }

}

/* Blockquote subheader */
.blockquote h4 {
    position: relative;
    font-size: 1.4rem;
    font-weight: normal;
    line-height: 1;
    margin: 0;
    padding-top: 20px;
    z-index: 1;
}

</style>

## Introduction

- What is this course about?
- Why should I consider how I engineer my projects?
- How is this course organised?

===

## Modern research is impossible without software

<img src='./media/image9.png'>

From thrown-together scripts, through an abundance of complex spreadsheets, to the millions of lines of code behind large-scale infrastructure, there are few areas where software does not play a fundamental part in research​

===

## The software you write is important!

<div style="width: 66%; float: left;">
<ul>
  <li>Software inherently contains <i>value</i>, not a throw-away artifact
  <br>
  <li>Difficult to gauge to what extent it might be used in the future
  <ul>
    <li>By who?
    <li>Which parts?
    <li>Which projects?
    <li>Reproducibility of results &mdash; from publications!
  </ul>
</ul>
</div>

<div style="width: 33%; float: right;">
  <img src='./media/image11.png'>
</div>

<div>
Can/should it be reusable by others? ...including yourself?
</div>

===

## When should you have considered how to engineer your software?

<div style="width: 66%; float: left;" class="blockquote-wrapper fragment">
  <div class="blockquote">
      The best time to plant a tree is 20 years ago. The second best time is now.
  </div>
</div>


<div style="width: 33%; float: right;">
  <img src='./media/image12.png'>
</div>


===

## Programming vs Software Engineering

<div style="width: 49%; float: left;">
  Programming / Coding
  <ul>
    <li>Focus is one aspect of software development (implementation)
    <li>Writes software for themselves
    <li>Mostly an individual activity
    <li>Writes software to fulfill research goals (ideally from a design)
  </ul>
</div>
<div style="width: 49%; float: right;">
  Engineering
  <ul>
    <li>Considers the <i>lifecycle</i> of software
    <li>Writes software for <i>stakeholders</i>
    <li>Takes <i>team ethic</i> into account
    <li>Applies a <i>process</i> to understanding, designing, building, releasing, and maintaining software
  </ul>
</div>

<div class="blockquote-wrapper fragment">
  <div class="blockquote">
      Programmers tend to start coding right away. Sometimes this works.
    <h4>&mdash; Eric Larsen, 2018</h4>
  </div>
</div>

Note:
What's the difference between programming and software engineering?

===

## Target Audience

A researcher developer, with foundational coding skills, now facing new challenges​

- Software projects becoming more complex​
- Scale of development increasing​
- More collaborative development and use, internal or external​
- Higher expectations on software​
- Increase in requests for change, more 'technical debt'​

<img width="800" src='./media/Slide17.jpg'>

===

## Course Outline

1. Environment for Collaborative Code Development
   - Setting up our software project, development environments and tools, virtual environments, Git & GitHub, coding conventions​
2. Ensuring Correctness of Software at Scale
   - Automatically testing your software, unit tests, continuous integration,​ debugging, improving code robustness​
3. Software Development as a Process
   - Software requirements, design, architecture and implementation (via programming paradigms) as typical stages of a software development process​
4. Collaborative Software Development for Reuse
   - Code review, documenting and preparing/packaging software for release and reuse​
5. Managing and Improving Software Over Its Lifetime
   - Tracking issues, managing team communications and software project planning and management

===

## How will the workshop run

Delivery is helper-supported self-learning (no live coding)​

- We will introduce each part with a short presentation
- Learners go through material individually (at their own pace)​
- You work together in groups of 4-5 people​
- Trainers will be available to assist with problems and answer questions​
- Initially exercises are performed individually, more group/team work in later stages when we will need to keep more in sync with everyone in a group​
- Feel free to ask questions and start discussions with people in your group or instructors. This is a good opportunity to ask related questions about your daily work as well.
- We will remind you to take regular breaks

===

## A final note ...

About working through the material

- Start from the actual section introduction - bigger picture​
- Exercises - try to do them on your own (before looking at the solution)​
- Exercises - don't skip them! Some later materials depend on this​
- Optional exercises are clearly marked - all other exercises should be completed​
- Please finish the section in the rest of the week if you were note finished. Note that section 1 is a bit bigger than the other sections.​
- We wrap up together at the end of the day. If you finish the section early you can work on the optional exercises in the collaborative document​
​
Please ask for help - do not suffer in silence!​

- Ask for help if needed ​
- We know from experience that some people don't like to read, especially not at the end of the day when you feel like everyone else is moving faster than you. Ask an instructor to explain instead of reading the texts!​

===

## The story ...

<div style="width: 66%; float: left;">
  You have just joined a team that works on an existing software project. The project is written in Python and studies and analyses inflammation in a group of patients that have been given a new treatment for arthritis in a medical trial. The software project is not finished and contains some bugs and tests that are failing. Over the course - you will work either individually or with your colleagues to develop more code and fix these errors.​
</div>
<div style="width: 33%; float: right;">
  <img src="./media/image13.jpg">
</div>