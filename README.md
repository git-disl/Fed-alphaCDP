
## description

This is the code for Securing Distributed SGD against Gradient Leakage Threats, which is published at IEEE Transactions on Parallel and Distributed Systems in 2023. 

## For Gradient leakage resilient federated learning

- Go to DP_code folder

- First install the conda environment with environment.yml.

- Then run create\_FLdistribution.sh to create a client distribution first (each client has two shards). The distribution file xxx_1000_clients.pkl would appear in the client folder and you may run the rest.

- This code includes both the participation-level Fed-SDP (FedSDP.py), instance-level Fed-CDP baseline (Fed\_CDP\_fixed.py) and Fed-DP dynamic(Fed\_CDP\_dynamic.py) . You may adjust the few lines within the local training for l2-max sensitivity (default fixed clipping sensitivity) and dynamic noise scale (default fixed noise scale). The privacy accounting approach is also provided for $\epsilon$ privacy spending in Fed-CDP.

## For leakage attacks

Go to gradient_leakage/ folder for gradient leakage attacks on MNIST, Fashion-MNIST, CIFAR10 and LFW (both type 1 leakage and type 2 leakage).


If you are interested in our research, please cite:

```
@inproceedings{wei2020framework,
  title={A framework for evaluating client privacy leakages in federated learning},
  author={Wei, Wenqi and Liu, Ling and Loper, Margaret and Chow, Ka-Ho and Gursoy, Mehmet Emre and Truex, Stacey and Wu, Yanzhao},
  booktitle={European Symposium on Research in Computer Security},
  year={2020},
 publisher={Springer}
}

@inproceedings{wei2021gradient,
  title={Gradient-Leakage Resilient Federated Learning},
  author={Wei, Wenqi and Liu, Ling and Wu, Yanzhao and Su, Gong and Iyengar, Arun},
booktitle={International Conference on Distributed Computing Systems},
  year={2021},
 publisher={IEEE}}


@ARTICLE{wei2022gradient,
  author={Wei, Wenqi and Liu, Ling},
  journal={IEEE Transactions on Information Forensics and Security}, 
  title={Gradient Leakage Attack Resilient Deep Learning}, 
  year={2022},
  volume={17},
  number={},
  pages={303-316},
  doi={10.1109/TIFS.2021.3139777}}


@ARTICLE{wei2023securing,
  author={Wei, Wenqi and Liu, Ling and Zhou, Jingya and Chow, Ka-Ho and Wu, Yanzhao},
  journal={IEEE Transactions on Parallel and Distributed Systems}, 
  title={Securing Distributed SGD Against Gradient Leakage Threats}, 
  year={2023},
  volume={34},
  number={7},
  pages={2040-2054},
  doi={10.1109/TPDS.2023.3273490}}


}
```





