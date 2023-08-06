**Service level indicator** is a quantitative measure of some aspect of the level of service being provided. Examples include throughput, latency, and error rate.

![[Pasted image 20230614235435.png]]

```
Fraction of 200 vs 500 HTTP responses from API endpoint measured per day

Time to last byte GET requests measured every 10 seconds aggregated per minute
```

Here are a couple more examples for an imaginary online bank. The SLI defines what you want to measure, like the fraction of 200 vs 500 HTTP responses from an API endpoint or the time to last byte GET requests measured every 10 seconds aggregated per minute.

The SLO defines the target you want to achieve, like 99.95% availability or that 95% of requests will complete in under 300 ms.

![[Pasted image 20230614235450.png]]

```
Fraction of 200 vs 500 HTTP responses from API endpoint measured per month

Time to last byte GET requests measured every 15 seconds aggregated per 5 minutes

Upload errors measured as a percentage of bulk uploads per day by custom metric

Fraction of 200 vs 500 HTTP responses from API endpoint measured per month

Time to last byte GET requests measured every
60 seconds aggregated per 10 minutes

```


Notice that the SLI describes what we are going to measure and how: for example, the “Fraction of 200 vs 500 HTTP responses from API endpoint measured per month.” This example is a way of measuring availability

![[Pasted image 20230615000037.png]]

```
Fraction of 200 vs 500 HTTP responses from API endpoint measured per month

Time to last byte GET requests measured every 15 seconds aggregated per 5 minutes

Upload errors measured as a percentage of bulk uploads per day by custom metric

Fraction of 200 vs 500 HTTP responses from API endpoint measured per month

Time to last byte GET requests measured every 60 seconds aggregated per 10 minutes

```