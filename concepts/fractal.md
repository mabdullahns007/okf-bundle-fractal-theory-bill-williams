---
type: Concept
title: Fractal (market)
description: Williams' bar-pattern definition of a market fractal, its grounding in Mandelbrot's fractal geometry, and the breakout-entry rule built on it.
tags: [trading, fractals, entry-rules]
sources:
  - id: practical-fractal-video
    resource: https://www.youtube.com/watch?v=bNxt298VVOw
    title: "The Practical Fractal: The Holy Grail to Trading"
    author: "Bill Williams, PhD"
generated: {by: claude-code/sonnet-5, at: 2026-08-28T00:00:00Z}
status: draft
---

# Fractal (market)

## Mathematical grounding

Williams traces "fractal" to Benoit Mandelbrot, who resolved a centuries-old puzzle about non-integer dimensionality (a sufficiently wiggly line can partially fill a plane, giving it a dimension between 1 and 2) and measured the Mississippi River's fractal dimension at 1.2610. Williams recounts that when IBM later asked Mandelbrot to find an economically useful application of this, he measured corn and cotton price series and found the *same* fractal dimension to three decimal places — later replicated on other rivers. Williams treats this as evidence that markets are a natural phenomenon shaped by an underlying "strange attractor," not a man-made mechanism, and says the realization kept him up all night.[^practical-fractal-video]

## Market definition — the "five-fingered boogie"

A minimum of 5 bars. An **up-fractal** is a bar higher than the two bars immediately before it and the two immediately after it (tied middle bars, or extra bars, are still valid provided nothing in the two-bar window on either side exceeds the center bar). A **down-fractal** is the mirror image.[^practical-fractal-video]

Sub-types named in the talk: **initiating fractal**, **breakout fractal**, and **responsive fractal** — together forming the "space" dimension of the [five dimensions of market structure](/concepts/five-dimensions-of-market-structure.md).[^practical-fractal-video]

## Entry rule

Place a buy-stop one tick above a confirmed up-fractal (sell-stop one tick below a down-fractal). Williams is explicit that this is, by construction, a breakout entry: it gives you the worst possible trade location and the maximum potential risk on that specific entry — but it guarantees you're never left out of a genuine trend. He calls a fractal breakout that catches a real trend a **"blind chicken trade"** — easy once the trend is underway — and notes fractal entry is deliberately the *fourth* of the five dimensions to act on, not the earliest or most profitable one.[^practical-fractal-video]

Context he gives for why this matters: markets trend only ~15–30% of the time; the other ~70% is non-trending/choppy, so a mechanical breakout rule needs the rest of the system (see the [stop-placement rule](/concepts/stop-placement-rule.md)) to survive the chop.[^practical-fractal-video]

## Where it's claimed to work

Demonstrated live in the talk on Japanese yen (see [case study](/case-studies/yen-fractal-trade-case-study.md)) and on inter-currency spreads (Swiss franc/yen, Deutsche mark/yen), and claimed to apply to options and stocks — with an in-progress book applying it specifically to equities, said to work *more* precisely on high-cap, high-volume stocks than on commodities.[^practical-fractal-video]

## Related

- [Balance line](/concepts/balance-line.md)
- [Five dimensions of market structure](/concepts/five-dimensions-of-market-structure.md)
- [Stop-placement rule](/concepts/stop-placement-rule.md)
- [Japanese yen fractal trade (case study)](/case-studies/yen-fractal-trade-case-study.md)

[^practical-fractal-video]: Bill Williams, *The Practical Fractal: The Holy Grail to Trading*.
