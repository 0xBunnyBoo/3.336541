# Hugepages allocation
sudo sysctl -w vm.nr_hugepages=2048
# UDP buffer sizes
sudo sysctl -w net.core.rmem_max=62500000
sudo sysctl -w net.core.rmem_default=62500000
sudo sysctl -w net.core.wmem_max=62500000
sudo sysctl -w net.core.wmem_default=62500000
# TCP buffer sizes
sudo sysctl -w net.ipv4.tcp_rmem='4096 62500000 62500000'
sudo sysctl -w net.ipv4.tcp_wmem='4096 62500000 62500000'
