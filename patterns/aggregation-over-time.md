    {%hyde

    title: "n by.--> 

Aggregation over time."
    type: pattern
    excerpt: "Instead of reporting immediately and continuously about resource consumption,
a consumer of a resource keeps track of its consumption locally (using a trusted device) and periodically reports on its total consumption (over the last reporting period) to the provider of the resource. This prevents the provider to learn details about when exactly the consumer used the resource, while still informing the provider about the total amount of resources used by each individual consumer. Using *aggregation over time* protects the privacy of the consumer, while still allowing to charge consumers for their resource use (for example)."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.--> 

Aggregation over time.

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->

##Summary
<!-- One short paragraph summarising the pattern.-->

Instead of reporting immediately and continuously about resource consumption,
a consumer of a resource keeps track of its consumption locally (using a trusted device) and periodically reports on its total consumption (over the last reporting period) to the provider of the resource. This prevents the provider to learn details about when exactly the consumer used the resource, while still informing the provider about the total amount of resources used by each individual consumer. Using *aggregation over time* protects the privacy of the consumer, while still allowing to charge consumers for their resource use (for example).

##Context
<!-- The situations in which the pattern may apply.-->

Consider a provider that offers remote usage of a resource to a (potentially large) group of consumers. The resource is provided in a 'broadcast/multicast' way, with the distinguishing feature that the consumer can consume the resource without the provider knowing when exactly the resource is consumed, or by whom. In some cases the provider may not even be aware that the resource is consumed at all.

Examples of this type of resource provisioning are, for example, utility (electricity, gas, water) networks or media broadcasting networks.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Given this context, the resource provider needs to learn (a function of) the total amount of resources used by each individual consumer. This may be necessary, for example, to charge consumers for their resource consumption, or to measure the spread of popularity of a resource over all consumers.

However, real time information about the consumption of a resource by a consumer may be quite privacy invasive. Precise information about how much energy is consumed at exactly what time can reveal one's religion (Muslims rising early for morning prayer) or medical traits (men with prostate issues going to the bathroom several times at night), for example.

Unfortunately, usage of the resource may be valued differently depending on when exactly the resource is used. This overall 'value' still needs to be communicated accurately to the provider.

Moreover, consumers may not be trusted to report on resource consumption fairly, especially if they are billed for the consumption.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The *aggregate over time* pattern places a component (called the *aggregator*) at the consumer that monitors consumption of the resource in real time by sampling it over very short fixed time intervals. The aggregator contains an accumulator to aggregate these measurements. In fact, the aggregator combines the current contents of the accumulator with a fixed function of the current resource usage, and stores the result back in the accumulator. More formally,
let $f$ and $g$ be two functions, and let $A$ be the current value of the accumulator. If the $i$-th input sample at real time $t_i$ equals $x_i$ then the new value of the accumulator becomes $g(A,f(x_i,t_i))$.

The resource provider may receive information about the current contents of the accumulator in two ways:

- either the aggregator sends the contents of the accumulator to the provider at fixed, predetermined, time slots, or
- the provider can send a request to the aggregator to return the current contents of the accumulator. The aggregator denies this request if it comes within a predetermined time after the previous granted request.

In both cases, after the contents of the accumulator have been transmitted to the provider, the contents of the accumulator are reset to a default value (and accumulation starts from scratch).

The functions $f$ (to compute the value to be combined with the accumulator based on the current input sample and the time it was sampled) and the function $g$ (to combine the result with the current accumulator value) are specified by the provider. This also holds for the default value of the accumulator. These functions may be fixed and hardwired into the aggregator, or the aggregator may have an additional input over which it receives updates to these functions. 


###Structure
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->

The aggregator may be a separate device (e.g a smart meter) or a software component running within the IT infrastructure of the consumer (an app running on the consumer smart phone, for example). In either case, the aggregator must be a trusted device that reliably computes the associated function, which cannot be influenced by the consumer (except with extraordinary effort through *tamper resistance*, or with high risk of detection through *tamper evidence*). 


The aggregator is placed between the resource and the consumer, so that all consumption of the resource is detected by the aggregator. It should be unfeasible to bypass this (see above). The aggregator is connected to the provider over a (long distance) communication link. This link may be unidirectional from aggregator to provider in the case of the aggregator periodically sends accumulated data to the provider. (This increases privacy as in this setup there is no way for the provider to reach the aggregator in its own accord.)

If dynamic updates to the aggregation functions are required, the aggregator has a separate input receiving updates from the provider over a (long distance) communication link.

<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->

##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

The benefits of applying this pattern are the following.

- Detailed resource usage information is withheld from the provider, protecting the privacy of the consumer.
- Information about the total resource consumption per consumer is obtained by the provider, at a granularity determined by the length of the time interval over which resource consumption is aggregated.
- This granularity is enforced by the aggregator and cannot be influenced by the provider (although it is set by the manufacturer of the aggregator).

The disadvantages are as follows.

- The producer does not obtain real time information about resource consumption.
- Certain, detailed, aggregation functions may leak rather precise information
about real time resource consumption.

###Constraints
<!-- limitations as a consequence of applying the pattern.-->

There are few constraints when applying the *aggregate over time* pattern.

- Given the last disadvantage of the previous section, the aggregation functions need to be simple; not all applications allow for this.
- There are no clear rules how to set the time interval over which resource consumption is aggregated. The larger the better, from a privacy perspective, but there may be cases where large values decrease the value proposition for the producer.

##Examples
<!--Motivational example to see how the pattern is applied.-->

The *aggregate over time* design pattern can be applied to

- measure usage of broadcasted information or media; here the resource consumer is the radio or TV owner and the resource provider is the broadcasting station.


###Known Uses
<!-- Pointers to various applications of the pattern.-->

The *aggregate over time* design pattern has been applied to
- measure electricity consumption by a household using a so-called smart meter; here the resource consumer is the household and the resource provider is the distribution system operator (DSO);

<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.--> 

###Related Patterns
<!-- Supporting and conflicting patterns-->

- Aggregate over location

<!--###[Sources]-->
<!-- References to the original source of the pattern.-->

##General Comments
<!-- Separate discussion on the pattern.-->

This pattern considers a resource provider as an entity separate from the resource owner or producer. They may be the same entity in mane cases (but are not, for example, in smart grid setting).

We note that the pattern equally applies to settings where a large group of anonymous providers collectively supply a resource that a single 'consumer' capitalises, exploits or values. In other words, 'consumption' of the resource 
as described in the pattern above actually creates value, which may incentivise consumers to over-report their 'consumption'.

(The name of the pattern may be too broad, perhaps referring to a class of patterns of which this one is a particular instance, related to resource consumption measurement)

<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->



