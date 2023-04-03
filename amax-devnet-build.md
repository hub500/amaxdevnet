
### 本地拉取镜像并运行devnet

```
# 拉取devnet镜像
docker pull hub500/amaxdevnet:23.1.1

# 运行devnet
docker run --name amaxdevnet:node1 -it hub500/amaxdevnet:23.1.1 /bin/bash

# 终端进入devnet
docker exec -it amaxdevnet:node1 /bin/bash
```

### devnet运行环境

```
cd /root
ls
# 输出如下
> amax  amax-unlock.sh  amax-wallet  amax.password  amnode-start.sh  default.password  eosio  tmp  workspace

1）运行amnode

bash ./amnode-start.sh

2）解锁钱包

bash ./amax-unlock.sh

3）部署amax.token AMAX

cd workspace
ls
# 输出如下
> amax.cdt  amax.contracts  amax.meta.chain  aplink.contracts  deploy-amax.token.sh  deploy-aplink.farm.sh  deploy-aplink.token.sh  hello_code

bash ./deploy-amax.token.sh

4）部署aplink.token APL

bash ./deploy-aplink.token.sh

5）部署aplink.farm

bash ./deploy-aplink.farm.sh

```
