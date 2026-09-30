个人备忘（）

```bash
# 端口
PROXY_PORT=7890

# 自动获取 Windows 主机 IP
WIN_HOST_IP=$(ip route show default | awk '/default/ {print $3; exit}')
PROXY_URL="http://${WIN_HOST_IP}:${PROXY_PORT}"

# 覆盖小写 + 大写代理变量
export http_proxy="$PROXY_URL"
export HTTP_PROXY="$PROXY_URL"
export https_proxy="$PROXY_URL"
export HTTPS_PROXY="$PROXY_URL"
export ftp_proxy="$PROXY_URL"
export FTP_PROXY="$PROXY_URL"
export all_proxy="$PROXY_URL"
export ALL_PROXY="$PROXY_URL"

# 不走代理的地址
export no_proxy='localhost,127.0.0.1,::1,0.0.0.0,10.0.0.0/8,172.16.0.0/12,192.168.0.0/16,.local'
export NO_PROXY="$no_proxy"

env | grep -i proxy
```