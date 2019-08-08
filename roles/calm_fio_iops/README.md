# calm_fio_iops
Role to enabled benchmarking using the CALM technique (Controlled
Ambient Load Mixing). This sets up a steady background IO load
using the rate_iops option of fio, and helps understand the
impact of noisy neighbors on the primary benchmark.

This creates a data set, so requires storage space. Ensure that
calm_fio_iops_dir points to a directory where the fio jobs can
create their files, and ensure that there is suffient storage
space.

