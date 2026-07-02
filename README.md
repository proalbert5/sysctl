| Parameter | 1GB / 1core | 2GB / 1core | 4GB / 2core | 8GB / 4core | 16GB / 8core |
|---|---|---|---|---|---|
| net.core.rmem_max / wmem_max | 8388608 | 16777216 | 33554432 | 67108864 | 134217728 |
| net.core.netdev_max_backlog | 8192 | 16384 | 32768 | 65536 | 131072 |
| net.core.somaxconn | 4096 | 8192 | 16384 | 32768 | 65535 |
| net.ipv4.tcp_max_syn_backlog | 4096 | 8192 | 16384 | 32768 | 65535 |
| net.netfilter.nf_conntrack_max * | 32768 | 65536 | 131072 | 262144 | 524288 |
| net.netfilter.nf_conntrack_buckets | 8192 | 16384 | 32768 | 65536 | 131072 |
| vm.min_free_kbytes | 16384 | 32768 | 65536 | 131072 | 262144 |
| fs.file-max / nr_open | 50000 | 100000 | 200000 | 400000 | 800000 |
| kernel.pid_max | 32768 | 65536 | 131072 | 131072 | 131072 |

The base config values are set for the **1GB / 1core** profile. Adjust these values according to your own server's RAM and core count.

Replace the **sysctl.conf** file with the **previous sysctl.conf file** in the **/etc** directory.
To save the **sysctl settings**, run this **command**:
‍‍‍‍‍‍``` sysctl -p ```
