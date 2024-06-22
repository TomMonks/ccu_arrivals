## Introduction

This notebook compares two approaches to simulating a time dependent process where the number of events is Poisson distributed.  In particular we explore a scenario where the number of events per hour follows hourly Poisson distributions.  

## Methods

We investigate two methods:

1. Parameterising Poisson distributions per hour and sampling the **number of events**. We call this *method3*
2. Sampling the time between arrivals, called the inter-arrival time, from hourly Exponential distributions where interval overruns are correct by *thinning*. This is a standard text book method for simulating Non-stationary Poisson processes.

We compare methods using the **mean number of arrivals per hour**. In the case of *method* the answer is straighforward as the number of events is the rate parameter of the distributions. For latter, we must simul
