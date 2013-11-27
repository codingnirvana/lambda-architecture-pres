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

## Components

- URL Frontier 
- URL Router
- Http Fetchers

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

- ... Distributable by Design
- ... Fault Tolerant & Self Healing
- ... Adaptive Load Balancing

## **How does Akka do it?**

## **Using Actors**

## What is an Actor?

- ... Unit of code organization in Akka
- ... Separates "Policy Decisions" from Business Logic
- ... Used since 1973
	- ... in Telecom with 9 nines availability

## More on Actors

- ... Encapsulated & decoupled 
- ... Manage their own memory & behavior
- ... Communicate via non-blocking async messages
- ... Hot Deploy - Change behavior at runtime

## Models for concurrency

- ... Shared state concurrency
- ... Message passing concurrency

## **Show me the code**

## 1. Create

<html><head>
<meta http-equiv="content-type" content="text/html; charset=ISO-8859-1">
<title>a.scala</title>
<link rel="stylesheet" type="text/css" href="highlight.css">
</head>
<body class="hl">
<pre class="hl"><span class="hl kwa">case class</span> <span class="hl kwd">Greeting</span><span class="hl opt">(</span>who<span class="hl opt">:</span> String<span class="hl opt">)</span>

<span class="hl kwa">case</span> GreetingActor <span class="hl kwa">extends</span> Actor with ActorLogging <span class="hl opt">{</span>
  <span class="hl kwa">def</span> receive <span class="hl opt">= {</span>
    <span class="hl kwa">case</span> <span class="hl kwd">Greeting</span><span class="hl opt">(</span>who<span class="hl opt">) =&gt;</span> log<span class="hl opt">.</span><span class="hl kwd">info</span><span class="hl opt">(</span><span class="hl str">&quot;Hello {}&quot;</span><span class="hl opt">,</span> who<span class="hl opt">)</span>     
  <span class="hl opt">}</span>
<span class="hl opt">}</span>

</pre>
</body>
</html>

 Code Samples

    <!DOCTYPE html>
    <html lang="en">
    <mark><head></mark> <mark class="comment"><!--Comment--></mark>
        <title>Shower</title>
        <meta charset="<mark class="important">UTF-8</mark>">
        <link rel="stylesheet" href="screen.css">
    <mark></head></mark>

## Even Tables

|  Locavore      | Umami       | Helvetica | Vegan     |
+----------------|-------------|-----------|-----------+
|* Fingerstache *| Kale        | Chips     | Keytar    |
|* Sriracha     *| Gluten-free | Ennui     | Keffiyeh  |
|* Thundercats  *| Jean        | Shorts    | Biodiesel |
|* Terry        *| Richardson  | Swag      | Blog      |

It’s good to have information organized.

## Pictures
{:.cover #Picture}

![](pictures/picture.jpg)
<!-- photo by John Carey, fiftyfootshadows.net -->

## **You can even shout this way**

## Inner Navigation

1. Lets you reveal list items one by one
2. …To keep some key points
3. …In secret from audience
4. …But it will work only once
5. …Nobody wants to see the same joke twice

## ![](http://shwr.me/pictures/logo.svg) [See more on GitHub](https://github.com/shower/shower/)
{:.shout #SeeMore}
