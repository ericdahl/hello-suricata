# hello-suricata

```
docker run -v $(pwd)/log:/var/log/suricata -v $(pwd)/suricata-etc:/etc/suricata -v $(pwd)/suricata-rules:/var/lib/suricata/rules --net host --rm -e PUID=$(id -u) -e PGID=$(id -g) --cap-add=net_admin --cap-add=net_raw --cap-add=sys_nice -it --name suricata jasonish/suricata -i wlp2s0  --af-packet=wlp2s0
```
