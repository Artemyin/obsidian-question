# Quantitative requirements are things that are measurable

Given the constraints:
- Time
- Finance
- People

What can be achieved:
- How many users are there?
- How much data is there?
- What are the rewards and risks?
- Which features can launched?

# Key performance indicators (KPIs) are metrics that can be used to measure success

In business, common KPIs include:
- Return on investment (ROI)
- Earnings before interest and taxes (EBIT)
- Employee turnover
- Customer churn

In software, common KPIs include:
- Page views
- User registrations
- Clickthroughs
- Checkouts

The goal is outcome or result you want to achieve. 
The KPI is a metric that indicates whether you are on track to achieve the goal.

**Goal**: Increase turnover for an online store
**KPI**: The percentage of conversions on the website

>**As an example,** a goal may be to increase turnover for an online store, and an associated KPI may be the percentage of conversions on the website.

# For KPIs to be effective, they must be SMART

## Specific
"User Friendly" is not as specific as "Section 508 Accessible."

## Measurable
You have to find an objective way to test whether you're meeting your KPls.

## Achievable
"100% Availability" might sound good, but it's not really possible.

## Relevant
Does it really matter to the user? Will it help achieve application goals?

## Time-bound
99% available: Per year? Per month? Per day? If we don't know, how can we measure?

# Quantitative requirements can be expressed in terms of SLIs, SLOs, and SLAs

## Indicators
An SLI is a measurable attribute of a service. A KPI.
E.g., Availability

- [-] Fast response time
- [x] HTTP GET requests respond within 400 ms aggregated per minute
- [-] Highly available
- [x] Percentage of successful requests over all requests aggregated per minute

>[!info] Not only must indicators be measurable, but the way they are aggregated needs careful consideration. 
>For example, consider requests per second to a service. How is the value calculated? 
>By measurements obtained once per second, or by averaging requests over a minute?
>The once per second measurement may hide high request rates that occur in bursts of a few seconds. 
>For example, consider a service that receives 1,000 requests per second on even-numbered seconds and zero requests on odd-numbered seconds. 
>The average request per second could be reported over a minute as 500. However, the reality is that the load at times is twice as large as the average.

## Objectives
The SLO is the number or the goal you want to achieve for a given SLI for a given duration.
Do you want 95%, 99%, or 99.99% availability?

## Agreements
An SLA is a binding contract providing the customer compensation if the service doesn't meet specific expectations.
The SLA is a more restrictive version of the SLO.


