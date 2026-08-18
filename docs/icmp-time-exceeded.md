# ICMP Time Exceeded

## What Is It?

ICMP Time Exceeded is an ICMP message used to report that a packet could not be forwarded because its lifetime expired.

For IPv4, this commonly occurs when the packet's TTL reaches zero.

## Packet Flow

```text
Source
  |
  | IPv4 packet
  | TTL = 1
  v
Router
  |
  | TTL becomes 0
  v
Packet discarded
  |
  v
ICMP Time Exceeded
  |
  v
Source
