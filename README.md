# StonkDesk

**A personal stock-research and data-monitoring prototype that keeps evidence, dates, and uncertainty visible.**

Built with AI-assisted development. This public repository contains screenshots and a project overview; application source and operational data remain private.

## What it does

StonkDesk brings retained company filings, historical price context, macro observations, and collection health into a local research interface. Each source keeps its own dates and evidence references. Opening a research page reads retained data rather than starting a new acquisition.

The interesting part is handling imperfect inputs: missing observations stay missing, overlapping accounting concepts stay unresolved, and a requested date range is distinguished from the data actually returned.

## Research brief

**All screenshots use invented fixture data in an isolated demo with outbound requests blocked.** Real ticker labels identify demo cases; prices, fundamentals, dates, and watchlist membership are synthetic. These are actual application captures, not design mockups or investment results.

![Synthetic research brief showing separate source dates and missing-evidence warnings](images/research-brief.png)

This example has company and market evidence but no macro acquisition or retained watchlist notice. The page exposes those gaps and keeps overlapping debt observations unresolved.

## Company comparison

![Synthetic company comparison with explicit source and reporting-period boundaries](images/company-comparison.png)

The comparison aligns metric names while preserving each company's reporting periods, warnings, and source dates. It does not turn mismatched observations into a common score or recommendation. Watchlist labels above belong to the demo fixture.

## Examples of data-quality behavior

| Situation | How it is represented |
| --- | --- |
| No retained change notice | Missing evidence, rather than a claim that nothing changed |
| No retained macro acquisition | An unavailable section with an explicit warning |
| Overlapping debt concepts | An unresolved value rather than double-counting |
| Different reporting periods | Each company's own period is retained |
| Returned market data ends before the requested range | A separate latest-observation date and an explicit warning |

The Collector Observatory also distinguishes unobserved scheduled runs, recorded failures, and integrity mismatches. An absent run record alone does not prove why a scheduled run was missed.

## Status and verification

This is an ongoing personal project, not a public trading service. There is no hosted demo or application download in this repository.

For this showcase, the research and comparison pages were opened and visually checked using isolated synthetic fixtures. The implementation and automated test sources were also reviewed for the behaviors described here; the full automated suite was not rerun for this publication. These checks are separate from manual testing performed by the project owner.

The screenshots demonstrate interface behavior, not provider reliability, investment performance, or production readiness. Historical adjusted series and current-vintage macro observations should not be treated as point-in-time backtest evidence.

## About

I'm Chase. I choose the direction, explore features, and use AI assistance to implement and refine my projects. StonkDesk is an exercise in making research software explain what it knows and what it cannot establish.

[More projects](https://github.com/chaser777f)
