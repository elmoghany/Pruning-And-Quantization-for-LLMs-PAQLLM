# Pruning and Quantization for LLMs (PAQLLM)

In this notebook, I'll be showing the results before and after results for each pruning & quantization

## 1) Intro
LLMs consume
1) High latency during inference
2) High Memory
3) Large Storage
4) High Power Consumption
5) Time Consuming Training Time

Due to the above reasons, we need pruning and quantization to fix those issues

## 2) References
1) Used llama 3.0 8B as the LLM
2) Used gaming laptop of GTX 1060i 6GB & 32GB of RAM
3) Used M2 NVMe (Samsung PM961 NVMe MZVLW512HMJP) hard disk

## 3) Quantization
Quantization is the process of converting a continuous signal into a discrete signal
![picture](images/quantization-overview.jpg)

Technique used:
* 4 bit quantization for the weights only
  
Pros for using quantization:
1) less memory usage
2) faster inference and fine-tuning time
3) less sotrage

### Quantization Storage
65% less storage is needed after quantization
![picture](images/quantization-storage-usage.png)

### Quantization Memory
82.5% less memory is needed after quantization
![picture](images/quantization-memory-usage.png)

### Quantization Inference time
98.81% less time is needed during inference
![picture](images/quantization-inference-time.png)

## 4) Pruning
