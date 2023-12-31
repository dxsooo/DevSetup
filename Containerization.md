# 容器化（Containerization）

## 镜像管理
### Docker

官方渠道下载，Mac或者windows直接下载对应的desktop，https://docs.docker.com/desktop/

Linux无需下载desktop，参考 https://docs.docker.com/engine/install/ 下载即可

### Podman

官方渠道下载，Mac或者windows直接下载对应的desktop，https://podman-desktop.io/downloads ，然后参考 https://podman-desktop.io/docs/Installation 进行配置

Linux无需下载desktop，参考 https://podman.io/docs/installation#installing-on-linux 下载即可

#### MacOS 下代理配置

由于机制原因，MacOS中实际上是运行了一个podman machine，由其进行相关动作如push、pull、run，所以如果是要使用代理，需要将代理配置到该 machine 中。操作方式参考 [https://github.com/containers/podman/issues/14087](https://github.com/containers/podman/issues/14087#issuecomment-1116097347) 和 [https://github.com/containers/podman/issues/11941](https://github.com/containers/podman/issues/11941#issuecomment-997279722)，修改 machine 内的设置并重启 machine 。

## 服务编排

### Docker compose

安装 Docker/Docker desktop 会包含，如果使用 podman 即需要单独安装，可以直接使用 podman desktop 中的安装指引

### k8s 相关工具

参考 https://kubernetes.io/docs/tasks/tools/ ，一般安装 kubectl 就够了
