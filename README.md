# Dpdk Ndpi Installation Script
This is a bash script for installation of DPDK 21.11 and ndpi.

This is not a final script yet...!

Step 1.
Make it executeable with
chmod +x dpdk.ndpi.sh

step 2.
Run file with 
sudo ./dpdk.ndpi.sh

step 3.
You have to updaye grub file manually.

cd /etc/default
sudo nano grub

GRUB_CMDLINE_LINUX=" default_hugepagesz=2M hugepagesz=2M hugepages=1024 iommu=pt intel_iommu=on isolcpu=1 "
default_hugepagesz=1M hugepagesz=1M hugepages=1024 iommu=pt intel_iommu=on isolcpu=1

sudo update-grub
