# dfs_bench
Performance benchmarking for distributed storage.

This project is in its early days. The aim is to create simple ansible playbooks to help with performance analysis of distributed storage solutions, like ceph and gluster.

## Basic Flow

There are two types of ansible roles at this time:

1. A single performance benchmark. An example is fio_1client_seqio, which does an fio sequential write and read test.

1. A helper role. An example is collect_sysstat, which is used to get output of monitoring utilities for the duration of the benchmark run, and is useful in analyzing results from the benchmark.

A typical playbook, like perform_benchrun.yml, proceeds as follows:

1. Setup a directory for all output for the run.
1. Start monitoring on all relevant hosts
1. Run a benchmark
1. Collect output of monitoring utilities, and information on hosts (e.g. /proc/cpuinfo) involved in the benchmark.

## Work in Progress 

Add more benchmarks, as well as add and improve helper roles.

