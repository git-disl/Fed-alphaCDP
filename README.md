
## description

This is the code for TPDS-2022-09-0583

## For Gradient leakage resilient federated learning

- Go to DP_code folder

- First install the conda environment with environment.yml.

- Then run create\_FLdistribution.sh to create a client distribution first (each client has two shards). The distribution file xxx_1000_clients.pkl would appear in the client folder and you may run the rest.

- This code includes both the participation-level Fed-SDP (FedSDP.py), instance-level Fed-CDP baseline (Fed\_CDP\_fixed.py) and Fed-DP dynamic(Fed\_CDP\_dynamic.py) . You may adjust the few lines within the local training for l2-max sensitivity (default fixed clipping sensitivity) and dynamic noise scale (default fixed noise scale). The privacy accounting approach is also provided for $\epsilon$ privacy spending in Fed-CDP.

## For leakage attacks

Go to gradient_leakage/ folder for gradient leakage attacks on MNIST, Fashion-MNIST, CIFAR10 and LFW (both type 1 leakage and type 2 leakage).







