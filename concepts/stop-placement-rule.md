---
type: Concept
title: Stop-placement rule
description: Williams' rule for where to place a protective stop once in a fractal-breakout position — two fractals back in the opposite direction, with a tie-break rule.
tags: [trading, risk-management, entry-rules]
sources:
  - id: practical-fractal-video
    resource: https://www.youtube.com/watch?v=bNxt298VVOw
    title: "The Practical Fractal: The Holy Grail to Trading"
    author: "Bill Williams, PhD"
generated: {by: claude-code/sonnet-5, at: 2026-08-28T00:00:00Z}
status: draft
---

# Stop-placement rule

Once in a position entered via a [fractal](/concepts/fractal.md) breakout, Williams places the protective stop at the **second-most-recent fractal** in the opposite direction. If that second-back fractal sits *closer* to price than the first-back one (i.e. they conflict), he uses whichever of the two is furthest from price.[^practical-fractal-video]

This rule is what lets the fractal breakout method (deliberately the worst-location, highest-initial-risk entry) survive the roughly 70% of the time markets aren't trending — see [Fractal (market)](/concepts/fractal.md) for that context.

[^practical-fractal-video]: Bill Williams, *The Practical Fractal: The Holy Grail to Trading*.
