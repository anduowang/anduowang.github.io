---
layout: page
title : research
header : Post Archive
group: navigation
---

<!-- # research -->
My research centers around designing and building manageable (network) systems by borrowing elegant ideas from formal methods, databases, knowledge representation and reasoning, logic-based artificial intelligence, and more.

----

## enabling agile network management with logic programming

The networking community is currently undergoing an exciting transition from guess-work protocols to disciplined software: Most research efforts involve adapting formal methods, often assuming a clean-slate, stand-alone, closed system architecture, for networking, utilizing highly optimized programming and reasoning tools tailored for specific problems. To tackle challenges that do not readily fit into these techniques, this project proposes rapid prototyping by a general logic programming platform. The key observation is that most ``unconventional'' problems in networks arise from uncertain and asynchronous events, multiple stakeholders and non-expert users, and diverse requirements that are ad-hoc and ever-changing. Many of these issues mirror those extensively studied in logic programming and its many fruitful application domains. As a first step to materialize this insight and to show the feasibility of using logic programming as a rapid prototyping tool, we develop (1) a general model for networks under uncertain and asynchronous events by extending the relation structures, addressing a challenge in existing network verification; and (2) a general network transformation system by exploiting the meta-logical feature of logic programming, subsuming earlier specialized network tools.

We emphasize that while a complete and final solution to formally managed networks is beyond the scope of this paper, we hope rapid prototyping with logic programming can pave the way to accelerate the migration from guesswork to formally managed networks.

- _Structural Semantics Management: an Application of the Chase in Networking_ [MASCOTS23](https://mascots.iitis.pl/) [[paper](http://anduowang.github.io/docs/MASCOTS23-camera.pdf)] [[slides](http://anduowang.github.io/docs/MASCOTS23-slide.pdf)]
- _Faure: A Partial Approach to Network Analysis_, [HotNets 2021](https://conferences.sigcomm.org/hotnets/2021/) [[paper](http://anduowang.github.io/docs/faure.pdf)] [[slides](http://anduowang.github.io/docs/faure-hotnets.pdf)]
- _Internet Routing and Non-monotonic Reasoning_ [LPNMR 2019](https://sites.sju.edu/plw/lpnmr-2019/) [[paper](http://anduowang.github.io/docs/lpnmr19.pdf)] [[slides](http://anduowang.github.io/docs/lpnmr19_talk.pdf)]


<!-- ## deductive knowledge plane for provably correct SDN integration -->

<!-- - _Automating SDN Composition: A Database Perspective_ SOSR'17 [[extended abstract](docs/sosr17extendedabstract.pdf)] [[poster](docs/sosr17poster.pdf)] -->

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


