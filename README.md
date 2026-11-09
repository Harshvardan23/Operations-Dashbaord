# Operations Dashboard

## Why this exists

**Purpose** — We have a PAN-India team with clients more than 700 and headcount more than 27,000, and in every region we have a Regional Head. Under the Regional Head we have a team that fills the data, which the Regional Head, MIS, People Operations Head and leadership team have to view to understand how the business is going — which is the reason why this dashboard exists.

The reason we built it is because the data was getting too scattered to be viewed at one place and to understand and take decisions out of it — that is why we created this dashboard, to check the business health.

The team under the Regional Head fills the data — their MIS.

Everyone who is involved in the operations, from the people filling the data to the top management, they all read the dashboard, so we have to make it in a way that it satisfies all the needs.

The dashboard is good in understanding the operations, which is why it gets read weekly on Monday, and the numbers are accurate — all the operations decisions happen through this report only.

## Data Pipeline

Data Pipeline — from the field to the dashboard

```
WMS
 │   Regional teams enter headcount data every week
 ▼
PostgreSQL
 │   System of record — the live database
 ▼
pgAdmin 4 — VIEW
 │   Joins the WMS tables into one output shape
 ▼
Looker Studio
 │   Live connection straight to the view
 ▼
Auto-refresh — every Monday, 9:00 AM
```

## Dashboard Preview

![Operations Dashboard](DASHBOARD%20PREVIEW/GITHUB_Weekly_Operations_Dashboard_page-0001.jpg)
