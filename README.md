# TTL & Routing Loops

> A visual and practical guide to Time To Live (TTL), routing loops, and ICMP Time Exceeded.

## Overview

Packets can become trapped in a routing loop when network devices repeatedly forward them between incorrect or inconsistent routes.

TTL provides a mechanism that limits how long an IP packet can remain in the network.

## Documentation

- [TTL Fundamentals](docs/ttl-fundamentals.md)
- [Routing Loops](docs/routing-loops.md)
- [ICMP Time Exceeded](docs/icmp-time-exceeded.md)

## Example

- [Traceroute and TTL](examples/traceroute.md)

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

## The Core Idea

```text
Routing Loop
     ↓
Packet keeps circulating
     ↓
TTL decreases at each hop
     ↓
TTL reaches 0
     ↓
Packet discarded
     ↓
ICMP Time Exceeded
