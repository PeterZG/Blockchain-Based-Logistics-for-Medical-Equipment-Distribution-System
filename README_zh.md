# 基于区块链的医疗设备分发物流系统


## 简介

在Dr. Arash Shaghaghi的委托下，我们开发了一套基于区块链的医疗设备分发系统，旨在解决传统医疗供应链在透明度和效率方面的不足，特别是在健康危机期间对关键物资分发的挑战。我们使用Hyperledger Fabric确保数据的不可篡改性，并提供实时追踪、库存管理、供需调整和防伪验证等功能，保障信息的透明性和各方的高效协作。该系统显著提升了医疗物资供应链的透明度和效率，为应对健康危机中的物资供应提供了坚实的技术支持。

## 技术框架

- **前端**: React  
- **后端**: Spring Boot  
- **区块链**: Hyperledger Fabric 2.54  

## 快速开始

### 环境需求

- Node.js 和 npm  
- Java JDK 17  
- Maven  
- Docker 和 Docker Compose  
- Git  

### 安装步骤

1. 克隆代码仓库：

```sh
git clone https://github.com/PeterZG/Blockchain-Based-Logistics-for-Medical-Equipment-Distribution-System.git
```

2. 安装前端依赖：

```sh
cd frontend
npm install
```

3. 安装后端依赖：

```sh
cd backend
mvn install
```

4. 配置 Hyperledger Fabric 网络：

```sh
cd Blockchain
sudo bash generate.sh
sudo bash deploy.sh
```

`generate.sh` 用于生成通道文件。  
`deploy.sh` 用于创建通道、加入通道、更新锚节点及部署链码的操作。

> （本项目中的二进制文件基于 linux-amd64。如果您使用 macOS，需要下载正确版本的文件，并替换 Blockchain 目录中的 `/bin`、`/builders` 和 `/config` 文件。[下载地址](https://github.com/hyperledger/fabric/releases)）

有关更详细的部署问题，请参考文档 `BlockchainDeploy.md`。如果仍无法解决问题，请通过以下联系方式联系我们：  
[weihouzeng@gmail.com] 或 [849997616@qq.com]。

### 运行应用程序

1. 启动后端服务：

```sh
cd backend
mvn spring-boot:run
```

2. 启动前端应用：

```sh
cd frontend
npm start
```

建议本地运行，否则可能会有响应延迟。

3. 启动区块链网络：

如果您已成功部署链码，则区块链网络现在应该已启动。如需下次启动，只需运行以下命令：

```sh
docker-compose up -d
```

在 Blockchain 目录下执行。

React 应用运行在 [http://localhost:3000](http://localhost:3000)，Spring Boot 应用运行在 [http://localhost:8080](http://localhost:8080)。

## 联系支持

如在部署或命令中遇到问题，请通过以下邮箱联系我们：  
[weihouzeng@gmail.com] 或 [849997616@qq.com]。

## 说明

这是一个私人项目，目前开发阶段已完成。如果您有任何疑问或希望了解更多，请随时通过上述邮箱联系我们。

## 作者

- **马广原** - *主要后端与区块链* - [Guangyuan](https://github.com/Noplusultra)  
- **邓榆川** - *主要后端与前端，次区块链* - [Yuchuan](https://github.com/dyc54)  
- **罗昊天** - *主要前端* - [Haotian](https://github.com/Haotian14)  
- **曾维厚** - *主要后端和区块链，次前端* - [Weihou](https://github.com/PeterZG)  

## 许可协议

当前项目未采用任何特定的开源许可协议。

## 致谢

- 致谢任何代码贡献者  
- 项目灵感来源  
- 等等
