# SixGPT Miner  中文教程
This is the official SixGPT miner.

# About

SixGPT is a decentralized synthetic data generation platform built on the Vana network. We empower users by giving them ownership of their data and enabling them to earn from it.

The SixGPT Miner is a software package which allows users to contribute data they generate for wikipedia question-answer based tasks to the network for rewards.
In the future, we will support other tasks such as chatbot conversations, image captioning, etc.

## Prerequisites
先安装docker

(1) install docker on your machine. (https://docs.docker.com/engine/install/)

存入0.1 VANA

(2) Fund your wallet with at least 0.1 $VANA


去网站用钱包链接一下 并且绑定google网盘


(3) Login with this wallet on sixgpt.xyz

git拉取


## Run the miner:
Clone the repository:
```
git clone https://github.com/sixgpt/miner.git
cd miner
```

CPU跑 不建议 基本上跑不动

直接运行这里跑GPU

先修改.env文件中你的密钥


### Run the miner with more advanced options
```
chmod +x run_sixgpt.sh
./run_sixgpt.sh
```

## Notes
- You must have logged into sixgpt.xyz with your wallet before running the miner
- Make sure the wallet associated with your vana private key has enough $VANA balance on the desired network (at least 0.1)

## Additional Notes on Handling GPU Detection
- [ollama github](https://github.com/ollama/ollama)
- [ollama docker](https://hub.docker.com/r/ollama/ollama)
- NVIDIA GPUs: Ensure that you have the NVIDIA Container Toolkit installed to enable GPU support in Docker. You can follow the installation guide [NVIDIA Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html).
- AMD GPUs: For AMD, ensure that the ROCm (Radeon Open Compute) stack is installed and configured correctly. More details can be found on the official ROCm documentation [ROCm (Radeon Open Compute) stack](https://rocm.docs.amd.com/en/latest/).
