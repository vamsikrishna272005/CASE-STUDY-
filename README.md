# CASE-STUDY-

Case Study Title: Resource Allocation and Cost Optimization in an OpenStack Private Cloud

Case Overview:

ABC Cloud Services runs a private cloud using OpenStack to host virtual machines (VMs) for internal development, testing, and production workloads. Their cloud infrastructure comprises:

5 Compute Nodes, each with:
64 vCPUs
256 GB RAM
2 TB SSD storage
OpenStack Services Deployed:
Nova (Compute)
Neutron (Networking)
Cinder (Block Storage)
Glance (Image Management)
Keystone (Identity)
Horizon (Dashboard)
Heat (Orchestration)

They are considering expanding their cloud but want to first evaluate current capacity usage, VM density, and cost efficiency. The goal is to calculate whether their resource usage aligns with business needs and how to optimize it.

Case Study Questions – OpenStack Calculation in Cloud Computing

1.Resource Utilization:

Based on the current infrastructure, what is the total available compute capacity in terms of:
Total vCPUs
Total RAM
Total storage

2.Storage Allocation:

Given 10 TB of total block storage across the cloud, how many VMs can be supported if:
a) Each VM is allocated 100 GB block storage
b) Snapshot storage consumes 20% extra on average

## SOLUTIONS:

# Problem 1 — Encryption time for 2 TB

Answer (binary TB, 1 TB = 1024 GB): ≈ 104,857.6 seconds ≈ 29.13 hours (≈ 1.21 days).
Answer (decimal TB, 1 TB = 1000 GB): 100,000 seconds ≈ 27.78 hours (≈ 1.16 days).

Work (binary units):
2 TB = 2 × 1024 GB = 2048 GB.
2048 GB = 2048 × 1024 MB = 2,097,152 MB.
Time = 2,097,152 MB × 0.05 s/MB = 104,857.6 s.
104,857.6 s ÷ 3600 = 29.127666… hours ≈ 29.13 hours.

(I’ve shown both conversions because storage vendors sometimes use 1000-based TB and sometimes 1024-based TB. Use the one matching your context.)

# Problem 2 — CPU utilization efficiency

Answer: 5.5 / 8 = 0.6875 → 68.75% CPU utilization efficiency.

Work: 5.5 ÷ 8 = 0.6875 → ×100 = 68.75%.

# Problem 3 — Network throughput efficiency

Answer: 600 Mbps / 1 Gbps = 600 / 1000 = 0.60 → 60% throughput efficiency.

Work: 1 Gbps = 1000 Mbps (common networking convention). 600 ÷ 1000 = 0.6 → 60%.

# Problem 4 — Energy efficiency (same workload)

Answer: Setup A is more energy-efficient.
Work:
Setup A energy = 500 W × 2 h = 1000 Wh = 1.00 kWh.
Setup B energy = 300 W × 3.5 h = 1050 Wh = 1.05 kWh.
Setup A uses 0.05 kWh (≈5%) less than B (1.05 − 1.00 = 0.05 kWh).
Relative saving: 0.05 ÷ 1.05 ≈ 4.76% less energy than B (or 5% less relative to A’s baseline).

# Problem 5 — Max VMs efficiently hosted
Work:
Total physical cores = 16. Optimal usable cores at 75% = 16 × 0.75 = 12 cores.
Each VM uses 2 cores → max VMs = 12 ÷ 2 = 6 VMs (must be whole VMs).

Answer: 6 VMs.

Work:
Total physical cores = 16. Optimal usable cores at 75% = 16 × 0.75 = 12 cores.
Each VM uses 2 cores → max VMs = 12 ÷ 2 = 6 VMs (must be whole VMs).
