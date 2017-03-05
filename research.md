---
layout: page
title : research
header : Post Archive
group: navigation
---

<!-- # research -->
My research centers around designing and building manageable (network) systems that leverage and re-ignite interests in database and formal methods.

----

## deductive knowledge plane for SDN

- _Automating SDN Composition: A Database Perspective_ SOSR'17 [[extended abstract](docs/sosr17-poster-dependency.pdf)]

----

## database-defined networking

Software-defined networking (SDN) provides an unprecedented opportunity to exercise computing principles in simplifying networking practice. Indeed, many salient SDN features --- central control and programming interfaces --- are enabled by principles from the fields of programming language, operating systems, and distributed systems. While these principles have produced a variety of programming abstractions that drastically improve networking practice, reducing the complex distributed protocols to simpler centralized programs, there is little consensus on what are the right abstractions. Moreover, network architects today need to combine heterogeneous data sources --- network forwarding rules, data flow and QoS metrics, host intrusion alerts, and so on --- to produce a cohesive view of the network and investigate problems. To tackle the challenging network abstraction and integration problem, this project will explore the computing principle --- a principle blessed with decades of fruitful theories and commercial success, yet surprisingly under-investigated in SDN --- of database.

### *ravel*: a realization

- Ravel is now open source, <http://download.ravel-net.org>
- companion site, <http://ravel-net.org>
- github organization, <https://github.com/ravel-net>

### publications ###

- position paper [[SOSR'16]]({{site.url}}/pdf/sdndb/sosr_paper70.pdf)
- abstraction and orchestration:
  [[SOSR'15 position paper]]({{site.url}}/pdf/sdndb/demo.pdf)
  [[SOSR'15 poster]]({{site.url}}/pdf/sdndb/ravel_SOSR15_poster.pdf)
  [(keynote)]({{site.url}}/pdf/sdndb/ravel_SOSR15_poster.key)
  [[overview]]({{site.url}}/img/sdndb.jpg "overview")
- concurrency control:
  [[ONS'14 position paper]]({{site.url}}/pdf/sdndb/ons14.pdf)

----

## networking and automated reasoning

### synthesizing dynamic network controller

The few existing synthesis work on network control today are about
translating a *static snapshot* of high-level control policy into the
actual control configurations that process traffic.  However, networks
are dynamic and the policies are by nature reactive: the policies are
reacting to the constantly changing network (its configurations states
and the live traffic being processed). To accommodate such dynamic
policies, we formulate network control as a two-player temporal game:
the controller and the dynamic network become two players engaging in
a game, the goal is to find a winning strategy for the controller
player such that no matter what moves the dynamic network take, the
controller ends up in a winnning state defined by some temporal
properties.

- a preliminary paper
  [[WRiPE13]]({{site.url}}/pdf/synthesis/wripe13.pdf)
  [[slide]]({{site.url}}/pdf/synthesis/WRiPE13-final.pdf)
  [(keynote)]({{site.url}}/pdf/synthesis/WRiPE13-final.key)


