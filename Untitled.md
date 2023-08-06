
Let’s consider an example of a service and SLI, SLO, and SLAs for the service. The service is an HTTP endpoint accessed using a HTTP GET.

The SLI is the end-to-end latency of successful HTTP responses, that is HTTP 200s. These are averaged over one minute. The SLO has been agreed that the latency of 99% of the responses must be less than or equal to two hundred milliseconds.

![[Pasted image 20230615000355.png]]

Service level indicator is a quantitative measure of some aspect of the level of service being provided. Examples include throughput, latency, and error rate.

Understanding what users want from a service will help inform the selection of indicators. The indicators must be measurable. For example, fast response time is not measurable, whereas HTTP GET requests that respond within 400ms aggregated per minute is clearly measurable. Similarly, highly available is not measurable, but percentage of successful requests over all requests aggregated per minute is measurable.

Not only must indicators be measurable, but the way they are aggregated needs careful consideration. For example, consider requests per second to a service. How is the value calculated: by measurements obtained once per second or by averaging requests over a minute? The once-per-second measurement may hide high request rates that occur in bursts of a few seconds.

For example, consider a service that receives 1000 requests per second on even numbered seconds and 0 requests on odd numbered seconds. The average requests per second could be reported over a minute as 500. However, the reality is that the load at times is twice as large as the average. Similar averages can mask user experience when used for metrics like latency. It can mask the requests that take a lot
longer to respond than the average.

It is better to use percentiles for such metrics where a high order percentile, such as 99%, shows worst case values, while the 50th percentile will indicate a typical case.