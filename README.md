# Swap-Memory-VPS-CLI

Only Copy This, 10G = 10GB Swap memory
```
sudo fallocate -l 10G /swapfile && sudo chmod 600 /swapfile && sudo mkswap /swapfile && sudo swapon /swapfile && echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab && sudo sysctl vm.swappiness=100 && echo 'vm.swappiness=100' | sudo tee -a /etc/sysctl.conf
```
