
# Soteria : 



## Abstract

Federated Learning (FL) is a widely-used distributed learning framework that addresses privacy concerns by not directly sharing private data. However, recent studies have revealed that sharing model updates in FL can expose it to inference attacks. In this study, we highlight our key finding that leakage of data representation from gradients is the main source of privacy breaches in FL. We provide an analysis to elucidate how this leakage occurs. Based on this insight, we propose a defense mechanism called Soteria to counter model inversion attacks in FL. Our defense strategy involves learning to perturb data representation to significantly degrade the quality of reconstructed data, while maintaining FL performance. Additionally, we establish certified robustness guarantees for FL and convergence guarantees for FedAvg after implementing our defense. To assess the effectiveness of our defense, we conduct experiments on MNIST and CIFAR10 datasets to defend against the DLG and GS attacks. Our results show that, without sacrificing accuracy, our defense approach can increase the mean squared error between reconstructed and raw data by up to 160 times for both attacks, compared to baseline defense methods.


## Setup

check version :

```
conda --version

```


Start conda :

```
conda activate base

```


Deactivate conda :

```
conda deactivate

```


initiate conda :

```
conda init 


```

Required Dependencies : 
```
pip install typing_extensions
pip install typing-extensions
```

## Preconfiguration

Necessary package Files :

```
pip install matplotlib
pip install numpy
pip install Pillow
pip install torch torchvision


```



use the following command :

```
Version ---
pytorch=1.2.0
torchvision=0.4.0

```
## Usage

To initiate, execute the following command :

```
./secure_chat_app -s alice1 

```



## To Run DLG Attack (Deep Leakage from Gradient)

To execute, Change the following command in code :

```
thresh = np.percentile(deviation_f1_x_norm_sum.flatten().cpu().numpy(), 1)

```




## To Run GS Attack (Gradient Similarly Attack)

To execute the following command :

```
python reconstruct_image.py --target_id=-1 --defense=ours --pruning_rate=60 --save_image

```





To execute Model compression command :

```
python reconstruct_image.py --target_id=-1 --defense=prune --pruning_rate=60 --save_image

```















 







