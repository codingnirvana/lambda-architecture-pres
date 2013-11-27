---

layout: ribbon

style: |

    #Cover h2 {
        margin:30px 0 0;
        color:#FFF;
        text-align:center;
        font-size:70px;
        }
    #Cover p {
        margin:250px 0 0;
        text-align:center;
        color:#FFF;
        font-style:italic;
        font-size:30px;
        }
        #Cover p a {
            color:#FFF;
            }
    #Picture h2 {
        color:#FFF;
        }
    #SeeMore h2 {
        font-size:100px
        }
    #SeeMore img {
        width:0.72em;
        height:0.72em;
        }
---

# Building a Distributed Crawler using Scala and Akka {#Cover}

*[Rajesh Muppalla](http://www.github.com/codingnirvana/) - rajesh@indix.com*

![](pictures/cover.jpg)
<!-- photo by John Carey, fiftyfootshadows.net -->

## About Me

- Developer @ `Indix`
	- ...Part of Platform Team
	- ...Working on Distributed Systems & Big Data
- ...Ex-Thoughtworks
	- ...Worked on `Go` - A continuous delivery product

## About Indix

- Product Intelligence Platform
- ...Founded Early 2012
- ...35 Person team in Chennai & Seattle
- ...Some Stats
	- ...120 M Products
	- ...5 B Prices
	- ...1 TB data crawled daily

## Data Pipeline @ Indix

- TODO - Add a nice diagram

## Crawler - Requirements

-  Focused
- ...Polite
- ...Distributed
- ...Efficient
- ...Fault Tolerant
- ...Pluggable

## Our Options

-  Existing Open Source
	- ... Nutch, Heritrix
-  ... Build Your Own
	- ... Work Distribution
	- ... Cluster Management
	- ... Storage
	- ... Algorithms

## Our Choice - Akka

![](pictures/akka.jpg)
{:.cover }

## Why Akka?

- ...Simpler
	- ... Concurrency
	- ... Scalability
	- ... Fault Tolerance

## Program at a Higher Level

- ... You need not think about
	- ... shared state, state visibility
	- ... threads, locks etc.
- ... Gives you
	- ... high CPU Utilization
	- ... low latency

## Scale Up vs Scale Out

- ... Distributed by Design
- ... Fault Tolerant & Self Healing
- ... Adaptive Load Balancing

## **How does Akka do it?**

## **Using Actors**

## What is an Actor?

- ... Unit of computation in Akka
- ... Purely reactive
	- ... a mailbox
	- ... behavior & state
	- ... scheduled to run when sent a message
- ... Used since 1973
	- ... in Telecom with 9 nines availability

## Models for concurrency

- ... Shared state concurrency
- ... Message passing concurrency

## **Show me the code**

## **Hello World**

## Parallelism

- ... Scale by creating multiple actor instances
- ... Order is not guaranteed

## Supervision

- ... Manage other Actor''s failure
- ... Termination messages sent to Supervisor
- ... Separates processing & error handling
- ... Multiple Strategies
	- ... One-For-One
	- ... All-For-One

## Clustering

- ... Released in Akka 2.2
- ... Gossip based Cluster Membership
- ... Failure Detector
- ... Cluster DeathWatch
- ... Adaptive Load Balancing

## ** Back to the Crawler **

## Key Components

- ... URL Frontiers 
	- ... Site Queues
	- ... Priority Queues
- ... URL Router ( 1 per frontier)
- ... Http Fetchers	
- ... URL Scheduler

## Patterns Used

- ... Supervision Strategy
- ... Work Pulling
- ... Throttling
- ... Periodic Message Scheduling
- ... Finite State Machine
	- ... Hot swapping Actor Behavior

## Lessons Learned

- ... The Actor Model
	- ... Like OO - New way of thinking
	- ... Actor Composition
	- ... Message Design
	- ... Externalize Business Logic
- ... EC2 Tuning
	- ... Unreliable Network
	- ... Failure detector tuning
- ... Message Tracing
	- ... Unique identifier for all messages
	- ... Splunk to visualize the flow

## Challenges

- ... 




