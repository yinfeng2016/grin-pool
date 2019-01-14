# grin-pool - 主要面向中文用户，并更新AWS 和Azure 的快速部署方式

## 简介:
一个MimbleWimble 算法加密货币[Grin](https://github.com/mimblewimble/grin)的开源矿池实现
* Linux挖矿客户端: [mimblewimble/grin-miner](https://github.com/mimblewimble/grin-miner)
* Linux挖矿客户端: [mozkomor/GrinGoldMiner](https://github.com/mozkomor/GrinGoldMiner)

## 试用方法:
* [About](https://medium.com/@blade.doyle/mwgrinpool-com-a-grin-mining-pool-345d67cb8e98)
* [Linux CPU Mining Guide](https://medium.com/@blade.doyle/cpu-mining-on-mwgrinpool-com-how-to-efb9ed102bc9)
* [Linux GPU Mining Guide](https://medium.com/@blade.doyle/gpu-mining-on-mwgrinpool-com-how-to-72970e550a27)
* [How to get Paid](https://medium.com/@blade.doyle/configure-payments-on-mwgrinpool-com-how-to-7b84163ec467)
* [Gitter Discussion Group](https://gitter.im/grin-pool/Lobby)

### 架构:
* 无状态的微服务架构

### 主要组件:
* 矿池 Stratum 代理: Rust
* 矿池数据处理: Python3/SQLAlchemy
* 矿池 API: Python3/Flask/gunicorn
* 矿池 Web UI: NodeJS/Electron/Bootstrap/React
* 数据库: MariaDB/Redis
* 打包: Docker
* 部署: gcloud Kuberntests CLI/AWS Cloud Formation
* Orchestration: Kubernetes
* 日志收集: Splunk
* 负载均衡/Certificates: NGINX/LetsEncrypt
* 监控与告警: AWS CloudWatch

#### GCP快速部署: [ansible/roles/pool/files/README.md](ansible/roles/pool/files/README.md)

#### 自行使用Dockerfile 部署: [stratum](stratum/) 和 [grin-py](grin-py/)

### 目前状态:
* 汉化和修正初始阶段, <B>~10%</B> 完成度, 争取和原repo更新进度保持一致
* 可以在此讨论（英文） [Gitter](https://gitter.im/grin-pool/Lobby)

## 捐献:
![BTC](https://ipfs.io/ipfs/QmZQxz5LdbCuyc8LcnUiCyTLzmWmHs644mAD7A91bmTzej) <sub>17Gmy9uhE6ziB1PzYT8MMY5A4va25dy3US</sub>

![XMR](https://ipfs.io/ipfs/QmTLh1DUXhNNuB4CkaTtv3VJftXaDEY7V8hYyYGVvYzMB8) <sub>43i7q6hVrMdgY21RH7nMghSPA6s5jjGXDeEmLjL3pNFfD1XBYqf6hJpWVabfGJ5ydJKdaBjKdFvMe1kaKRj5w7Ao7q7mK8v</sub>
