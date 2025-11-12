# Distri Place - Project plan

## Overview

A distributed collaborative pixel canvas where multiple users can simultaneously place colored pixels, inspired by Reddit's r/place. The system runs on 3 independent server nodes that maintain a shared canvas state through distributed consensus and synchronization protocols.

## System Architecture

Three Python backend nodes communicate peer-to-peer using TCP sockets. Each node maintains a full replica of the 100x100 pixel canvas in memory. A React frontend allows users to place pixels by sending HTTP requests to any available node.

## Core Functionality

Users connect through a web interface to view the canvas and place colored pixels at specific coordinates. When a pixel is placed, the receiving node broadcasts the update to its peers, ensuring all nodes converge to the same canvas state despite concurrent modifications and network delays.

## Distributed Systems Features

- Shared State: Each node stores a complete canvas replica with pixel data (position, color, timestamp, origin node).
- Consistency & Synchronization: Vector clocks track causality of updates across nodes. Conflicts from concurrent writes to the same pixel are resolved using last-write-wins with node-id tie-breaking.
- Consensus: Nodes use leader election (Bully algorithm) where the leader coordinates batch commits of pixel updates through two-phase commit protocol, ensuring all nodes agree on the order of operations.
- Fault Tolerance: Heartbeat mechanism detects node failures. When a node crashes, surviving nodes continue operating with the remaining replicas. Recovered nodes synchronize state from active peers.
- Scalability: For large-scale deployment (100+ nodes), the canvas would be partitioned using consistent hashing, with each shard replicated across multiple nodes for fault tolerance.

## Technology Stack

- Backend: Python 3 (sockets, Flask)
- Frontend: React
- Communication: JSON over TCP
- Deployment: University svm servers (3 VMs)
