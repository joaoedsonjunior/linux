# Configurar interface de rede Linux

1 - Acesse o arquivo de acordo com o nome da Interface de Rede 
```sh
vi /etc/sysconfig/network-scripts/ifcfg-IFACE
```

2 - Edite as informações de IP, GW, MASK,DNS
```sh
TYPE="Ethernet"
PROXY_METHOD="none"
BROWSER_ONLY="no"
BOOTPROTO="none"
DEFROUTE="yes"
IPV4_FAILURE_FATAL="no"
IPV6INIT="yes"
IPV6_AUTOCONF="yes"
IPV6_DEFROUTE="yes"
IPV6_FAILURE_FATAL="no"
IPV6_ADDR_GEN_MODE="stable-privacy"
IPADDR0="192.168.1.50"
PREFIX0="24"
GATEWAY0="192.168.1.1"
DNS1="192.168.1.1"
DNS2="8.8.8.8"
NAME="enp0s3"
UUID="ef0b12a8-6b0d-40b2-8fee-aa96345d9d8d"
DEVICE="enp0s3"
ONBOOT="yes"
```

3 - Reiniciar o NetworkManager
```sh
systemctl restart NetworkManager
```
