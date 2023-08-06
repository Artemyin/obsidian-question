# SLOs must be achievable and relevant

| SLI                                                                               | SLO                                                                   |     |     |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------- | 
| HTTP POST photo uploads complete within 100ms aggregated per minute               | (-) 99% If our users are using mobile phones, maybe this is overkill. |     |     |
|                                                                                   | (v) 80% This might be good enough.                                    |     |     |
| Available as measured with an uptime check every 10 seconds aggregated per minute | (-) 100% Sounds good, but not practical.                              |     |     |
|                                                                                   | (-) 99.999% Possible, but maybe too expensive.                        |     |     |
|                                                                                   | (v) 99% Maybe good enough and easier and more cost-effective.         |     |     |

# Tips for determining SLOs

The goal isn’t to make SLOs as high as possible; the goal is to make them as low as you can get away with while still making users happy. That’s why it’s important to understand your users.

The higher you set the SLO, the higher the cost in compute resources (redundancy) and operations effort (people time).

Applications should not significantly outperform their SLOs, because users come to expect the level of reliability you usually give them.

A poor SLO will result in a significant amount of wasted work if it is too ambitious or a poor product if it is to relaxed.

# An SLA is a business contract between the provider and the customer
The SLA stipulates that:
-  A penalty will apply to the provider if the service does not maintain certain availability and/or performance thresholds.
-  If the SLA is broken, the customer will receive compensation from the provider.

Not all services have an SLA, but all services should have an SLO.
Your SLO thresholds should be stricter than your SLA.

# Example: SLI, SLO, and SLA

![[Pasted image 20230610160905.png]]

SLI: The latency of successful HTTP responses (HTTP-200).
SLO: The latency of 99% of the responses must be s 200 ms.
SLA: The user is compensated if 99th percentile latency exceeds 300 ms.

![[Pasted image 20230610161739.png]]
