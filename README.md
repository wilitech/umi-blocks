# umi-blocks
业务区块整合

## 新建区块

1. 安装 [umi](https://umijs.org/zh/guide/getting-started.html#%E7%8E%AF%E5%A2%83%E5%87%86%E5%A4%87)
2. 在本项目根目录创建区块文件夹
3. 进入区块文件夹，执行命令`yarn create umi`
    * 模板类型选择 `block`
    * github 仓库地址填写 `wilitech/umi-blocks`
    * 选择不启用 TS
    * 目前 umi 版本还需要手动在 package.json 添加[版本兼容配置项](https://github.com/umijs/umi/pull/2367)
      ```
      "blockConfig": {
        "specVersion": "0.1"
      }
      ```

![](./screenshots/1.jpg)


## FAQ
windows下，如果用umi创建antd-pro项目出现了问题，请确保在终端可以执行create-umi，如果出现了报错，则需要添加变量到path中
具体步骤：
1. $ yarn global bin (得到路径值)
2. 控制面板-系统和安全-系统-高级系统设置，选择环境变量
3. 在用户变量和系统变量下找到Path，选择编辑，都添加上你在终端得到的路径值（如：C:\Program Files\nodejs\node\global\bin
