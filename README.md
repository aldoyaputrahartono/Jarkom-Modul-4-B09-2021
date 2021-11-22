# Jarkom-Modul-4-B09-2021

Repositori Praktikum Jarkom Modul 4

|NRP           |Nama                   |
|:------------:|:---------------------:|
|05111940000084|Aldo Yaputra Hartono   |
|||
|||

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
![image](https://user-images.githubusercontent.com/81459084/142914120-a340b011-d3a1-4508-b241-419cd7f572d2.png)

### Setting GNS3


### Routing


## Kendala


## Pembagian Tugas
|Nama                   |Soal   |
|:---------------------:|:-----:|
|Aldo Yaputra Hartono   ||
|||
|||
