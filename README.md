 Distributed Storage Lab

A SeaweedFS cluster on Docker Compose that I break on purpose to study replication, fault tolerance and performance.

Status: work in progress (October 2026).

## Goals

- Run a small but realistic cluster: 1 master, 1 filer, 1 S3 gateway, 4 volume servers on 2 racks.
- Replicate every volume across racks (replication 010) and verify the placement.
- Inject failures (node, rack, disk, master, network partition, slow node) and observe recovery.
- Measure throughput and latency, monitor with Prometheus and Grafana.
- Write a runbook entry for each failure scenario.

## Architecture

To be added with the Compose topology.

## Requirements

- Linux or WSL2 with a kernel that provides sch_netem (network fault injection)
- Docker with Compose v2
- 6 GB of RAM for the WSL2 VM

## Quick start

To be added.

## Network fault injection

To be confirmed by scripts/netem-check.sh.

## Results

To be added.

## License

MIT, see LICENSE.
