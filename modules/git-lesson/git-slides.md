---
title: Git and GitHub
type: slides
order: 1
---

<!-- .slide: data-state="title" -->

# Automated Version Control

What is version control and why should I use it?

Note:
- Git all set up?
- SSH working?
- Otherwise: breakout room

===

<!-- .slide: data-state="standard" -->
<img style="height: 70vh;" src="https://swcarpentry.github.io/git-novice/fig/phd101212s.png"/>

<span style="font-size: small;">“Piled Higher and Deeper” by Jorge Cham, http://www.phdcomics.com </span>

===

<!-- .slide: data-state="standard" -->
## Documents are...
<div class="fragment">
  a series of changes
  <img style="height: 30vh; margin: 0; padding: 0;" src="https://swcarpentry.github.io/git-novice/fig/play-changes.svg"/>
</div>

===

<!-- .slide: data-state="standard" -->
## Collaboration
<div style="float: left; width: 49%;">
  independent changes
  <img style="height: 350px;" src="./media/versions.svg"/>
</div>
<div class="fragment" style="float: right; width: 49%;">
  can be merged
  <img style="height: 350px;" src="./media/merge.svg"/>
</div>

===

<!-- .slide: data-state="standard" -->
## Version Control: Key Points

- Version control is track changes on steroids.
- Version control is like an unlimited **undo**.
- Version control also allows many people to work in parallel.

===

<!-- .slide: data-state="standard" -->
## The Holy Realms of Git

<img src="https://swcarpentry.github.io/git-novice/fig/git-staging-area.svg">

<ul>
  <li><b>workspace</b>&nbsp;&nbsp;📂</li>
  <ul>
    <li>Your filesystem</li>
  </ul>
  <li class="fragment"><b>index</b>&nbsp;&nbsp;🕒
    <ul>
      <li>Staging area</li>
      <li>Files wait patiently to be committed</li>
    </ul>
  </li>
  <li class="fragment"><b>local repository</b>&nbsp;&nbsp;🗂️
    <ul>
      <li>Contains branches, commits, history, etc.</li>
    </ul>
  </li>
<ul>

===

<!-- .slide: data-state="standard" -->
## Crowded Staging Area / Index

<img src="https://swcarpentry.github.io/git-novice/fig/git-committing.svg">

The Staging Area / Index can hold many files and folders.

===

<!-- .slide: data-state="standard" -->
## Quiz 1/2

<blockquote style="text-align: left;">
Which commit message should I choose?
<ol>
  <li>“Changes”</li>
  <li>“Added line ‘This project started as a joke’ to myfile.txt”</li>
  <li>“Discuss origin of the project”</li>
</ol>
</code></pre>
</blockquote>
<blockquote class="fragment" style="text-align: right;">
Make it short, descriptive, and imperative <span style="font-style: normal;">🐺</span>
</blockquote>
<blockquote class="fragment" style="text-align: right;">
So yeah, the last one is good! <span style="font-style: normal;">🐺</span>
</blockquote>

===

<!-- .slide: data-state="standard" -->
## Quiz 2/2

<blockquote style="text-align: left;">
Which command saves <b>myfile.txt</b> to my Git repo?<br>
<ol>
  <li>
    <pre style="width: 100%; font-style: normal;" data-id="code-animation"><code data-trim class="bash">
    $ git commit -m "my recent changes"
    </code></pre>
  </li>
  <li>
    <pre style="width: 100%; font-style: normal;" data-id="code-animation"><code data-trim class="bash">
    $ git init myfile.txt
    $ git commit -m "my recent changes"
    </code></pre>
  </li>
  <li>
    <pre style="width: 100%; font-style: normal;" data-id="code-animation"><code data-trim class="bash">
    $ git add myfile.txt
    $ git commit -m "my recent changes"
    </code></pre>
  </li>
  <li>
    <pre style="width: 100%; font-style: normal;" data-id="code-animation"><code data-trim class="bash">
    $ git commit -m myfile.txt "my recent changes"
    </code></pre>
  </li>
</ol>
</code></pre>
</blockquote>
<blockquote class="fragment" style="text-align: right;">
3. adds your file to the index, and then commits it. That's the one.
<span style="font-style: normal;">🐺</span>
</blockquote>


===

<!-- .slide: data-state="standard" -->
## Tracking Changes: Key Points

- Files can be stored in
  - **working directory**: the files you can see
  - **staging area / index**: files about to be committed
  - **local repository**: the permanent record
- **git status**&nbsp; shows the status of a repository
- **git add**&nbsp; puts files in the staging area
- **git commit**&nbsp; saves the staged content as a new commit in the local repository
- Write short, descriptive, and imperative commit messages

===

<!-- .slide: data-state="standard" -->
## Exploring history
<img src="https://carpentries-incubator.github.io/collaborative-git-and-github-lesson/fig/git-restore.svg">

Use `git restore` with the `-s` option to retrieve a specific state. 

Note:
In this example we restore to the state before the most recent commit, 
which is `HEAD~1` or `f22b25e`

===

<!-- .slide: data-state="title" -->
## Git branches

===

<!-- .slide: data-state="standard" -->
## What is a branch?
<div style="float: left; width: 49%;">
  A branch is simply a pointer to a commit
  <img src="./media/main-branch.png"/>
</div>
<div class="fragment" style="float: right; width: 49%;">
  Creating a branch only creates a new pointer, nothing changes in your code
  <img src="./media/crazy-experiment-branch.png"/>
</div>

Note:
In git a branch is effectively a pointer to a snapshot of your changes. 
It’s important to understand that branches are just pointers to commits. 
When you create a branch, all Git needs to do is create a new pointer, 
it doesn’t change the repository in any other way.
Images come from https://carpentries-incubator.github.io/advanced-git/02-branching/index.html

===

<!-- .slide: data-state="standard" -->
## A branching workflow
<img style="height: 350px;" src="./media/branching-example.png">

Whenever you add a new feature or fix a bug, you work on a new branch.

Note:
Branching is a feature available in most modern version control systems. 
Branching in other version control systems can be an expensive operation in both time and disk space. 
In git, branches are a part of your everyday development process. 
When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch 
to encapsulate your changes. 
This makes it harder for unstable code to get merged into the main code base, 
and it gives you the chance to clean up your future’s history before merging it into the main branch.

===