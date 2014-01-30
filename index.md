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

# Testing Challenges in Big Data Applications {#Cover}

*[Rajesh Muppalla](http://www.github.com/codingnirvana/) - rajesh@indix.com*

## About Me

- Developer @ `Indix`
	- ...Part of Platform Team
	- ...Working on Distributed Systems & Big Data
- ...Ex-Thoughtworks
	- ...Worked on `Go` - A continuous delivery product

## About Indix

- Product Intelligence Platform
- ...Founded - Jan 2012
- ...45 Person team in Chennai & Seattle
- ...Data Company 
- ...Some Stats
	- ...150 M Products
	- ...6 B Prices
	- ...3 TB data crawled daily

## Data Pipeline @ Indix {#Pipeline}

![](pictures/data-pipeline.png)

## **What is Big Data?** {#SeeMore1}

## 3Vs of Big Data

- <b>Volume</b>
	- ...Terabytes + 	
- ...<b>Velocity</b>
	- ...Real Time, Streaming
- ...<b>Variety</b>
	- ...Heterogeneous Sources
	- ...Unstructured Data

## Traditional Testing

- You Test For
	- ...Happy Path Scenarios
	- ...Failures
	- ...Fault Tolerance/Concurrency/Performance
- ...Practices
	- ...TDD
	- ...Continuous Integration
	- ...Mocks/Stubs

## What do you test for in Data?

- Accuracy
	- ...Capturing the real price
- ...Coverage
	- ...All products within a e-commerce store
- ...Consistency
	- ...Multiple views of the data should be in sync
- ...Completeness
	- ...All mandatory attributes of a product captured

## **Some Challenges** {#SeeMore2}

## URL Canonicalization

- Problem Statement
	- Normalize URLs
	- ...RFC 3986
- ...Unit Testing
- ...Gotchas
	- ...Sorting Query Params
	- ...Removing Double Slashes	

## Product Tagger

- Problem Statement
- ...Unit Testing
- ...Integration Testing
- ...Gotchas
	- ...Server is Down/Under Maintenance
	- ...Sample page no longer available
	- ...Testing Output Data Semantics

## Product Matching Accuracy

- Problem Statement
- ...Unit Testing
- ...Gotchas
	- ...How to Verify Accuracy at Scale?
		- ...Back to Square One

## Changing Algorithms and Data

- Problem Statement
	- ...Go back in time and re-process
- ...Gotchas
	- ...Too much volatility


## **Testing Techniques** {#SeeMore}

## Data Sampling

- Take random samples
- ...Do Manual verification
- ...Use Mechanical Turk To Scale
- ...Automate this process
- ...Guard against data bias

## Metrics, Monitoring & Alerting

- Metrics Funnel @ Indix
- ...Don''t monitor absolute counts
- ...Use Historical Stats
- ...Remove outliers
- ...Anomaly Detection & Correlation

## Tiered Data Quality

- Tier Your Data
	- ...Top E-commerce Sites
	- ...Top Categories
- ...For Top Tier Data
	- ...Larger sample validation
	- ...Lower alert thresholds

## In Summary

- Big Data Testing
	- ...is Hard
	- ...gives great dividends
	- ...build on top of Traditional
	- ...needs good data understanding
- ...Very nascent field
	- ...Ripe for thought leadership

## **Questions**

## **Thanks**

## Lambda Architecture

- ...All data is immutable
- ...Three Layers
	- ...Batch Layer
	- ...Serving Layer
	- ...Speed Layer

## Lambda Architecture

- ...Human Fault Tolerance
	- ...Embrace Human Errors
- ...Reduces Complexity
	- ...Rebuild everything on errors

