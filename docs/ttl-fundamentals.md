# TTL Fundamentals

## What Is TTL?

Time To Live (TTL) is an IPv4 field used to limit the lifetime of a packet as it is forwarded through a network.

Despite its name, TTL is normally treated as a hop-count mechanism in modern IP forwarding.

## What Happens at Each Router?

When a router forwards an IPv4 packet, it decreases the TTL by at least one.

Example:

```text
Initial TTL: 4

Host
  |
  v
Router A   TTL = 3
  |
  v
Router B   TTL = 2
  |
  v
Router C   TTL = 1
  |
  v
Next Router TTL = 0
