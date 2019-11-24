# Pembuatan Topologi

![topologi](https://user-images.githubusercontent.com/42793740/69493243-01dd5600-0edf-11ea-8513-377f9fe3d1e2.PNG)

# Setting IP (nano /etc/network/interfaces)

![ip venusaur](https://user-images.githubusercontent.com/42793740/69493523-41597180-0ee2-11ea-8a38-3826825fb33f.PNG)

![ip arceus](https://user-images.githubusercontent.com/42793740/69493524-41597180-0ee2-11ea-990b-eeb39703102d.PNG)

![ip articuno](https://user-images.githubusercontent.com/42793740/69493525-41f20800-0ee2-11ea-95fe-6258fb23629c.PNG)

![ip blastoise](https://user-images.githubusercontent.com/42793740/69493526-41f20800-0ee2-11ea-92f1-a6538cba0a26.PNG)

![ip mew](https://user-images.githubusercontent.com/42793740/69493527-428a9e80-0ee2-11ea-9d10-0facc072f150.PNG)

![ip mewtwo](https://user-images.githubusercontent.com/42793740/69493528-428a9e80-0ee2-11ea-91fe-f2d1796d0c33.PNG)

![ip moltres](https://user-images.githubusercontent.com/42793740/69493529-428a9e80-0ee2-11ea-8207-fb2cc9813ecc.PNG)

![ip pikachu](https://user-images.githubusercontent.com/42793740/69493530-43233500-0ee2-11ea-909c-109a33def53e.PNG)

![ip psyduck](https://user-images.githubusercontent.com/42793740/69493532-43bbcb80-0ee2-11ea-8cd1-67feaf5e8abf.PNG)

![ip snorlax](https://user-images.githubusercontent.com/42793740/69493533-43bbcb80-0ee2-11ea-969e-8a5f0d24c427.PNG)

# Routing

![routing arceus](https://user-images.githubusercontent.com/42793740/69493372-ccd20300-0ee0-11ea-964b-115a687dfa95.PNG)

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.9
```

![routing blastoise](https://user-images.githubusercontent.com/42793740/69493373-cd6a9980-0ee0-11ea-9577-43e2c423ebfe.PNG)

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.1
```

![routing pikachu](https://user-images.githubusercontent.com/42793740/69493374-cd6a9980-0ee0-11ea-8f6b-e7dc68cb6ee0.PNG)

```
route add -net 192.168.0.128 netmask 255.255.255.128 gw 192.168.0.2
route add -net 10.151.73.16 netmask 255.255.255.248 gw 192.168.0.2
route add -net 192.168.0.8 netmask 255.255.255.252 gw 192.168.0.6
route add -net 192.168.1.0 netmask 255.255.255.0 gw 192.168.0.6
route add -net 192.168.0.16 netmask 255.255.255.248 gw 192.168.0.6 
```

![routing venusaur](https://user-images.githubusercontent.com/42793740/69493375-cd6a9980-0ee0-11ea-92b3-649b9d8cc20d.PNG)

```
route add -net 0.0.0.0 netmask 0.0.0.0 gw 192.168.0.5
route add -net 192.168.0.16 netmask 255.255.255.248 gw 192.168.0.10 
```

# Kendala yang dialami 

- Keterbatasan waktu
