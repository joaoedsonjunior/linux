# Desativando a inteface gráfica do Linux

1 - Buscar a configuração padrão
```sh
systemctl get-default 
```

2 - Setar a configuração desejada
```sh
systemctl set-default multi-user.target
```

3 - Fazer reboot para aplicar as configurações
```sh
systemctl reboot
```

### OBS.: Para desfazer é só setar a interface gráfica novamente
