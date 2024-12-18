
# Blockchain-Based-Logistics-for-Medical-Equipment-Distribution-System

## Introduction

Under the commission of Dr. Arash Shaghaghi, we developed a blockchain-based medical equipment distribution system aimed at addressing the shortcomings of traditional healthcare supply chains in terms of transparency and efficiency, particularly the challenges of distributing critical supplies during health crises. We utilized Hyperledger Fabric to ensure the immutability of data and incorporated features such as real-time tracking, inventory management, dynamic supply-demand adjustment, and anti-counterfeiting verification to ensure transparency of information and efficient collaboration among stakeholders. This system significantly enhanced the transparency and efficiency of the medical supply chain, providing robust technical support for the supply of medical resources during health crises.

## Technical Framework

- **Frontend**: React
- **Backend**: Spring Boot
- **Blockchain**: Hyperledger Fabric 2.54

## Getting Started

### Prerequisites

- Node.js and npm
- Java JDK 17
- Maven
- Docker and Docker Compose
- Git

### Installation

1. Clone the repository:

```sh
git clone https://github.com/PeterZG/Blockchain-Based-Logistics-for-Medical-Equipment-Distribution-System.git
```

2. Install the frontend dependencies:

```sh
cd frontend
npm install
```

3. Install the backend dependencies:

```sh
cd backend
mvn install
```

4. Set up the Hyperledger Fabric network:

```sh
cd Blockchain
sudo bash generate.sh
sudo bash deploy.sh
```

generate.sh is used to generate channel-artifacts

deploy.sh is used to create channel, join channel, update the anchor peer and a series of chain code deployment operations.

(the binary file in our project is based on linux-amd64. If you use the mac os, you need to downloads the correct version file and change the /bin /builders /config file in the Blockchain https://github.com/hyperledger/fabric/releases)

For more specific deployment issues,you can see the md file "BlockchainDeploy.md".If you still can not resolve the problem, please contact us;[weihouzeng@gmail.com][849997616@qq.com].

### Running the Application

1. Start the backend server:

```sh
cd backend
mvn spring-boot:run
```

2. Run the frontend application:

```sh
cd frontend
npm start
```

Run it locally, otherwise there will be slow responses or lags.

3. Run the Blockchain network

If you have successfully deployed the chaincode then the blockchain network should now be open, if you want to open it next time just use

```sh
docker-compose up -d
```

in the Blockchain directory.


The React application should now be running on [http://localhost:3000](http://localhost:3000), and the Spring Boot application on [http://localhost:8080](http://localhost:8080).

## Contact Us for Support

If you encounter any deployment or command issues, please email us for consultation[weihouzeng@gmail.com][849997616@qq.com].


## Overview

This is a private project and we have completed the development phase. However, if you have questions or would like to learn more about the project, please feel free to contact us via the email addresses provided[weihouzeng@gmail.com][849997616@qq.com].


## Authors

- **Guangyuan Ma** - *Primary Backend and Blockchain* - [Guangyuan](https://github.com/Noplusultra)
- **Yuchuan Deng** - *Primary Backend and Frontend, Secondary Blockchain* - [Yuchuan](https://github.com/dyc54)
- **Haotian Luo** - *Primary Frontend* - [Haotian](https://github.com/Haotian14)
- **Weihou Zeng** - *Primary Backend and Blockchain, Secondary Frontend* - [Weihou](https://github.com/PeterZG)


## License

Currently, this project is not under any specific open source license.


## Acknowledgments

- Hat tip to anyone whose code was used
- Inspiration
- etc

---

**Note**: Replace `[repository-url]` with the actual URL of your repository.
