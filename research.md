---
layout: page
title : research
header : Post Archive
group: navigation
---

<!-- # research -->
My research centers around designing and building manageable (network) systems that leverage and re-ignite interests in database and formal methods.

----

## database-defined networking
<br>

SDN's logically centralized control provides an insertion point for programming the network.  While it is generally agreed that higher-level abstractions are needed to make that programming easy, there is little consensus on what are the ``right'' abstractions.  Indeed, as SDN moves beyond its initial specialized deployments to broader use cases, it is likely that network control applications will require diverse abstractions that evolve over time.

To this end, we champion a perspective that SDN control fundamentally revolves around data representation. We discard any application-specific structure that might be outgrown by new demands. Instead, we adopt a plain data representation of the entire network --- network topology, forwarding, and control applications --- and seek a universal data language that allows application programmers to transform the primitive representation into any high-level representations presented to applications or network operators. Driven by this insight, we present a system, *Ravel*, that implements an entire SDN network control infrastructure within a standard SQL database.  In Ravel, network abstractions take the form of user-defined *SQL views* expressed by SQL queries that can be added on the fly. A key challenge in realizing this approach is to *orchestrate* multiple simultaneous abstractions that collectively affect the same underlying data.  To achieve this, Ravel enhances the database with novel data integration mechanisms that merge the multiple views into a coherent forwarding behavior. Moreover, Ravel is exposed to applications through the one simple, familiar and highly interoperable SQL interface. While this is an ambitious long-term goal, our prototype built on the PostgreSQL database exhibits promising performance even for large scale networks.

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


