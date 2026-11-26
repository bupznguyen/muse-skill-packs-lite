---
name: pinterest-analytics
description: Analyze Pinterest data from any source — CSV exports, PDF reports, dashboard screenshots, and trend reports like Pinterest Predicts or Pinterest Trends — to find top-performing pins, rank trending search demand, track performance over time, and produce polished client-ready reports. Use this skill whenever the user mentions Pinterest data, pins, boards, Pinterest Analytics, Pinterest Predicts, trend reports, impressions/saves/outbound clicks, or uploads files that look like Pinterest exports, dashboard screenshots, or Pinterest trend forecasts, even if they just say "analyze this" or "make a report from this" without naming Pinterest explicitly. Also use it for month-over-month Pinterest comparisons, content strategy or content calendar recommendations based on pin performance or search trends, and combining multiple Pinterest files into one report.
---

# Pinterest Analytics

Turn raw Pinterest data (CSVs, PDFs, dashboard screenshots) into insight and client-ready reports.

## Why this skill exists

Pinterest data arrives messy and in mixed formats — PDF summaries, dashboard screenshots, CSV exports whose structure varies by page. The goal: figure out what content is working, how performance is moving, and communicate it clearly. The deliverable is insight, not a data dump.

## Workflow overview

1. **Ingest** every file the user provides
2. **Normalize** into one tidy dataset
3. **Analyze** — top performers, trends, and anything the user specifically asked for
4. **Report** — pick the right deliverable format and build it

## Step 1: Reading each input type

Inventory all uploaded files first; every file is a data source. CSV exports come in pin-level, time-series and ads shapes — match columns by meaning, not exact name, and convert text-formatted numbers before doing math. From PDFs, extract tables and stated metrics, always capturing the reporting period. From screenshots, transcribe every legible number and date range before analyzing; if a chart has no readable values, describe the trend's shape and say so — **never invent numbers a screenshot doesn't show**. Flag unreadable files and missing pieces (e.g. the date range) instead of guessing.

## Step 2: Normalizing the data

Build one tidy dataset (or two: pin-level and time-series), recording source file, metric, value, date/period and pin/board identifiers. Watch for the Pinterest-specific traps: overlapping export periods (deduplicate by date, flag it), impressions ≠ success (never rank top pins by impressions alone), fresh-pin bias (normalize by days live before comparing), mixed granularity (never sum a time-series file with a lifetime pin export).

## Step 3: Analysis

Keep the two kinds of data separate: **performance data** (how the account's own pins did) answers "what's working for us"; **demand data** (Pinterest Predicts, Pinterest Trends) answers "what the audience wants next." Compute, when the columns exist: **Engagement rate** = Engagements / Impressions · **Save rate** = Saves / Impressions (the strongest resonance signal) · **Outbound click rate** = Outbound clicks / Impressions · **Clicks per save**. Rank top performers on the metric matching the user's goal, note *why* each likely performed, and surface underperformers too. For trends: aggregate daily to weekly beyond ~6 weeks, read seasonality with Pinterest's 2–3 month planning lead time, compare like periods first. For demand reports, capture every search term with its growth figure and the analysis period, rank trends programmatically (never by eye), and turn demand into a dated content calendar. **Never present forecast data as performance data.** End with 3–5 specific, data-grounded recommendations — or say what export would unlock them.

## Step 4: The deliverable

Format follows audience: an Excel workbook for client/team reports, a Word document for formal deliverables, a compact in-chat table for a quick look. Every report follows one structure: executive summary, performance overview, top content, trends, recommendations, and data notes (sources, periods, gaps, assumptions) — not optional when inputs were mixed.

## Full version

This is a free lite preview. The complete skill — with all checklists, templates and references — is in the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
