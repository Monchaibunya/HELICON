# HELICON
HELICON: A Hierarchical Reinforcement Learning approach for Orchestrating Low-latency, Load-balanced Virtual Network Functions.

1 Testbed facilities

5GinFIRE testbed (https://5ginfire.eu/); University of Bristol city testbed site (https://5ginfire.eu/university-of-bristol-5g-testbed/)

Functions & Prerequisites

  1. Software: (1.1) Ubuntu 16.04; (1.2) KVM; (1.3) Openstack queen (Controller & Compute node); (1.4) OSM Mano release 4; (1.5) Open CV 3; (1.6) Panda, Python, Numpy, Scikit learn

  2. Hardware minimum requirements: (2.1) At least 4 Compute nodes with INTEL I7 4-core processor, memory 8 GB RAM, 80 GB HD; (2.2); At least 3 Raspberry Pi (Raspi) model 3B running Raspbian Jessi (2.3); At lease 3 IP-capable cameras; (2.4) All connected to the same network.
 

2 Software

Software available in https://github.com/monchai-bunya/HELICON.

This software is organised into five folders. Each folder is installed in 1. OSM node; 2. Compute node; 3. Raspberry Pi; 4. Virtual machine; and 5. User device
 

Execution:

1. OSM node: 1.1 change Hosts.txt to order IP accordingly; 1.2 execute listen.py 1 for server mode; 1.3 execute monitor.py 5 to monitor every 5 seconds.

2. Compute node: 2.1 change Hosts.txt to order IP accordingly; 2.2 execute get_vnfrs_values.py in background process; 2.3 execute get_vnfue_values.py as background process; 2.4 execute rs_list.py in background process; 2.5 execute ue_list.py as background process; 2.6 execute pm_info_update.py as background process; 2.7 execute listen.py 0 for normal mode.

3. Raspberry Pi: 3.1 execute rs_listen.py as a background process; 3.2 execute from-thetav-live-mea.py.

4. Virtual Machine: 4.1 execute vm_listen.py as a background process; 4.2 execute face-nvr-reg-mea.py.

5. User device: 5.1 execute ue_listen.py as a background process; 5.2 execute usermea.py.
