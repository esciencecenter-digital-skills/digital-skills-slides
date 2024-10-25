---
title: Testing
type: slides
order: 4
author: Ole Mussmann
description: Getting more professional
---

<!-- .slide: data-state="blue_overlay yellow_flag yellow_strip purple_half_circle_bottom purple_blob right_e_top" data-background-video="./media/testing/606762245.mp4" data-background-video-loop data-background-video-muted="true" -->
<!-- https://pixabay.com/videos/engine-motor-mechanic-technology-5497/ -->

# Testing

===

<!-- .slide: data-state="standard"  -->

## Basics of testing

### Mistakes *will* happen!


<div style="display: flex; justify-content: center; align-items: center">
    <div>
      <ul>
        <li class="fragment">The more complex the code, the harder to keep an eye on everything.</li>
        <li class="fragment">However, we can build safeguards against problems:
        <ul>
          <li class="fragment">Throwing exceptions</li>
          <li class="fragment">Logging (intermediate) results</li>
          <li class="fragment"><b>Writing tests</b></li>
        </ul></li>
      </ul>
  </div>
    <img src="./media/testing/Doh.png" width="250">
</div>

===

<!-- .slide: data-state="standard" -->

## Why Test?

<div style="display: flex; justify-content: center; align-items: center">
  <div>
    <ul>
      <li class="fragment">Preserve functionality
      <ul>
        <li>Detect (new) errors early</li>
        <li>Avoid unexpected outputs</li>
      </ul></li>
      <li class="fragment">Help users
      <ul>
        <li>Verify correct installation</li>
        <li>Ensure reproducibility</li>
      </ul></li>
      <li class="fragment">Enable developers
      <ul>
        <li>Manage complexity</li>
        <li>Simplify refactoring</li>
        <li>Facilitate collaboration</li>
      </ul></li>
    </ul>
  </div>
    <img src="./media/testing/experiment.webp" width="400" style="margin-left: 60px">
</div>


===

<!-- .slide: data-state="standard" -->

## Test Types

<ul>
    <li class="fragment">Exceptions in the code base
    <ul>
      <li>Intended to handle "expected" problems</li>
      <li>Sound an alarm as soon as the problem arises</li>
      <li>Provide clear feedback to the user</li>
  </ul></li></span>
  <li class="fragment">Unit testing
  <ul>
    <li>Smallest possible unit (module)</li>
    <li>No dependency on outside code...</li>
    <li>(... replace them with mocks, stubs, etc.)</li>
  </ul></li>
  <li class="fragment">Integration testing
  <ul>
    <li>Test interactions between units</li>
    <li>Can be on small scales, system wide, ...</li>
  </ul></li></span>
</ul>

===

<!-- .slide: data-state="standard" -->

## Testing frameworks

Most modern programming languages have good options to streamline testing

- Python: [Pytest](https://docs.pytest.org/en/7.3.x/)
- Java: [Junit](https://junit.org/junit5/)
- R: [testthat](https://testthat.r-lib.org/)
- Matlab: [Testing Frameworks](https://nl.mathworks.com/help/matlab/matlab-unit-test-framework.html?s_tid=CRUX_lftnav)
- Julia: [Test](https://docs.julialang.org/en/v1/stdlib/Test/)
- C++: [GTest](https://google.github.io/googletest/) (developed by Google) or [Catch2](https://catch2-temp.readthedocs.io/en/latest/index.html)
- etc.

===

<!-- .slide: data-state="standard" -->


## Testing metrics

#### Targets are arbitrary and indicative

<div style="display: flex; justify-content: center; align-items: center">
  <div>
    <ul>
      <li class="fragment fade-up">Coverage
        <ul>
          <li>Proportion of code that is executed</li>
          <li>Target >= 80%</li>
        </ul>
      </li>
      <li class="fragment fade-up">Ratio (lines of code:lines of test)
        <ul>
          <li>Target: (1:3)</li>
        </ul>
      </li>
      <li class="fragment fade-up">Metrics can be misleading
        <ul>
          <li>They do not measure quality</li>
          <li>Don't get blindsided by hitting targets over writing good tests</li>
  </div>
  <img src="./media/testing/metrics.jpg" width="300" style="margin-left: 60px">
</div>

===

<!-- .slide: data-state="standard" -->

## Take-away

- Use pure functions when possible 👌
  - Do you remember what these are? 💭
- Testing does not have to be hard 👏
  - You often test anyway, but then throw the test away 🧐
  - Use pytest if programming with Python 🎭
- You don't have to strive for 💯% test coverage
  - But be smart about what you are testing 🧠
- Aim for a balance between unit- and integration tests ⚖️
- Testing removes the dread of refactoring 🔁
- Your future you (and others!) will thank you 🙏
