# Network Topologies

## What is it?

Network topology is the way devices are connected to each other in a network. It describes the layout of the system, not just the devices themselves.

A topology can be physical or logical.

- Physical topology describes the actual cables and placement of devices.
- Logical topology describes how data flows from one device to another even if the wiring is hidden.

## Why do we need it?

The structure of a network affects:

- how fast it can communicate
- how reliable it is
- how easily it can be expanded
- how much troubleshooting is needed

A network with the wrong layout may be slow, fragile, or difficult to manage.

## Common network topologies

### Bus topology

All devices share a single communication line.

This used to be common in older local networks, but it is rarely used now.

### Star topology

All devices connect to a central switch or hub.

This is the most common topology in homes and businesses.

### Ring topology

Devices connect in a circle, so each device passes data to the next.

This design is less common in modern Ethernet networks but still appears in some systems.

### Mesh topology

Every device has a path to every other device, or at least many possible paths.

Mesh networks are common in large or highly redundant systems.

## Real-world example

Most home networks use a star topology:

```text
[ Laptop ]
    |
[ Switch ] --- [ Router ] --- Internet
    |
[ Printer ]
```

The switch sits in the center, and devices connect to it. This makes it simple to add or remove devices.

## Why star networks are so common

Star networks are easy to manage, easy to troubleshoot, and easy to expand. If one device fails, it usually does not affect the rest of the network.

## Common beginner mistakes

- Confusing topology with the devices themselves
- Assuming a network is always wired the same way it is logically arranged
- Thinking all networks use the same layout

## Practice exercise

1. Draw a simple home network using a star topology.
2. Label the router, switch, laptop, and printer.
3. Explain why one failed device does not necessarily break the whole network.

## Quick quiz

1. What does topology describe?
2. Which topology is most common in homes and small offices?
3. What is the difference between physical and logical topology?
4. Why is a star topology easier to troubleshoot than a bus topology?

## Summary

Network topology is about how a network is laid out. Different layouts have different strengths and weaknesses. For beginners, understanding topology helps explain why some networks are easier to expand, troubleshoot, and manage than others.
