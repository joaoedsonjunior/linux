# Desativando a inteface gráfica do Linux

1 - Buscar a configuração padrão
```sh
systemctl get-default 
```

2 - Setar a configuração desejada
```sh
systemctl set-default multi-user.target
```

### OBS.: Para desfazer é só setar a interface gráfica novamente
