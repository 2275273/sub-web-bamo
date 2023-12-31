
依次运行下面四行代码，若是 Debian/Ubuntu 系统，请自行替换下面前两行命令中的 yum 为 apt

yum update -y

curl -fsSL https://deb.nodesource.com/setup_16.x | 
sudo -E bash -
sudo apt-get install -y nodejs

npm install -g cnpm --registry=https://registry.npm.taobao.org

cnpm install -g yarn


检测版本号

node -v
v16.19.0

yarn --version
1.22.21


拉取 sub-web 程序，并进入 sub-web 文件夹

git clone https://github.com/CareyWang/sub-web.git

cd sub-web-bamo


在项目目录中安装构建依赖项，构建的过程稍微有点长

yarn install

使用 webpack 运行 Web 客户端以进行本地开发。

yarn serve

断开或者退出当前环境 CTRL+C，打包网页

yarn build
