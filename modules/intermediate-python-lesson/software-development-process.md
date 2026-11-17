---
title: Software Development Process
type: slides
order: 4
author: Sander van Rijn
description: "Section 3: Software Development as a Process"
---

<!-- .slide: data-state="title" -->

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

/* Blockquote right double quotes */
.blockquote:after {
    position: absolute;
    content: "”";
    font-size: 10rem;
    line-height: 0;
    bottom: -43px;
    right: 30px;
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

# Software Development as a Process

===

<!-- .slide: data-state="standard 10" -->

## Programming vs Software Engineering

<div class="blockquote-wrapper fragment">
  <div class="blockquote" style="margin: 30px auto 0; font-size: smaller;">
    Software designed deliberately will be much easier to work with in the long term than software we build without a plan - time spent planning in advance will save you a lot more time later.
  </div>
</div>

==

<!-- .slide: data-state="standard 10" -->

## Programming vs Software Engineering

Software requirements, design, architecture and implementation as typical stages of a software development process
- Design requirements and constraints - what affects our design choices?
- Software design	
- Writing readable, maintainable and testable code
- Pure functions, classes and abstractions

Note:

The terms programming (or even coding) and software engineering are often used interchangeably. They are not. Someone who is engineering software takes a wider view:
The lifecycle of software: from understanding what is needed, to writing the software and using/releasing it, to what happens afterwards.
Who will (or may) be involved: software is written for stakeholders. This may only be the researcher initially, but there is an understanding that others may become involved later (even if that isn’t evident yet). A good rule of thumb is to always assume that code will be read and used by others later on, which includes yourself!
Software (or code) is an asset: software inherently contains value - for example, in terms of what it can do, the lessons learned throughout its development, and as an implementation of a research approach (i.e. a particular research algorithm, process, or technical approach).
As an asset, it could be reused: again, it may not be evident initially that the software will have use beyond its initial purpose or project, but there is an assumption that the software - or even just a part of it - could be reused in the future.

===

<!-- .slide: data-state="standard 10" -->

## Waterfall Software Development

<img src='./media/image32.jpeg'>

Note:

The software development process consists of multiple stages, which in the 'traditional (/ old fashioned)' waterfall model follows one step after another.
So far, you are all familiar with the "Implementation" step, as that 'simply' consists of the programming you're already doing, and you have worked a bit on the "testing" step too, to make sure what you've implemented is actually correct.
But it's also important to consider what you actually want to implement in the first place

*point out 'System Design'*

After all, it doesn't make sense to start programming if you haven't thought about what you're going to build in the first place.
But there's more you can take into account when designing your program than just how to implement and test it.

*point out 'Deployment' and 'Maintenance'*

How you deploy and eventually have/want to maintain your project can also influence your design decisions. 
Although Deployment and Maintenance are typically much less 'formal' in a research (and especially in an academic) setting compared to a corporate setting.
Think of the different in running your analysis for a paper compared to deploying a new version of the ns.nl website.
 
There is actually one more step in the process.
Just like you can't build without a design, you can't really design without knowing what you want.
 
*point out 'Requirement Gather & Analysis'* 
 
That's where properly specifying your requirements comes in.
Taking dedicated time to think about what the requirements of your project are can be vital in making the right (design) decisions at the start.
After all, the sooner you can correct or avoid a mistake, the cheaper it is.

==

<!-- .slide: data-state="standard 10" -->

<h2>Software development as a <i>continuous</i> process

<div style="font-size: smaller;">
Requirements will <i>almost always</i> change on reflection!
</div>

==

<!-- .slide: data-state="standard 10" -->

<img src='./media/image33.png'>

==

<!-- .slide: data-state="standard 10" -->

## 3.1 Software Requirements

Write them down so you only build what's actually needed!

<ul>
  <div class="fragment" data-fragment-index="1">
    <li>Start high level
    <ul><li>What goal am I trying to achieve?</ul>
  </div>
  <br>
  <div class="fragment" data-fragment-index="2">
    <li>Refine
    <ul><li>What feature do I need do achieve this?</ul>
  </div>
  <br>
  <div class="fragment" data-fragment-index="3">
    <li>Make specific
    <ul><li>How do I implement that?</ul>
  </div>
</ul>

Note:

For the first episode of this section, we'll focus on the requirements step. To really think about them, and give yourself the best chance of sticking to them later, it's best to actually write down your requirements.

This will probably feel like a lot of overhead, so will take some discipline. But by writing it down, you're forcing yourself to be specific, which helps to identify problems as soon as possible, saving you a lot of time later in the process.

When thinking about requirements of code, we should avoid the temptation to immediately think in terms of code, but instead start at a high level.

** reveal 'Start high level' **

First make sure you identify what goal you're actually trying to achieve. Again, we don't want to build anything we're never going to need.

** reveal 'Refine' **

When the goal is clear, we can refine it down to start defining features the software should have...

** reveal 'Make specific' **

… which can be further specified by implementation details.

These three levels can be named 'business', 'user, and 'solution', requirements. Although as the lesson materials mention, this naming scheme is actually quite arbitrary, and you may find different terminology being used in different contexts.

>> For this episode, talk through the exercises as a group.

===


