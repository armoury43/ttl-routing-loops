# Routing Loops

## What Is a Routing Loop?

A routing loop occurs when routing decisions cause packets to repeatedly travel through the same set of routers instead of progressing toward their destination.

## Simple Example

Consider three routers:

```text
        +---------+
        | Router A |
        +---------+
             |
             v
        +---------+
        | Router B |
        +---------+
             |
             v
        +---------+
        | Router C |
        +---------+
             |
             +----------+
                        |
                        v
                   Router A
