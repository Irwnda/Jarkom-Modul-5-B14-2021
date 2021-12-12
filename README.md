# Jarkom-Modul-5-B14-2021

![Untitled (1)](https://user-images.githubusercontent.com/45300477/145710982-59757371-2052-4c64-8e02-8a4f908612c5.jpg)

Tree VLSM adalah sebagai berikut:
![jarkom-Jarkom 5 drawio](https://user-images.githubusercontent.com/45300477/145711016-cacf04b7-22a5-48bf-ba84-66a9e7cb1335.png)

Berdasarkan tabel tersebut, didapat pembagian IP sebagai berikut:
| Subnet | Keterangan        | IP              |
| ------ | ----------------- | --------------- |
| A1     | NetworkID         | 10.14.0.8       |
|        | NetMask           | 255.255.255.248 |
|        | Broadcast Address | 10.14.0.15      |
| A2     | NetworkID         | 10.14.0.128     |
|        | NetMask           | 255.255.255.128 |
|        | Broadcast Address | 10.14.0.255     |
| A3     | NetworkID         | 10.14.4.0       |
|        | NetMask           | 255.255.252.0   |
|        | Broadcast Address | 10.14.7.255     |
| A4     | NetworkID         | 10.14.0.0       |
|        | NetMask           | 255.255.255.252 |
|        | Broadcast Address | 10.14.0.3       |
| A5     | NetworkID         | 10.14.0.4       |
|        | NetMask           | 255.255.255.252 |
|        | Broadcast Address | 10.14.0.7       |
| A6     | NetworkID         | 10.14.2.0       |
|        | NetMask           | 255.255.255.254 |
|        | Broadcast Address | 10.14.3.255     |
| A7     | NetworkID         | 10.14.1.0       |
|        | NetMask           | 255.255.255.0   |
|        | Broadcast Address | 10.14.0.255     |
| A8     | NetworkID         | 10.14.0.16      |
|        | NetMask           | 255.255.255.248 |
|        | Broadcast Address | 10.14.0.23      |


## Network Configuration
### Foosha
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 10.14.0.1
	netmask 255.255.255.252

auto eth2
iface eth2 inet static
	address 10.14.0.5
	netmask 255.255.255.252
```

### Water7
```
auto eth0
iface eth0 inet static
	address 10.14.0.2
	netmask 255.255.255.252

auto eth1
iface eth1 inet static
	address 10.14.0.129
	netmask 255.255.255.128

auto eth2
iface eth2 inet static
	address 10.14.0.9
	netmask 255.255.255.248

auto eth3
iface eth3 inet static
	address 10.30.4.1
	netmask 255.255.252.0
```

### Guanhao
```
auto eth0
iface eth0 inet static
	address 10.14.0.6
	netmask 255.255.255.252

auto eth1
iface eth1 inet static
	address 10.14.2.1
	netmask 255.255.254.0

auto eth2
iface eth2 inet static
	address 10.14.1.1
	netmask 255.255.255.248

auto eth3
iface eth3 inet static
	address 10.14.0.17
	netmask 255.255.255.0
```


### Doriki
```
auto eth0
iface eth0 inet static
	address 10.14.0.10
	netmask 255.255.255.248
	gateway 10.14.0.9
```

### Jipangu
```
auto eth0
iface eth0 inet static
	address 10.14.0.11
	netmask 255.255.255.248
	gateway 10.14.0.9
```

### Blueno, Cipher, Elena dan Fukurou
```
auto lo
iface lo inet loopback

auto eth0
iface eth0 inet dhcp
```

### Maingate
```
auto eth0
iface eth0 inet static
	address 10.14.0.19
	netmask 255.255.255.248
	gateway 10.14.0.17
```

### Jorge
```
auto eth0
iface eth0 inet static
	address 10.14.0.18
	netmask 255.255.255.248
	gateway 10.14.0.17
```
