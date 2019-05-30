# ansible-container
下载并安装ansible-container  # 依赖docker | ansible | python3.5

推荐使用anaconda配置虚拟环境然后安装

```bash
git clone https://github.com/ansible/ansible-container.git
cd ansible-container
pip install -e .[docker,openshift] # websock.client版本可能不对,需要卸载重装
ansibe-container init
ansible-container build 下载基础镜像
```
进入对应目录修改container.yml配置,然后制作镜像并运行

```
cd jenkins
ansible-container build # 由于需要去国外下载基础镜像第一次很慢,也可以跳过此步骤,从dockerhub上下载
ansible-container run
```

