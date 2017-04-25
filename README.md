## 利用rhc搭建socks5梯子

## 步骤
  1. 在rhc上任意建立一个项目，我选择了之前建立好的wordpress项目，获取了ssh访问主机的命令。![获取ssh访问主机命令](https://note.augus.tech/api/file/getImage?fileId=58e743163c9b99000c000010)
  2. 在作为代理的机器上用 ssh-keygen 生成密钥,并将公钥内容添加到rhc的设置中![rhc添加key](https://note.augus.tech/api/file/getImage?fileId=58e743163c9b99000c00000f)
  3. 在作为代理的机器上执行 ssh -N -D 0.0.0.0:1080 xxxxxxx.rhcloud.com
  4. 在局域网中其他机器上用chrome+switchyomega做测试
