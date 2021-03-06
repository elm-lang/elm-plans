# Guidelines for Goal-Oriented Discussions

Communities are built around some sort of shared experience. For this discussion, they fall roughly into these categories:

![communities for what?](communities.png)

Every community will fill some subset of these roles in varying degrees.

  * On elm-discuss it is mostly about expression, partly for connection
  * On twitter or /r/elm it is more about connections, but a lot about expression
  * On GitHub it is primarily for action

This document describes how to organize on GitHub to acheive collective action most effectively. Unlike discussions for expression, discussions for action can succeed or fail. Discussions can be efficient or innefficient. It's weird. I am calling these **goal-oriented discussions**. This document outlines how to engage in efficient and enjoyable goal-oriented discussions for [bug reports](#bug-reports), [pull requests](#pull-requests), and [design discussions](#design-discussions).

<br>

## Bug Reports

The big thing here is "leave nothing to the imagination". The more specific you are, the more quickly we can help! So the basic rules are:

  * **Title** &mdash; Provide a title that summarizes your problem as clearly and specifically as possible.
  * **Minimal Reproduction** &mdash; Provide [a minimal reproduction](http://sscce.org/) of the issue. Ideally this is a code snippet that fits in the issue and can be run in elm-lang.org/try
  * **Error Message** &mdash; If there is an error message associated, include it in the issue. This way folks can assess the situation directly from the issue, no extra steps.
  * **Environment** &mdash; Describe the environment where you observed the issue. Which OS? Which browsers? Is a certain directory structure required?
  * **Curation** &mdash; As more is learned about the issue, a maintainer should update the title as necessary to make it easier to understand and find when it is just in a big issue list.

#### Handling Duplicates

  * Close all the relevant user submitted issues
  * Open a new meta issue describing the problem in its purest most minimal form
  * Link to all the duplicates from the meta issue so we can check their code snippets when we have a solution

<br>

## Pull Requests

#### Submitting

  * **Title** &mdash; clearly describe the problem that is solved.
  * **Performance** &mdash; outline any performance concerns. Maybe there are none, maybe some overhead is introduced. Document that in the initial description. Provide benchmarks as necessary.
  * **Tests** &mdash; how did you test this code? How can we reproduce those tests easily? Can the tests be added into the repo easily? If so, add this as part of the PR.
  * **Style** &mdash; make sure that you are in line with the appropriate style guides:  [Elm](http://elm-lang.org/docs/style-guide), [Haskell](https://gist.github.com/evancz/0a1f3717c92fe71702be), and [JS](http://google.github.io/styleguide/javascriptguide.xml). Make sure your style (comments, indentation, new lines) are in line with the file you are modifying.

#### Commenting

  * **Details** &mdash; Sort out any style, performance, or correctness issues.
  * **Blockers** &mdash; Document if there is any design questions that might block this. Key weaknesses? Better approach is possible? etc. Document these.
  * **Curation** &mdash; If things are blocked close the PR and open an issue describing the state of affairs.

<br>

## Design Discussions

#### Goals

  - **Division of labor** &mdash; get feedback on ideas in a way that *efficiently* uses the time of the originator and commenters
  - **Curation** &mdash; curate discussions so someone looking over them can quickly understand what is going on
  - **Turn Talk to Action** &mdash; turn talk into concrete and productive actions that can be handled by specific individuals. The easier it is to distribute the workload the better!
  - **Avoid Syntax Wars** &mdash; make discussions more robust to derailing via syntax concerns


#### Basic Guidelines

Issue comments are excellent at finding "this seems not so good" and "how about this idea?" and "we need to benchmark this first". That said, issue comments are *not* good at bringing these things all together in a coherent way. Without curation, good ideas can get lost and it becomes tricky to turn them into concrete and productive action.

So productive comments on a design discussion include things like:

  * Concrete examples that may pose problems
  * Concerns about learning, efficiency, etc.
  * Ideas of how to do things in a nicer way

As progress is made on these, the original description should be updated to the latest state of affairs. OP is in charge of managing this curation.


#### Curation

What happens when there are two design discussions about the same general problem? What happens when one discussion has gotten out of control?
 
Over time, every discussion will spiral out of control, leaving an issue with tons of comments that are difficult to follow. This is especially bad if someone comes back months later to an issue that is 50 comments long. When a discussion becomes unmanagable, the next steps are:

  1. Close the issue.
  2. Create a meta issue that:
      - links to the old issue
      - summarizes any unanswered questions
  3. Any potential alternative ideas are turned into issues describing the alternative completely. The originator of the idea should do this.
  4. As alternatives come into existence:
      - edit the root comment in the meta issue to link to the alternative
      - close the issue describing the alternative, but continue discussion of specifics there

So the goal here is to break the problem down into coherent subparts and organize things such that someone can quickly understand the problem and the state of affairs within that realm.


#### About Syntax and Naming

This is the number one way to waste time and derail discussions. It is extraordinarily tempting to do, even if you know it will hurt the discussion. It is also very important to get it right.

If you see someone talking about this in a discussion *not* about syntax, do not engage. Sometimes to keep a discussion on track you must pretend parts of it did not happen. This way ideas can be shared without side-tracking everything.

If you *need* to discuss syntax directly, collect all the suggestions in separate issue and run things in an evidence based way:

  * **Opinions do not matter** &mdash; No one's opinion matters because everyone participating in these discussions is atypical by virtue of being here. What you think does not represent the present and future users of this language, so don't put too much weight on it.
  * **Historical Context** &mdash; Does this appear in other languages? If so, what does it look like in all of them? List that explicitly so we know the context.
  * **Code Examples** &mdash; Get code examples from real code and create a gist demonstrating the proposed syntax.
  * **Technical Problems** &mdash; Can it be parsed unambiguously?

Once the organization is done, the issue is blocked until Evan can review things and do a user study on how things work in practice. Further comment and opinions on the existing cannot change the fundamentals of those ideas.
