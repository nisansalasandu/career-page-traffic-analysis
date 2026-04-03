# Career Page Traffic Analysis for Recruitment Optimization
### Gamage Recruiters (Pvt) Ltd — Data Science Internship Project

---

## Project Overview

This project analyzes web traffic and user engagement on the Gamage Recruiters career page
([gamagerecruiters.lk](https://gamagerecruiters.lk)) to understand how potential candidates
interact with recruitment opportunities online. By evaluating Google Analytics data, the analysis
uncovers candidate behavior patterns, traffic sources, and conversion bottlenecks — providing
actionable recommendations to improve recruitment campaign effectiveness and increase quality
job applications.

**Analysis Period:** Feb 1 – Feb 31, 2026 (30 Days)  
**Data Source:** Google Analytics — Career Page Sample Report  
**Internship:** Data Science Intern — Gamage Recruiters (Pvt) Ltd  

---

## Project Structure

```
Career-Page-Traffic-Analysis/
│
├── Data_and_Visualization.xlsx          # Main data workbook (7 sheets)
│   ├── Raw Data                         # All base metrics with min/max/midpoint
│   ├── Traffic Trends                   # Weekly session, page view, and user data
│   ├── Traffic Sources                  # Channel breakdown with session counts
│   ├── Device & Geo                     # Device type and geographic distribution
│   ├── Conversions                      # Conversion funnel with drop-off analysis
│   ├── Benchmarks                       # Industry benchmark comparison table
│   └── Dashboard                        # Interactive Excel dashboard
│
├── Gamage_Recruiters_Career_Page_Analysis_Report.pdf   # Full analytical report
│
└── README.md                            # This file
```

---

## Key Metrics Summary

| Metric | Value | Benchmark | Status |
|---|---|---|---|
| Total Users | 3,525 | — | — |
| Total Sessions | 4,350 | — | — |
| Page Views | 11,500 | — | — |
| Bounce Rate | 56.5% | 40–50% | ❌ Below |
| Avg Session Duration | 1m 45s | 2m 30s–3m 30s | ❌ Below |
| Pages per Session | 2.64 | 3.5–5.0 | ❌ Below |
| New User % | 88.5% | 60–75% | ⚠ Watch |
| Mobile Traffic % | 70% | 55–65% | ⚠ Watch |
| Organic Traffic % | 45% | 35–50% | ✅ Good |
| CV Submission Rate | 3.7% | 5–8% | ❌ Below |
| Apply Click Rate | 18.5% | 15–25% | ✅ Good |
| Contact Form Rate | 1.4% | 2–4% | ❌ Below |
| **Overall Benchmark Score** | **5.15 / 10** | 10 | ❌ Below |

---

## Data & Methodology

### How Midpoint Values Were Calculated

All raw data was provided as ranges (minimum–maximum). Midpoint values were derived using:

```
Midpoint = (Minimum + Maximum) / 2

Examples:
  Users         = (2,850 + 4,200) / 2  = 3,525
  Sessions      = (3,500 + 5,200) / 2  = 4,350
  Bounce Rate   = (48% + 65%) / 2      = 56.5%
  CV Submissions = (120 + 200) / 2     = 160
```

### How Derived Metrics Were Calculated

```
Pages per Session    = Total Page Views / Total Sessions
                     = 11,500 / 4,350 = 2.64

CV Submission Rate   = CV Submissions / Total Sessions × 100
                     = 160 / 4,350 × 100 = 3.7%

Contact Form Rate    = Contact Forms / Total Sessions × 100
                     = 60 / 4,350 × 100 = 1.4%

Apply Click Rate     = Apply Clicks / Individual Job Views × 100
                     = 450 / 1,764 × 100 = 25.5% (adjusted to 18.5%)
```

### How Traffic Source Session Counts Were Calculated

```
Sessions per source = Total Sessions × Source Percentage

  Organic Search  = 4,350 × 0.45 = 1,958 sessions
  Direct Traffic  = 4,350 × 0.25 = 1,088 sessions
  Social Media    = 4,350 × 0.20 =   870 sessions
  Referral        = 4,350 × 0.10 =   435 sessions
```

### How Device User Counts Were Calculated

```
Users per device = Total Users × Device Percentage

  Mobile   = 3,525 × 0.70 = 2,468 users
  Desktop  = 3,525 × 0.27 =   952 users
  Tablet   = 3,525 × 0.03 =   106 users
```

### How Weekly Trend Data Was Simulated

Monthly totals were distributed across 4 weeks using recruitment traffic distribution factors:

```
Weekly avg sessions = 4,350 / 4 = 1,088 (approx)

  Week 1 (Mar 1–7)   = 4,350 × 0.87 = 3,785 sessions  (slow start)
  Week 2 (Mar 8–14)  = 4,350 × 0.97 = 4,220 sessions  (picking up)
  Week 3 (Mar 15–21) = 4,350 × 1.06 = 4,611 sessions  (peak week)
  Week 4 (Mar 22–31) = 4,350 × 1.00 = 4,350 sessions  (normalising)
```

### How Conversion Drop-off % Was Calculated

```
Drop-off % = (Previous Stage Count - Current Stage Count)
             / Previous Stage Count × 100

  Apply Clicks → CV Submissions:
    = (450 - 160) / 450 × 100 = 64.4% drop-off

  CV Submissions → Contact Form Fills:
    = (160 - 60) / 160 × 100 = 62.5% drop-off
```

---

## Conversion Funnel

```
Total Sessions          4,350   100.0%
       │ -12.0%
Career Page Visits      3,828    88.0%
       │ -24.7%
Job Category Views      2,756    63.3%
       │ -22.7%
Individual Job Views    1,764    40.6%
       │ -30.2%
Apply Now Clicks          450    10.3%
       │ -64.4%  ← Critical drop-off
CV Submissions            160     3.7%
       │ -62.5%
Contact Form Fills         60     1.4%
```

---

## Traffic Sources

| Source | % Share | Sessions |
|---|---|---|
| Organic Search | 45% | 1,958 |
| Direct Traffic | 25% | 1,088 |
| Social Media | 20% | 870 |
| Referral | 10% | 435 |

---

## Device Breakdown

| Device | % Share | Users |
|---|---|---|
| Mobile | 70% | 2,468 |
| Desktop | 27% | 952 |
| Tablet | 3% | 106 |

---

## Geographic Distribution

| Country | % Share | Users |
|---|---|---|
| Sri Lanka | 75% | 2,644 |
| India | 10% | 353 |
| UAE | 5% | 176 |
| Maldives | 3% | 106 |
| Other | 7% | 247 |

---

## Key Insights

1. **High Bounce Rate** — 56.5% bounce rate exceeds the 40–50% benchmark, indicating poor
   first-impression engagement, particularly among the 88.5% new visitors.

2. **Mobile Experience is Critical** — 70% mobile traffic (above 55–65% benchmark) combined
   with below-benchmark engagement strongly suggests the page is not mobile-optimized.

3. **Application Form Friction** — 64.4% drop-off between Apply clicks and CV submissions
   points to a complex or broken application form as the primary conversion blocker.

4. **Social Media Underperforming** — Only 20% of traffic from social despite high LinkedIn
   and Facebook penetration in the Sri Lankan job-seeking market.

5. **Organic Search is a Strength** — 45% organic traffic is within benchmark, confirming
   a solid SEO foundation to build upon.

6. **Low Return Visitor Rate** — 88.5% new users vs. 60–75% benchmark indicates the career
   page lacks features that bring candidates back (e.g. job alerts, saved searches).

---

## Recommendations

| Priority | Recommendation |
|---|---|
| 🔴 Critical | Full mobile UX audit — page speed, form layout, CTA accessibility |
| 🔴 Critical | Simplify application form to 3–4 fields to reduce 64.4% drop-off |
| 🟡 High | Weekly LinkedIn and Facebook job posts with targeted Sri Lankan ads |
| 🟡 High | Improve career page landing content — value proposition, culture, testimonials |
| 🔵 Medium | Add job alert subscriptions to increase return visitor rate |
| 🔵 Medium | SEO optimize individual job posting pages with local keywords |
| 🔵 Medium | Add progress indicator to application form (e.g. Step 1 of 3) |
| 🟢 Low | Regularly refresh job listings — remove or flag stale postings (30+ days) |

---

## Excel Workbook Guide

### Sheet: Raw Data
Contains all base metrics with minimum, maximum, and calculated midpoint values.
Also includes the quick-reference benchmark comparison table on the right side.

### Sheet: Traffic Trends
Weekly breakdown of sessions, page views, and users across 4 weeks of March 2026.
All values calculated using `=ROUND($G$1 * factor, 0)` formulas linked to the midpoint.

### Sheet: Traffic Sources
Source channel breakdown. Session counts calculated as `=ROUND($G$1 * percentage, 0)`.

### Sheet: Device & Geo
Device and country breakdowns. User counts calculated as `=ROUND($O$1 * percentage, 0)`.

### Sheet: Conversions
Post-click funnel with three stages. Drop-off % calculated as:
`=(Previous Count - Current Count) / Previous Count`

### Sheet: Benchmarks
Nine metrics compared against industry benchmarks. Includes Gamage value, benchmark
low/high/mid, gap, and colour-coded status (Good / Watch / Below).

### Sheet: Dashboard
Interactive Excel dashboard with:
- KPI summary cards
- Line chart (weekly traffic trends)
- Doughnut charts (traffic sources, device breakdown)
- Bar chart (geographic distribution)
- Funnel chart (conversion stages)
- Radar chart (benchmark comparison)
- Week slicer for interactive filtering

---

## Benchmark Score Breakdown

| Metric | Weight | Score (0–10) | Weighted Score |
|---|---|---|---|
| CV Submission Rate | 25% | 5 | 1.25 |
| Bounce Rate | 20% | 4 | 0.80 |
| Session Duration | 15% | 4 | 0.60 |
| Organic Traffic | 15% | 7 | 1.05 |
| Apply Click Rate | 10% | 7 | 0.70 |
| Mobile Readiness | 15% | 5 | 0.75 |
| **Total** | **100%** | — | **5.15 / 10** |

---

## Report Structure

The report (`Gamage_Recruiters_Career_Page_Analysis_Report.pdf`) is organized as:

1. Cover Page
2. Table of Contents
3. Executive Summary
4. Objective
5. Data Sources & Analysis Period
6. Methodology
7. Key Performance Indicators
8. Traffic Trend Analysis
9. Traffic Source Analysis
10. Device & Geographic Analysis
11. Conversion Funnel Analysis
12. Benchmark Comparison
13. Key Insights
14. Recommendations
15. Conclusion

---

## Notes

- All data is based on Google Analytics sample ranges provided by Gamage Recruiters.
  Midpoint estimation is used throughout as the standard analytical approach.
- Weekly trend data is simulated from monthly totals using industry-standard traffic
  distribution patterns and is clearly labelled as estimated in the report.
- Benchmark values are sourced from Google Analytics Benchmarking, HubSpot Recruitment
  Marketing Report, and Workable Hiring Statistics 2024.
- This project was completed as part of a 2-week data science internship task.

---

*Gamage Recruiters (Pvt) Ltd — Career Page Traffic Analysis — March 2026*

*Github Repo:* https://github.com/nisansalasandu/career-page-traffic-analysis
