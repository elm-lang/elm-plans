# Elm Plans

A central home for future plans for [Elm](http://elm-lang.org).

As Elm is a young, evolving language, nothing is set in stone...keep in mind
that these plans might very well change, a lot, and on short notice!


## Feature Requests

When you want a new feature to the language or core tools, open an issue here
proposing the idea.

The Elm community tends to discuss things thoroughly, request before-and-after
examples and specific motivating use cases, and generally hold proposals to a
high standard. Please be prepared for that if you submit one! See the
[String Interpolation Proposal](https://github.com/elm-lang/elm-compiler/issues/905)
as an example.


## Collaborate

We have a nice list of [projects](https://github.com/elm-lang/projects) that
would work great as community projects!


## Planned for Next Release (Elm 0.16)

These are currently planned for the next release.

1. [Self-Tail-Call Optimization](https://groups.google.com/d/msg/elm-dev/mmcqrySAxzs/yWJf0elgUooJ)
2. [String Interpolation](https://github.com/elm-lang/elm-compiler/issues/905)
3. [Warnings for inexhaustive and redundant pattern matches](https://github.com/elm-lang/elm-compiler/pull/924)
4. Many bugfixes and improvements to [elm-reactor](https://github.com/elm-lang/elm-reactor)
5. [Versioned build-artifacts/ directory](https://github.com/elm-lang/elm-plans/issues/1)


## Coming Soon

These aren’t planned for the next release, but could be a release or two away from that one.

1. Improved way to develop Native modules
2. Revisiting various aspects of Signal and Mailbox
3. The ability to serialize union types through ports
4. Some way to run logic when elm-html creates, modifies, and removes actual DOM elements. This will make integrating with third-party JS libraries substantially easier.


## Coming Eventually

It’s intended that these will make it into the language someday, but they are not a priority in the near term. Don’t expect them for a long time.

1. Improved code reuse. This could involve some combination of Rank-N types, Higher-Kinded Polymorphism, typeclasses, or none of these. Since there have been several questions about this in various places, @evancz posted an explanation of [the philosophy behind Elm’s direction on code reuse](https://groups.google.com/forum/#!msg/elm-discuss/oyrODCgYmQI/T2I_8L-AL6EJ). The short version is that the aforementioned features are on the radar and well-understood (and used in [Elm’s compiler](https://github.com/elm-lang/elm-compiler/), which is written in Haskell), but none of the existing implementations are a good fit for what Elm wants to be. It’s possible that Elm might never incorporate these exact features, so please don’t make plans assuming it will!
2. Source Maps
3. IDE support
4. Alternative compilation targets besides in-browser JavaScript


## Open for Discussion

See the [list of Open Proposals](https://github.com/elm-lang/elm-plans/issues?q=is%3Aopen+is%3Aissue+label%3Aproposal).


## Decided Against

See the [list of Closed Proposals](https://github.com/elm-lang/elm-plans/issues?utf8=%E2%9C%93&q=is%3Aclosed+is%3Aissue+label%3Aproposal+).