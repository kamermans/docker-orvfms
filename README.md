
Run a webserver that controls your Orvibo S20 sockets in a single command (assuming you have Docker installed):

```
docker run -d \
    --name orvfms \
    -p80:80 \
    --net=host \
    -e "IP_BROADCAST=192.168.1.255" \
    kamermans/orvfms
```

You should replace `192.168.1.255` with your broadcast IP.
