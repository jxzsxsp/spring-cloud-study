
- spring.cloud.config.label         指明远程仓库的分支
- spring.cloud.config.profile       指明环境配置文件
  - dev开发环境
  - test测试环境
  - pro正式环境

#### http请求地址和资源文件映射如下:
- /{application}/{profile}[/{label}]
- [http://localhost:6100/user/dev](http://localhost:6100/user/dev)
- [/{label}]/{application}-{profile}.yml
- [http://localhost:6100/user-dev.yml](http://localhost:6100/user-dev.yml)
- [/{label}]/{application}-{profile}.properties
- [http://localhost:6100/user-dev.properties](http://localhost:6100/user-dev.properties)
- /{property}/{profile}
- [http://localhost:6100/foo/dev](http://localhost:6100/foo/dev)