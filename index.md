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
    #SeeMore1 h2 {
        font-size:100px
        }
    #SeeMore2 h2 {
        font-size:100px
        }
    #SeeMore3 h2 {
        font-size:100px	
        } 
    #Akka img {
        width:25em;
        height:17em; 
        }
    #Actor img {
        width:17em;
        height:17em; 
        }
    #Pipeline img {
       width:30em;
       margin:-30px -10px 0 0; 
       height:20em;    
       }
    #AkkaSurvey img {
       width:30em;
       margin:-20px -10px 0 0; 
       height:17em;    	  		
      }
---

# Building a Distributed Crawler using Akka {#Cover}

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
- ...Founded - Jan 2012
- ...35 Person team in Chennai & Seattle
- ...Big Data Company 
- ...Some Stats
	- ...120 M Products
	- ...5 B Prices
	- ...1.5 TB data crawled daily

## Data Pipeline @ Indix {#Pipeline}

![](pictures/data-pipeline.png)


## Crawler - Requirements

- ...Distributed
- ...Polite
- ...Focused
- ...Efficient
- ...Fault Tolerant
- ...Extensible

## Our Options

-  Existing Open Source
	- ... Nutch, Heritrix
-  ... Build Your Own
	- ... Work Distribution
	- ... Cluster Management
	- ... Storage
	- ... Algorithms

## Our Choice - Akka {#Akka}

![](pictures/akka.jpg)

## Why Akka?

- Simpler
	- ... Concurrency
		- ... Program at a higher level
		- ... Don`t think 
			- ... threads, shared state
	- ... Scalability
		- ... Distributed by Design
	- ... Fault Tolerance

## **So what`s the <br>secret sauce?** {#SeeMore}

## **Actors**

## What is an Actor?

- ... Unit of computation in Akka
- ... Message passing concurrency
- ... Purely reactive
	- ... a mailbox
	- ... behavior & state
	- ... scheduled to run when sent a message
- ... Used since 1973
	- ... in Telecom with 9 nines availability

## With a Diagram {#Actor}
![](pictures/actor.jpg) 

## **Show me the code** {#SeeMore1}

## **Hello World** {#SeeMore2}

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

## **Back to the Crawler** {#SeeMore3}

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

## Lessons Learned

- ... The Actor Model
	- ... Like OO - New way of thinking
	- ... Actor composition
	- ... Message design
	- ... Externalize business logic
- ... No Blocking
	- ... Degraded performance due to starvation
	- ... Separate thread pool

## Lessons Learned (Continued)

- ... Running on EC2
	- ... Unreliable Network
	- ... Failure detector tuning

- ... Message Tracing - Debugging
	- ... Unique identifier for all messages
	- ... Splunk to visualize the flow

## Akka Survey {#AkkaSurvey}
![](pictures/akka-survey.png)

## Future Akka Roadmap

- ... Persistence
	- ... Journaling system
	- ... Replay messages on failure
- ... Cluster
	- ... Optimization (for > 200 nodes)
	- ... Re-joining Unreachable Members

## Resources

- [Akka Documentation](http://akka.io/docs)
- [LetItCrash Blog](http://www.letitcrash.com)
- Coursera Course - Reactive Programming 

## **Questions**

## **Thanks**

## Extras

- ... Map Reduce Example
- ... Cluster - Advanced 
	- ... Gossip Convergence 
	- ... Leader Election





