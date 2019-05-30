# ansible-container

```bash
# 下载并安装ansible-container  # 依赖docker | ansible | python3.5
# 推荐使用anaconda配置虚拟环境然后安装
git clone https://github.com/ansible/ansible-container.git
cd ansible-container
pip install -e .[docker,openshift] # websock.client版本可能不对,需要卸载重装
```

