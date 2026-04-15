依赖安装方式
在项目根目录执行：

corepack enable
yarn install
如果你本机还没准备好 Yarn 4，先执行（任选其一）：

corepack prepare yarn@4.9.2 --activate
# 或
yarn set version 4.9.2
说明：.yarnrc.yml 指向 .yarn/releases/yarn-4.9.2.cjs，如果本地没有这个文件，上面两步可以补齐环境。

运行方式（开发）
yarn start
等价于：

ng s -o
补充：

serve 默认配置是 development（angular.json 中已设置）
代理文件是 proxy.conf.js，当前 API 代理是注释状态，默认不转发后端请求
常用命令
构建：yarn build
Lint：yarn lint
单测：yarn test
覆盖率：yarn test-coverage