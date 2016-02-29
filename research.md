---
layout: page
title : research
header : Post Archive
group: navigation
---

<!-- # research -->

My research centers around designing and building manageable (network)
systems that leverage and re-ignite interests in formal reasoning
(database theories, deductive formal methods, inductive machine
learning etc).

----

## networking and database

### an SDN control plane without packet processing

Today's control planes are centered around packet processing that
limits SDN's power. Control applications must describe their policies
in terms of indirect packet-processing actions, and topology
abstractions as the only mean to raise switch-level actions are
restricted. Orchestrating such applications requires explicit
coordination of the packet-processing actions that jointly drive a
network, resulting in a complex master program or an additional
orchestration layer.

In search of a control plane that exploits SDN's full potential, we
take a fresh look and design a database-centered solution, *a
packet-processing independent control platform*. We take the entire
SDN network under the hood of a relational active database: the
forwarding rules become the stored (base) tables, from which the
control plane database derives for each application a virtual table
(SQL view) for application-network interaction. This base-view two
layer relational structure brings about an open and direct
abstraction, reducing policies to integrity constraints on the
views. More importantly, it enables loosely-coupled orchestration that
addresses more application interactions. Individual applications can
independently control the network via constraint-preserving and
constraint-restoring actions over their views, of which the resulting
network updates are controlled on the base by a data-sharing protocol.

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


