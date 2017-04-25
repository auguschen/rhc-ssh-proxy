## 利用rhc搭建socks5梯子

## 步骤
  1. 在rhc上任意建立一个项目，获取ssh访问主机的命令。
  2. 在作为代理的机器上用 ssh-keygen 生成密钥,并将公钥内容添加到rhc的设置中
  3. 在作为代理的机器上执行 ssh -N -D 0.0.0.0:1080 xxxxxxx.rhcloud.com，此处xxxxxx为第一步中获取的访问主机命令中的主机地址
  4. 在局域网中其他机器上用chrome+switchyomega做测试
