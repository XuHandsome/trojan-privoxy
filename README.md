# trojan-privoxy

trojan client with privoxy for http proxy

## How to use

```bash
docker run -dit --restart always\
    --name trojan-proxy \
    -e REMOTE_ADDR="server host" \
    -e REMOTE_PORT="server port" \
    -e PASSWORD="your password" \
    -e VERIFY=false \
    -p trojan_port:1086 \
    -p privoxy_port:1087 \
    handsomexu/trojan-privoxy
```
