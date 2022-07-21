on ubuntu 24.04 gcp vm:

1. if nvidia-smi can' connect to driver, driver is not loaded:



> sudo apt update

> sudo apt remove '^nvidia'
 
> sudo apt-get purge 'nvidia*'
 
> sudo apt autoremove

> sudo reboot

then run

> sudo apt install nvidia-driver-470 libnvidia-gl-470 libnvidia-compute-470 libnvidia-decode-470 libnvidia-encode-470 libnvidia-ifr1-470 libnvidia-fbc1-470

>sudo reboot


helper links:

https://askubuntu.com/questions/1370843/how-to-properly-install-nvidia-470-drivers-on-ubuntu-20-04 [working]

https://dev.to/simonpham/how-to-fix-ubuntu-nvidia-driver-is-not-loaded-2ipp

https://unix.stackexchange.com/questions/38560/gpu-usage-monitoring-cuda

https://forums.developer.nvidia.com/t/error-nvidia-driver-470-is-not-loaded-ubuntu-20-04/193133

https://askubuntu.com/questions/1370843/how-to-properly-install-nvidia-470-drivers-on-ubuntu-20-04

-------------------------------------------------------------
#to monitor:

> nvitop -
