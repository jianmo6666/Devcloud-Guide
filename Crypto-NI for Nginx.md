点击图示图标，等待弹出下面的横框并点击
![图1](https://github.com/jianmo6666/Devcloud-Guide/blob/main/images/3194a101fa94c82d4370335fbf20931.png?raw=true)
屏幕下方弹出交互Shell，按以下命令进行测试
![图2](https://github.com/jianmo6666/Devcloud-Guide/blob/main/images/3194a101fa94c82d4370335fbf20931.png?raw=true)
启用Crypto新指令情况下
# ps aux | grep nginx
# wrk -t 18 -c 1000 -d 20s https://127.0.0.1:443/

未启用Crypto新指令情况下
# nginx -s stop
# nginx -c /usr/local/share/nginx/conf/nginx-https.conf
#wrk -t 18 -c 1000 -d 20s https://127.0.0.1:443 

预期结果：
对比两个测试wrk产生的”Requests/sec”结果，启用Crypto的情况下，对比未启用应有若干倍的提升。

