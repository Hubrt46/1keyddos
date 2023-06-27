适合绝大部分VPS使用 

DD成功：oci  aws  az  rn  vultr  layerstack

重装

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/robram9572/1KEYDD/master/InstallNET.sh') -d 11 -v 64 -p 123456 -port 22

bash <(wget --no-check-certificate -qO- 'https://raw.githubusercontent.com/robram9572/1KEYDD/master/InstallNET.sh') -u 20.04 -v 64 -p 123456 -port 22


系统参数

-d 10  【7、8、9、10，11】Debian

-u 20.04  【14.04、16.04、18.04、20.04】Ubuntu

密码参数，可以改成别的


-p 12345

端口参数

port 22


安装完成后VPS会重启安装，等待10分钟左右，尝试重新连接

用户名为root

密码是你设置的

成功连接后输入下面的更新组件和BBR命令，完善基础系统环境


更新组件

apt update -y && apt install -y curl && apt install -y socat && apt install wget -y

BBR

wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh
