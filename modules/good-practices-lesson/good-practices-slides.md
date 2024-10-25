---
title: Good Practices
type: slides
order: 1
author: Ole Mussmann
description: Getting more professional
---

<!-- .slide: data-state="title" -->

# Good Practices for Research Software Development

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

<!-- .slide: data-state="standard"  -->

## Who are we?

+ **The Netherlands eScience Center is a national center for innovative software solutions in academic research**
+ **Our Research Software Engineers**
  - Help researchers interpret results
  - Make tools and methods reusable for the wider research community
  - Co-author research and methodological publications. 

===


## Programming vs Software Engineering

<div class="blockquote-wrapper fragment">
  <div class="blockquote">
      Software engineering is programming integrated over time.
    <h4>&mdash;Titus Winters, Google C++ devlead</h4>
  </div>
</div>

Note:
What's the difference between programming and software engineering?

===

<!-- .slide: data-state="standard" -->

<img width="800" alt="development speed" src="./media/good-practices/development-speed.svg">

===

<!-- .slide: data-state="standard" -->

## Development Speed ⚡

<div style="float: left;">
<ul>
  <li>Red curve
  <ul>
    <li>Writing code</li>
  </ul>
  <li>Blue curve
  <ul>
    <li>Version Control</li>
    <li>Collaborative development</li>
    <li>Code review</li>
    <li>Testing</li>
    <li>Modular code</li>
    <li>Documentation</li>
  </ul>
</ul>
</div>

===

<!-- .slide: data-state="standard" -->

## Projects are Different

<img style="height: 70vh;" src="./media/good-practices/branching.png"/>

===

<!-- .slide: data-state="standard" -->

## What to Use When?

<div style="width: 49%; float: left; font-size: smaller;">
  <table>
    <tr>
      <th>⏱️&nbsp;lifetime</th>
      <th>use</th>
    </tr>
    <tr>
      <td>1-shot</td>
      <td class="fragment" data-fragment-index="1">🚫</td>
    </tr>
    <tr>
      <td>week+</td>
      <td class="fragment" data-fragment-index="2">Git &amp; GitHub</td>
    </tr>
    <tr>
      <td>3 months+</td>
      <td class="fragment" data-fragment-index="3">Testing</td>
    </tr>
    <tr>
      <td>6 months+</td>
      <td class="fragment" data-fragment-index="4">Documentation,<br>automate testing</td>
    </tr>
  </table>
</div>

<div style="width: 49%; float: right; font-size: smaller;" class="fragment" data-fragment-index="5">
  <table>
    <tr>
      <th>🧑🧑&nbsp;users</th>
      <th>use</th>
    </tr>
    <tr>
      <td>1</td>
      <td class="fragment" data-fragment-index="6">Push to main</td>
    </tr>
    <tr>
      <td>2+</td>
      <td class="fragment" data-fragment-index="7">Branches, merging</td>
    </tr>
    <tr>
      <td>2+ (+students)</td>
      <td class="fragment" data-fragment-index="8">Code review</td>
    </tr>
    <tr>
      <td>2+ (+external)</td>
      <td class="fragment" data-fragment-index="9">Release branch, <br>&amp; everything else</td>
    </tr>
  </table>
</div>

Note:
- Train these tools
- Experience their effect
- Use own judgement, but
- avoid "but in my project..."

===

<!-- .slide: data-state="standard" -->

## Good practices are investments

Profits come in

- Development efficiency
- Reproducibility
- Reusability
- Faster debugging
- Robustness, fewer errors
- Fewer headaches!