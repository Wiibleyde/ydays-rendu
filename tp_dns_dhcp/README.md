# TP 1 : DNS DHCP

## 1. Trouvez l’adresse réseau, broadcast, masque sous-réseau, nombre de client possible, plages des clients possibles sur les réseaux suivants 

- `192.168.0.0/24` : 
  * Adresse réseau : `192.168.0.0`
  * Adresse broadcast : `192.168.0.255`
  * Masque sous-réseau : `255.255.255.0`
  * Nombre de client possible : `254`
  * Plage des clients possibles : `192.168.0.1 - 192.168.0.254`
- `10.0.0.0/8` : 
  * Adresse réseau : `10.0.0.0`
  * Adresse broadcast : `10.255.255.255` 
  * Masque sous-réseau : `255.0.0.0`
  * Nombre de client possible : `16,777,214`
  * Plage des clients possibles : `10.0.0.1 - 10.255.255.254`
- `172.16.0.0/255.255.0.0172.16.0.0` : 
  * Adresse réseau : `172.16.0.0`172.16.255.255`
  * Adresse broadcast : `172.16.255.255`
  * Masque sous-réseau : `255.255.0.0`
  * Nombre de client possible : `65,534`
  * Plage des clients possibles : `172.16.0.1 - 172.16.255.254`
- `192.168.255.0/30` : 
  * Adresse réseau : `192.168.255.0`
  * Adresse broadcast : `192.168.255.3`
  * Masque sous-réseau : `255.255.255.252`
  * Nombre de client possible : `2`
  * Plage des clients possibles : `192.168.255.1 - 192.168.255.2`
- `10.50.0.0/22` : 
  * Adresse réseau : `10.50.0.0`
  * Adresse broadcast : `10.50.3.255`
  * Masque sous-réseau : `255.255.252.0`
  * Nombre de client possible : `1,024`
  * Plage des clients possibles : `10.50.0.1 - 10.50.3.254`
- `172.28.0.0/255.248.0.0` :
  * Adresse réseau : `172.24.0.0`
  * Adresse broadcast : `172.31.255.255`
  * Masque sous-réseau : `255.248.0.0`
  * Nombre de client possible : `1,048,576`
  * Plage des clients possibles : `172.24.0.1 - 172.31.255.254`

