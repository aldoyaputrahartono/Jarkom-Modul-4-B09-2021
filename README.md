# Jarkom-Modul-4-B09-2021

Repositori Praktikum Jarkom Modul 4

|NRP           |Nama                   |
|:------------:|:---------------------:|
|05111940000084|Aldo Yaputra Hartono   |
|05111940000092|Maximilian H M Lingga  |
|05111840000023|Izzulhaq Fawwaz Syauqiy|

## Topologi
![soal](https://user-images.githubusercontent.com/31863229/142765592-e971b1a2-0214-4565-811a-87f083ecc4f3.PNG)

## CPT - VLSM
### Pembagian subnet
![c1](https://user-images.githubusercontent.com/31863229/142777462-03a67e5a-f0e3-4b3a-9223-b0ea659e6fc0.png)

### Perhitungan subnet
|Subnet|Jumlah IP|Netmask|
|------|---------|-------|
|A1|1001|/22|
|A2|2|/30|
|A3|701|/22|
|A4|2|/30|
|A5|2021|/21|
|A6|101|/25|
|A7|2|/30|
|A8|521|/22|
|A9|502|/23|
|A10|13|/28|
|A11|2|/30|
|A12|252|/24|
|A13|721|/22|
|**Total**|**5841**|**/19**|

### VLSM Tree
![c2](https://user-images.githubusercontent.com/31863229/142777556-b5c3fa17-f9bd-427e-8cc3-a38e27724d5d.png)

### Pembagian IP
|Subnet|Network ID|Netmask|
|------|----------|-------|
|A1|192.181.8.0|255.255.252.0|
|A2|192.181.0.0|255.255.255.252|
|A3|192.181.12.0|255.255.252.0|
|A4|192.181.0.4|255.255.255.252|
|A5|192.181.24.0|255.255.248.0|
|A6|192.181.0.128|255.255.255.128|
|A7|192.181.0.8|255.255.255.252|
|A8|192.181.16.0|255.255.252.0|
|A9|192.181.2.0|255.255.254.0|
|A10|192.181.0.16|255.255.255.240|
|A11|192.181.0.12|255.255.255.252|
|A12|192.181.1.0|255.255.255.0|
|A13|192.181.20.0|255.255.252.0|

### Routing
|Router|Subnet|Network ID|Netmask|Next Hop|
|------|------|----------|-------|--------|
|**FOOSHA**|A3|192.181.12.0|255.255.252.0|192.181.0.2|
||A5|192.181.24.0|255.255.248.0|192.181.0.2|
||A6|192.181.0.128|255.255.255.128|192.181.0.2|
||A8|192.181.16.0|255.255.252.0|192.181.1.10|
||A9|192.181.2.0|255.255.254.0|192.181.1.10|
||A10|192.181.0.16|255.255.255.240|192.181.1.10|
||A12|192.181.1.0|255.255.255.0|192.181.1.10|
||A13|192.181.20.0|255.255.252.0|192.181.1.10|
||FUKUROU|10.151.79.108|255.255.255.252|192.181.1.10|
|**WATER7**|DEFAULT|0.0.0.0|0.0.0.0|192.181.0.1|
||A5|192.181.24.0|255.255.248.0|192.181.0.6|
||A6|192.181.0.128|255.255.255.128|192.181.0.6|
|**PUCCI**|DEFAULT|0.0.0.0|0.0.0.0|192.181.0.5|
|**GUANHAO**|DEFAULT|0.0.0.0|0.0.0.0|192.181.0.9|
||A10|192.181.0.16|255.255.255.240|192.181.2.2|
||A12|192.181.1.0|255.255.255.0|192.181.0.14|
||A13|192.181.20.0|255.255.252.0|192.181.0.14|
||FUKUROU|10.151.79.108|255.255.255.252|192.181.0.14|
|**ALABASTA**|DEFAULT|0.0.0.0|0.0.0.0|192.181.2.1|
|**OIMO**|DEFAULT|0.0.0.0|0.0.0.0|192.181.0.13|
||A13|192.181.20.0|255.255.252.0|192.181.1.2|
|**SEASTONE**|DEFAULT|0.0.0.0|0.0.0.0|192.181.1.1|

## GNS3 - CIDR
### Pembagian subnet
**Langkah 1**
![c1](https://user-images.githubusercontent.com/31863229/142777462-03a67e5a-f0e3-4b3a-9223-b0ea659e6fc0.png)

**Langkah 2**
![g1](https://user-images.githubusercontent.com/31863229/142810611-684a1bbe-ae73-4aab-b6af-066ca8f4b5de.png)

**Langkah 3**
![g2](https://user-images.githubusercontent.com/31863229/142810624-4624bd3d-4aba-46d8-8ff6-791b7d7b6ac9.png)

**Langkah 4**
![g3](https://user-images.githubusercontent.com/31863229/142810638-386b21d0-db72-4910-9c44-83e4bb77d5d4.png)

**Langkah 5**
![g4](https://user-images.githubusercontent.com/31863229/142810659-a6eb3d31-9f39-4485-a887-528b4991a923.png)

**Langkah 6**
![g5](https://user-images.githubusercontent.com/31863229/142810676-1511d433-8618-47a0-8455-ca97d4463541.png)

**Langkah 7**
![g6](https://user-images.githubusercontent.com/31863229/142810689-9edecc00-5d43-432a-84fd-f54066365f68.png)

**Hasil subnetting**
![g7](https://user-images.githubusercontent.com/31863229/142810707-01d3c9a7-7030-45a5-9849-fc243a400e2b.png)

### CIDR Tree
![g8](https://user-images.githubusercontent.com/31863229/143030104-10faa525-ee24-4d32-aaaa-b598e6233d9e.png)

### Setting GNS3
**Router**
- **FOOSHA**
```
auto eth0
iface eth0 inet dhcp

auto eth1
iface eth1 inet static
	address 192.181.192.1
	netmask 255.255.252.0

auto eth2
iface eth2 inet static
	address 192.181.64.1
	netmask 255.255.255.252

auto eth3
iface eth3 inet static
	address 192.181.160.1
	netmask 255.255.255.252

auto eth4
iface eth4 inet static
	address 10.151.79.105
	netmask 255.255.255.252
```

- **WATER7**
```
auto eth0
iface eth0 inet static
	address 192.181.64.2
	netmask 255.255.255.252
	gateway 192.181.64.1

auto eth1
iface eth1 inet static
	address 192.181.32.1
	netmask 255.255.252.0

auto eth2
iface eth2 inet static
	address 192.181.16.1
	netmask 255.255.255.252
```

- **PUCCI**
```
auto eth0
iface eth0 inet static
	address 192.181.16.2
	netmask 255.255.255.252
	gateway 192.181.16.1

auto eth1
iface eth1 inet static
	address 192.181.0.1
	netmask 255.255.248.0

auto eth2
iface eth2 inet static
	address 192.181.8.1
	netmask 255.255.255.128
```

- **GUANHAO**
```
auto eth0
iface eth0 inet static
	address 192.181.160.2
	netmask 255.255.255.252
	gateway 192.181.160.1

auto eth1
iface eth1 inet static
	address 192.181.132.1
	netmask 255.255.252.0

auto eth2
iface eth2 inet static
	address 192.181.128.1
	netmask 255.255.254.0

auto eth3
iface eth3 inet static
	address 192.181.152.1
	netmask 255.255.255.252
```

- **ALABASTA**
```
auto eth0
iface eth0 inet static
	address 192.181.128.2
	netmask 255.255.254.0
	gateway 192.181.128.1

auto eth1
iface eth1 inet static
	address 192.181.130.1
	netmask 255.255.255.240
```

- **OIMO**
```
auto eth0
iface eth0 inet static
	address 192.181.152.2
	netmask 255.255.255.252
	gateway 192.181.152.1

auto eth1
iface eth1 inet static
	address 192.181.144.1
	netmask 255.255.255.0

auto eth2
iface eth2 inet static
	address 10.151.79.109
	netmask 255.255.255.252
```

- **SEASTONE**
```
auto eth0
iface eth0 inet static
	address 192.181.144.2
	netmask 255.255.255.0
	gateway 192.181.144.1

auto eth1
iface eth1 inet static
	address 192.181.148.1
	netmask 255.255.252.0
```

**Client**
- **BLUENO**
```
auto eth0
iface eth0 inet static
	address 192.181.192.2
	netmask 255.255.252.0
	gateway 192.181.192.1
```

- **CIPHER**
```
auto eth0
iface eth0 inet static
	address 192.181.32.2
	netmask 255.255.252.0
	gateway 192.181.32.1
```

- **CALMBELT**
```
auto eth0
iface eth0 inet static
	address 192.181.0.2
	netmask 255.255.248.0
	gateway 192.181.0.1
```

- **COURTYARD**
```
auto eth0
iface eth0 inet static
	address 192.181.0.3
	netmask 255.255.248.0
	gateway 192.181.0.1
```

- **JIPANGU**
```
auto eth0
iface eth0 inet static
	address 192.181.8.2
	netmask 255.255.255.128
	gateway 192.181.8.1
```

- **JABRA**
```
auto eth0
iface eth0 inet static
	address 192.181.132.2
	netmask 255.255.252.0
	gateway 192.181.132.1
```

- **MAINGATE**
```
auto eth0
iface eth0 inet static
	address 192.181.128.3
	netmask 255.255.254.0
	gateway 192.181.128.1
```

- **JORGE**
```
auto eth0
iface eth0 inet static
	address 192.181.130.2
	netmask 255.255.255.240
	gateway 192.181.130.1
```

- **ENIESLOBBY**
```
auto eth0
iface eth0 inet static
	address 192.181.144.3
	netmask 255.255.255.0
	gateway 192.181.144.1
```

- **ELENA**
```
auto eth0
iface eth0 inet static
	address 192.181.148.2
	netmask 255.255.252.0
	gateway 192.181.148.1
```

**Server**
- **DORIKI**
```
auto eth0
iface eth0 inet static
	address 10.151.79.106
	netmask 255.255.255.252
	gateway 10.151.79.105
```

- **FUKUROU**
```
auto eth0
iface eth0 inet static
	address 10.151.79.110
	netmask 255.255.255.252
	gateway 10.151.79.109
```

### Routing
- **FOOSHA**
```
route add -net 192.181.0.0 netmask 255.255.192.0 gw 192.181.64.2
route add -net 192.181.128.0 netmask 255.255.224.0 gw 192.181.160.2
route add -net 10.151.79.108 netmask 255.255.255.252 gw 192.181.160.2
```

- **WATER7**
```
route add -net 192.181.0.0 netmask 255.255.240.0 gw 192.181.16.2
```

- **GUANHAO**
```
route add -net 192.181.130.0 netmask 255.255.255.240 gw 192.181.128.2
route add -net 192.181.144.0 netmask 255.255.248.0 gw 192.181.152.2
route add -net 10.151.79.108 netmask 255.255.255.252 gw 192.181.152.2
```

- **OIMO**
```
route add -net 192.181.148.0 netmask 255.255.252.0 gw 192.181.144.2
```

Pada router FOOSHA, jalankan:
```
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE -s 192.181.0.0/16
```

Pada semua node (router dan client) selain FOOSHA, jalankan:
```
echo nameserver 192.168.122.1 > /etc/resolv.conf
```

## Kendala


## Pembagian Tugas
|Nama                   |Soal   |
|:---------------------:|:-----:|
|Aldo Yaputra Hartono   ||
|||
|||
