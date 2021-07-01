### Liberando porta no IPtables:
```sh
iptables -I INPUT -p tcp --dport 8989 -j ACCEPT
```
### Verificando se a porta está liberada (regra):
```sh
iptables -nL | grep 8989
```
### Liberando porta FirewallD:
```sh
firewall-cmd --permanent --zone=public --add-port=8989/tcp
```
### Recarregando o firewall para aplicar as alterações:
```sh
firewall-cmd --reload
```

### Verificando se a porta está liberada (regra):
```sh
firewall-cmd --zone=public --query-port=8989/tcp
```
