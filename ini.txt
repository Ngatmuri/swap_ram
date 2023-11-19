free -m
sudo dd if=/dev/zero of=/mnt/swap.0 bs=1024 count=1048576
sudo mkswap /mnt/swap.0
sudo su
echo "/mnt/swap.0 swap swap defaults 0 0" >> /etc/fstab
swapon /mnt/swap.0
sudo swapon -s
