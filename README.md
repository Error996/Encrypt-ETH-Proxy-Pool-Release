# Encrypt-ETH-Proxy-Pool-Release
Encrypt-ETH-Proxy/Pool-Release

![1](https://user-images.githubusercontent.com/12880110/145681404-0239eff0-e88f-47c9-8824-ae0bc4e96f99.png)

## 说明 
1.miner不联网,仅client联网，采用随机算法链接Forward，Forward不做任何解密动作，压缩处理后转发Server，server解密还原拼接后提交Pool
2.miner和server之间可以无法联通，server要求最低2g内存20g硬盘，Forward不做要求，256内存可跑
3.大幅优化流量，所有重复内容在server做缓存，client只接受job和提交work
4.加密采用WebSocket Over Tls,可走cdn

## 进度
已完成client和forward,server完成90%还差细节bug修复
