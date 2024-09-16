---
title: CI
type: slides
order: 5
author: Ole Mussman
description: Day 3 Code Refinery
---


<!-- .slide: data-state="title" -->

# Continuous Integration

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
    font-size: 1 rem;
    font-weight: normal;
    line-height: 1;
    margin: 0;
    padding-top: 20px;
    z-index: 1;
}

</style>

# Continuous Integration (CI)

<div class="blockquote-wrapper fragment">
  <div class="blockquote">
     maintain the main version of a project via frequent or automated integration of changes.
    <h4>&mdash;</h4>
  </div>
</div>

===

<!-- .slide: data-state="standard" -->


# Motivation
How can we implement __automatic testing__ each time we push changes to the repository? 

<img src="./media/ci/automate.jpg">


===

<!-- .slide: data-state="blue_overlay yellow_flag logo 9" data-background="./media/ci/reload-97640.svg" data-background-size="50%" -->

## CI includes automatic testing!

Allows to identify any conflicts and bugs that are introduced by changes, so they are found and fixed early, minimising the effort required to do so. 

===

<!-- .slide: data-state="standard" -->

## What else?
- Building & compiling
  - Code, Documentation, ...
- Deploying (PyPi, Kubernetes, GitHub Pages)
  - Just like these slides
- Code analysis
    - linting (style conventions), formatting, quality metrics, ...
- Security analyses
- Send messages
  - Slack, Discord, Matrix, Mastodon, email, ...


===


<!-- .slide: data-state="standard" -->

## CI service providers

- GitHub Actions
- GitLab CI
- Azure Pipelines
- Jenkins
- etc

===

<!-- .slide: data-state="standard" -->

## Take-away

- Best practices are a time-investment _with returns_
- CI saves time and keeps your project clean
- What improvements could your project benefit from?
- What's nice to know, but overkill for your current work?

===

<!-- .slide: data-state="standard" -->

## Hands-On

<div style="float: left; width: 60%; margin-bottom: 1em;">
  <ol>
    <li><strong>Person A: </strong>Ensure your repository has tests</li>
    <li><strong>Person A: </strong>Set up Continuous Integration (automatic testing)</li>
    <li><strong>Person A: </strong>Verify that tests ran</li>
    <li><strong>Person A: </strong>Add a test that fails</li>
    <li><strong>Person A: </strong>Open an issue</li>
    <li><strong>Person B: </strong>Fork ⚠️ and clone person A's repo</li>
    <li><strong>Person B: </strong>Fix the broken test</li>
    <li><strong>Person B: </strong>Open a pull request linked to the issue</li>
    <li><strong>Person B: </strong>Verify that tests now run</li>
    <li><strong>Person A: </strong>Accept Person B's pull request</li>
  </ol>
</div>
<img style="float: right; width: 39%;" src="./media/ci/full-cycle-ci.png">


