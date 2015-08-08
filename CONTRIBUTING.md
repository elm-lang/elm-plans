## Bug Reports

The big thing here is "leave nothing to the imagination". The more specific you are, the more quickly we can help! So the basic rules are:

  * **Title** &mdash; Provide a title that summarizes your problem as clearly and specifically as possible.
  * **Repro** &mdash; Provide a minimal reproduction of the issue. Ideally this is a code snippet that fits in the issue and can be run in elm-lang.org/try
  * **Error Message** &mdash; If there is an error message associated, include it in the issue. This way folks can assess the situation directly from the issue, no extra steps.
  * **Environment** &mdash; Describe the environment where you observed the issue. Which OS? Which browsers? Is a certain directory structure required?
  * **Curation** &mdash; As more is learned about the issue, a maintainer should update the title as necessary to make it easier to understand and find when it is just in a big issue list.

If duplicates start to appear:

  * Close all the relevant user submitted issues
  * Open a new meta issue describing the problem in its purest most minimal form
  * Link to all the duplicates from the meta issue so we can check their code snippets when we have a solution


## Design Discussions

#### Goals

  - **Division of labor** &mdash; get feedback on ideas in a way that *efficiently* uses the time of the originator and commenters
  - **Curation** &mdash; curate discussions so someone looking over them can quickly understand what is going on
  - **Turn Talk to Action** &mdash; turn talk into concrete actions that can be handled by the community


#### Guidelines

Issue comments are excellent at finding "this seems not so good" and "how about this idea?" and "we need to benchmark this first". That said, issue comments are *not* good at bringing these things all together in a coherent way. Without curation, good ideas can get lost and it becomes tricky to turn them into concrete and productive action.

So productive comments on a design discussion include things like:

  * Concrete examples that may pose problems
  * Concerns about learning, efficiency, etc.
  * Ideas of how to do things in a nicer way

As progress is made on these, the original description should be updated to the latest state of affairs.
  
Even with that curration, the danger is that things spirals out of control, leaving an issue with tons of comments that are difficult to follow. This is especially bad if someone comes back months later to an issue that is 50 comments long. When a discussion enters this death spiral, the next steps are:

  1. Close the issue.
  2. Create a meta issue that:
      - links to the old issue
      - summarizes any unanswered questions
  3. Any potential alternative ideas are turned into issues describing the alternative completely. The originator of the idea should do this.
  4. As alternatives come into existence:
      - edit the root comment in the meta issue to link to the alternative
      - close the issue describing the alternative, but continue discussion of specifics there

So the goal here is to break the problem down into coherent subparts and organize things such that someone can quickly understand the problem and the state of affairs within that realm.
