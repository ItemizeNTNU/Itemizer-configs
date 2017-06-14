# Itemizer-configs
The file _paradise-vm.sh_ is now configured to be able to spawn 4 different VMs. Each with 8 CPU cores, 1 GPU, 16GB RAM, one 40BG disk and one 120GB disk, and a bridged network adapter.

## Startup
VM 1 can be started like this:
```
sudo ./paradise-vm.sh 1
```

## Run time
To tap into the session for VM 2 or any other, use screen.
```
sudo screen -r vm-2
```

## Troubleshooting
Using only DVI-cables may pose some problems. We used DVI for the two upper cards, and display/hdmi for the two lower ones.  
USB devices change bus and device ID when disconnected and reconnected. This is important to know when mapping USB devices to   

A lot of the inspiration has been gathered from:
https://github.com/gmasse/gpu-pci-passthrough/tree/develop
