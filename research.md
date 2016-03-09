---
layout: page
title : research
header : Post Archive
group: navigation
---

<!-- # research -->
My research centers around designing and building manageable (network) systems that leverage and re-ignite interests in formal reasoning (database theories, deductive formal methods, inductive machine learning etc).

----

## networking and database

### Ravel: a database-defined network


- [[SOSR'16 short paper]]({{site.url}}/pdf/sdndb/sosr_paper70.pdf)
- [[overview]]({{site.url}}/img/sdndb.jpg "overview")
- abstraction and orchestration:
  [[SOSR'15 position paper]]({{site.url}}/pdf/sdndb/demo.pdf)
  [[SOSR'15 poster]]({{site.url}}/pdf/sdndb/ravel_SOSR15_poster.pdf)
  [(keynote)]({{site.url}}/pdf/sdndb/ravel_SOSR15_poster.key)
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


