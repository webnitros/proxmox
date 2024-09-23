### Установка

```shell
bash -c "$(wget -qLO - https://raw.githubusercontent.com/webnitros/proxmox/refs/heads/master/ubuntu2404-vm.sh)"
```

### Проброс порта до машины

```shell
iptables -t nat -A PREROUTING -i vmbr0 -p tcp --dport 20109 -j DNAT --to-destination 10.10.10.109:22
```


```shell
sudo apt-get update && apt-get upgrade -y
apt install curl -y
curl -sSL https://get.docker.com/ | sh
```



