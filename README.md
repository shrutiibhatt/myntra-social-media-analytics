# Myntra Social Media Analytics for Strategic Branding

A social media analytics project for Myntra, India's fashion e-commerce platform, completed as part of the Internshala Digital Marketing course. It analyses 300 posts and 50 weeks of platform data across Facebook, Instagram, Twitter (X) and YouTube to answer which content, platforms and campaigns work best.

**Author:** Shruti Bhatt · **Course:** Internshala Digital Marketing

## What's in this repo

| File | What it is |
|---|---|
| `Task-1_DataCleaning.xlsx` | Cleaned posts, split hashtags, weekly engagement summary, campaign data |
| `Task-2_EngagementAnalysis.xlsx` | Engagement rate per platform, top 10 posts, pivots |
| `Task-3_Platform_Analysis.xlsx` | Platform comparison and follower growth |
| `Task-4_Hashtag_Content_strategy.xlsx` | Hashtag and content type performance |
| `Task-5_Campaign_Effectiveness.xlsx` | Campaign totals, uplift and ROI |
| `Task-6_Follower_retention___Loyalty.xlsx` | Weekly follower trends and ad spend correlation |
| `Myntra_Social_Media_Dashboard.xlsx` | Formula-driven dashboard with Platform and Campaign dropdown filters |
| `Myntra_Dashboard.html` | Interactive web dashboard with a platform filter (open in any browser) |

## Key findings (from the dashboard data)

- **Instagram leads.** It has the highest average post engagement rate (19.3%) and the most net new followers (48,004).
- **Facebook gets the most ad spend but returns the least.** It converts spend into 25.8 net followers per 1,000 spent, against 41.2 on Instagram.
- **Instagram Reels (26.0%) and Stories (24.6%)** are the strongest platform/format combinations. Text posts are the weakest format overall (11.8%).
- **Ad spend barely explains follower growth.** The weekly correlation with net follower adds is -0.06 across all platforms.
- **Hashtag choice is a minor lever.** The gap between the best (#StyleWithMyntra, 15.6%) and worst (#FashionDeals, 13.7%) hashtag is about 2 percentage points.
- **StyleRevolution** has the best average engagement rate (15.8%) and added the most followers per 1,000 budget during its dates. EndOfSeasonSale generated the most total engagement.

## Method and caveats

- **Engagement rate** = (Likes + Shares + Comments) / Impressions. The dashboards show both the average of per-post rates and the pooled rate (total engagement / total impressions).
- **Net followers** = New followers minus unfollows. The supplied `Total_Followers` column jumps erratically from week to week, so the dashboards do not use it. The follower figures in Tasks 5 and 6 were derived from `Total_Followers`, so they will not match the dashboard's net-follower numbers.
- **Campaign tags and dates don't line up.** Posts carry a campaign tag, but post dates span the whole year regardless of campaign dates. Post-based and date-window campaign figures measure different things.
- **Outliers.** A few posts with very low impressions have engagement rates above 100%. They are kept in the data and the pooled rate is shown alongside the average.
- **Small samples.** Each content type × platform combination has about 12 posts, so those comparisons are directional, not statistically tested.
- **Ad spend currency** is not stated in the source data.
- **No duplicates were found.** All 300 post IDs are unique.

## Data

The dataset comes from the course project materials and appears to be synthetic. Findings describe this dataset and should not be read as statements about Myntra's real performance.

## Tools

Analysis (Tasks 1-6) built in Microsoft Excel. The two dashboard files were generated with Claude (Anthropic) from the cleaned Task 1 data.
