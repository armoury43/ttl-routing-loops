# TTL & Routing Loops

> A visual and practical guide to Time To Live (TTL), routing loops, and ICMP Time Exceeded.

## Overview

Packets can become trapped in a routing loop when network devices repeatedly forward them between incorrect or inconsistent routes.

TTL provides a mechanism that limits how long an IP packet can remain in the network.

## How It Works

```text
Packet
  ↓
Router A
  ↓
Router B
  ↓
Router C
  ↓
TTL reaches 0
  ↓
Packet discarded
  ↓
ICMP Time Exceeded
