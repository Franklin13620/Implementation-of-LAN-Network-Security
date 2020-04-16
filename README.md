# Implementation-of-LAN-Network-Security
### REQUERIMIENTOS:
- [x] **A**. Configure las VLANs, rangos de interfaces y enrutamiento Inter-VLAN de acuerdo con la siguiente información:

| VLANs | Nombre | Switches | IPv4 | Inter-VLAN |
| :---: | :---: | :---: | :---: | :---: |
| 10 | Guatemala | S1,S2,S3 | 192.25.10.0/25 | Router-on-a-stick |
| 20 | EEUU | S1,S2,S3 | 192.25.10.128/25 | Router-on-a-stick |
| 30 | ELSalvador | S4,S5,S6 | 192.25.20.0/25 | Router-on-a-stick |
| 40 | Colombia | S4,S5,S6 | 192.25.20.128/25 | Router-on-a-stick |
| 50 | Italia | S7,S8,S9 | 192.25.30.0/26 | Router-on-a-stick |
| 60 | Panama | S7,S8,S9 | 192.25.30.64/26 | Router-on-a-stick |
| 70 | Servidor_Radius | S7,S8,S9 | 192.25.30.128/26 | Router-on-a-stick |
|  |  |  |  |  |
| 10 | Mexico | SW-1,SW-2,SW-3 | 172.25.10.0/25 | Router-on-a-stick |
| 20 | Espania | SW-1,SW-2,SW-3 | 172.25.10.0/25 | Router-on-a-stick |
| 30 | Honduras | SW-4,SW-5,SW-6 | 172.25.20.0/26 | Router-on-a-stick |
| 40 | Brasil | SW-4,SW-5,SW-6 | 172.25.20.64/26 | Router-on-a-stick |
| 50 | Servidor_Tacacs | SW-4,SW-5,SW-6 | 172.25.20.128/26 | Router-on-a-stick |

- [x] **B**. La asignación de direcciones IPs para las computadoras de las VLANs será mediante el servicio de DHCP.

- [x] **C**. Configure el protocolo EIGRP para que los dispositivos de la red interna se comuniquen y anuncie una rutaestática hacia el ISP y viceversa.

- [ ] **D**. Permita que los puertos de acceso aprendan 6 direcciones MAC en caso de que haya infracción las
interfaces deben apagarse con un tiempo de envejecimiento de 10 minutos.

- [ ] **E**. El tráfico no etiquetado debe viajar por la VLAN 100 además deshabilite la propagación de BPDU y evite los estados de escucha y aprendizaje para minimizar el tiempo de convergencia de STP.

- [ ] **F**. Habilite la mitigación DHCP snooping y ARP en los switches donde configuro las VLANs .

- [ ] **G**. Utilizando el modelo AAA cree un grupo llamado CafeNegroLeaks para almacenar la lista de usuarios de
inicio de sesión en el router R2 y configure en el Servidor_Radius cada uno de los integrantes del
microgrupo de trabajo con su respectiva contraseña.

- [ ] **H**. Utilizando el modelo AAA cree un grupo llamado CafeNegro para almacenar la lista de usuarios de inicio de sesión en el router R4 y configure en el Servidor_Tacacs cada uno de los integrantes del microgrupo de trabajo con su respectiva contraseña.

- [ ] **I**. En los routers R2 y R4 configure el acceso vía SSH y agregue el usuario local Gabriela con la contraseña DondeEstaGabriela.

### Topologia de la Red:
![alt text](https://raw.githubusercontent.com/Franklin13620/Implementation-of-LAN-Network-Security/master/assets/Topologia.png)