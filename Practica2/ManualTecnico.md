## **¡Manual técnico!**

# Tabla de resumen de todas las direcciones IP utilizadas en la práctica:

<table>
  <thead>
    <tr>
      <th>Dispositivo</th>
      <th>Dirección IP</th>
      <th>Máscara de Subred</th>
      <th>Gateway</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Central</td>
      <td>10.0.0.1</td>
      <td>255.255.255.252/30</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>Central</td>
      <td>123.168.1.2</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>Central</td>
      <td>123.168.2.2</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R2</td>
      <td>123.168.1.1</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>Central</td>
      <td>123.168.0.2</td>
      <td>255.255.255.0/24</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R3</td>
      <td>123.168.2.1</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R3</td>
      <td>123.168.0.3</td>
      <td>255.255.255.0/24</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R2-R3</td>
      <td>123.168.0.1</td>
      <td>255.255.255.0/24</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>VPC11</td>
      <td>123.168.0.4</td>
      <td>255.255.255.0/24</td>
      <td>123.168.0.1</td>
    </tr>
    <tr>
      <td>Villa_Nueva</td>
      <td>10.0.0.2</td>
      <td>255.255.255.252/30</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>Villa_Nueva</td>
      <td>123.178.1.1</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>Villa_Nueva</td>
      <td>123.178.2.1</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R5</td>
      <td>123.178.1.2</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R5</td>
      <td>123.178.0.2</td>
      <td>255.255.255.0/24</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R6</td>
      <td>123.178.2.2</td>
      <td>255.255.255.248/29</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R6</td>
      <td>123.178.0.3</td>
      <td>255.255.255.0/24</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>R5-R6</td>
      <td>123.178.0.1</td>
      <td>255.255.255.0/24</td>
      <td>No aplica</td>
    </tr>
    <tr>
      <td>VPC12</td>
      <td>123.178.0.4</td>
      <td>255.255.255.0/24</td>
      <td>123.178.0.1</td>
    </tr>
  </tbody>
</table>

# Tabla de datos de subredes

<table>
    <thead>
      <tr>
        <th>Subred</th>
        <th>Máscara de Subred</th>
        <th>Total de IP Disponibles</th>
        <th>Primera IP Disponible</th>
        <th>Última IP Disponible</th>
        <th>Dirección de Broadcast</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>255.255.255.0/24</td>
        <td>255.255.255.0</td>
        <td>256</td>
        <td>123.168.1.1</td>
        <td>123.168.1.254</td>
        <td>123.168.1.255</td>
      </tr>
      <tr>
        <td>255.255.255.248/29</td>
        <td>255.255.255.248</td>
        <td>8</td>
        <td>123.168.1.1</td>
        <td>123.168.1.6</td>
        <td>123.168.1.7</td>
      </tr>
      <tr>
        <td>255.255.255.252/30</td>
        <td>255.255.255.252</td>
        <td>4</td>
        <td>123.168.1.1</td>
        <td>123.168.1.2</td>
        <td>123.168.1.3</td>
      </tr>
    </tbody>
  </table>

## Configuración de routers Central, R2 y R5, configuración de switch SW7, configuración de VPC11

### Router Central

- `enable`: Ingresa al modo de configuración privilegiada.
- `configure terminal`: Ingresa al modo de configuración global.
- `hostname Central`: Configura el nombre del host como "Central".
- `interface e0/0`: Ingresa a la configuración de la interfaz Ethernet 0/0.
- `ip address 123.168.1.2 255.255.255.248`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `exit`: Sale de la configuración de la interfaz.
- `interface e0/1`: Ingresa a la configuración de la interfaz Ethernet 0/1.
- `ip address 123.168.2.2 255.255.255.248`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `exit`: Sale de la configuración de la interfaz.
- `interface s1/0`: Ingresa a la configuración de la interfaz Serial 1/0.
- `ip address 10.0.0.1 255.255.255.252`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `exit`: Sale de la configuración de la interfaz.
- `ip route 123.168.0.0 255.255.255.0 123.168.1.1`: Configura una ruta estática.
- `ip route 123.168.0.0 255.255.255.0 123.168.2.1`: Configura otra ruta estática.
- `ip route 123.178.0.0 255.255.255.0 123.178.1.2`: Configura una tercera ruta estática.
- `ip route 123.178.0.0 255.255.255.0 123.178.2.2`: Configura otra ruta estática.
- `ip route 123.178.1.0 255.255.255.248 10.0.0.2`: Configura una ruta estática más.
- `ip route 123.178.2.0 255.255.255.248 10.0.0.2`: Configura otra ruta estática.
- `do write`: Guarda la configuración en la memoria del dispositivo.

### Router R2

- `enable`: Ingresa al modo de configuración privilegiada.
- `configure terminal`: Ingresa al modo de configuración global.
- `hostname R2`: Configura el nombre del host como "R2".
- `interface e0/0`: Ingresa a la configuración de la interfaz Ethernet 0/0.
- `ip address 123.168.1.1 255.255.255.248`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `exit`: Sale de la configuración de la interfaz.
- `interface e0/1`: Ingresa a la configuración de la interfaz Ethernet 0/1.
- `ip address 123.168.0.2 255.255.255.0`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `glbp 1 ip 123.168.0.1`: Configura una dirección IP virtual para el protocolo GLBP.
- `glbp 1 priority 150`: Establece la prioridad GLBP.
- `glbp 1 preempt`: Habilita la prelación en el protocolo GLBP.
- `glbp 1 load-balancing round-robin`: Configura el equilibrio de carga para GLBP.
- `exit`: Sale de la configuración de la interfaz.
- `ip route 10.0.0.0 255.255.255.252 123.168.1.2`: Configura una ruta estática.
- `ip route 123.168.2.0 255.255.255.248 123.168.0.3`: Configura otra ruta estática.
- `ip route 123.178.0.0 255.255.255.0 123.178.1.2`: Configura una tercera ruta estática.
- `ip route 123.178.0.0 255.255.255.0 123.178.2.2`: Configura otra ruta estática.
- `ip route 123.178.1.0 255.255.255.248 10.0.0.2`: Configura una ruta estática más.
- `ip route 123.178.2.0 255.255.255.248 10.0.0.2`: Configura otra ruta estática.

### Router R5

- `enable`: Ingresa al modo de configuración privilegiada.
- `configure terminal`: Ingresa al modo de configuración global.
- `hostname R5`: Configura el nombre del host como "R5".
- `interface e0/0`: Ingresa a la configuración de la interfaz Ethernet 0/0.
- `ip address 123.178.1.2 255.255.255.248`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `exit`: Sale de la configuración de la interfaz.
- `interface e0/1`: Ingresa a la configuración de la interfaz Ethernet 0/1.
- `ip address 123.168.0.2 255.255.255.0`: Asigna la dirección IP y máscara de subred a la interfaz.
- `no shutdown`: Habilita la interfaz.
- `standby 1 ip 123.178.0.1`: Configura una dirección IP virtual para HSRP.
- `standby 1 version 2`: Establece la versión HSRP.
- `standby 1 priority 150`: Establece la prioridad HSRP.
- `standby 1 preempt`: Habilita la prelación en HSRP.
- `exit`: Sale de la configuración de la interfaz.
- `ip route 10.0.0.0 255.255.255.252 123.178.1.1`: Configura una ruta estática.
- `ip route 123.168.0.0 255.255.255.0 123.168.1.1`: Configura otra ruta estática.
- `ip route 123.168.1.0 255.255.255.0 123.168.2.1`: Configura una tercera ruta estática.
- `ip route 123.168.1.0 255.255.255.248 10.0.0.1`: Configura una ruta estática más.
- `ip route 123.168.2.0 255.255.255.248 10.0.0.1`: Configura otra ruta estática.
- `ip route 123.178.2.0 255.255.255.248 123.178.0.3`: Configura una última ruta estática.

### Switch SW7

- `enable`: Ingresa al modo de configuración privilegiada.
- `configure terminal`: Ingresa al modo de configuración global.
- `hostname SW7`: Configura el nombre del switch como "SW7".
- `interface Port-channel 1`: Ingresa a la configuración del grupo de puertos.
- `description LACP`: Agrega una descripción al grupo de puertos.
- `exit`: Sale de la configuración del grupo de puertos.
- `interface range e0/2-3`: Ingresa a la configuración de un rango de interfaces desde Ethernet 0/2 hasta 0/3.
- `channel-group 1 mode passive`: Configura el grupo de puertos en modo pasivo.
- `exit`: Sale de la configuración de las interfaces.

### VPC11

- `ip 123.168.0.4/24 123.168.0.1`: Asigna una dirección IP a VPC11 con la puerta de enlace predeterminada.
- `save`: Guarda la configuración de VPC11.

## Resumen de los comandos usados: Creación de ruta estática, creación de PortChannel con PAGP y LACP, creación de IP virtual con HSRP y GLBP y configuración de VPC.

### Port Channels LACP

**SW7**
- `interface Port-channel 1`: Ingresa a la configuración del grupo de puertos.
- `description LACP`: Agrega una descripción al grupo de puertos.
- `exit`: Sale de la configuración del grupo de puertos.
- `interface range e0/2-3`: Ingresa a la configuración de un rango de interfaces desde Ethernet 0/2 hasta 0/3.
- `channel-group 1 mode passive`: Configura el grupo de puertos en modo pasivo.
- `exit`: Sale de la configuración de las interfaces.

**SW8**
- `interface Port-channel 1`: Ingresa a la configuración del grupo de puertos.
- `description LACP`: Agrega una descripción al grupo de puertos.
- `exit`: Sale de la configuración del grupo de puertos.
- `interface range e0/0-1`: Ingresa a la configuración de un rango de interfaces desde Ethernet 0/0 hasta 0/1.
- `channel-group 1 mode active`: Configura el grupo de puertos en modo activo.
- `exit`: Sale de la configuración de las interfaces.

### Port Channels PAgP

**SW9**
- `interface Port-channel 1`: Ingresa a la configuración del grupo de puertos.
- `description PACP`: Agrega una descripción al grupo de puertos.
- `exit`: Sale de la configuración del grupo de puertos.
- `interface range e0/2-3`: Ingresa a la configuración de un rango de interfaces desde Ethernet 0/2 hasta 0/3.
- `channel-group 1 mode auto`: Configura el grupo de puertos en modo auto.
- `exit`: Sale de la configuración de las interfaces.

**SW10**
- `interface Port-channel 1`: Ingresa a la configuración del grupo de puertos.
- `description LACP`: Agrega una descripción al grupo de puertos.
- `exit`: Sale de la configuración del grupo de puertos.
- `interface range e0/0-1`: Ingresa a la configuración de un rango de interfaces desde Ethernet 0/0 hasta 0/1.
- `channel-group 1 mode desirable`: Configura el grupo de puertos en modo deseable.
- `exit`: Sale de la configuración de las interfaces.

### Rutas Estáticas

**Ejemplo para Router R5:**

- `ip route 10.0.0.0 255.255.255.252 123.178.1.1`: Configura una ruta estática.
- `ip route 123.168.0.0 255.255.255.0 123.168.1.1`: Configura otra ruta estática.
- `ip route 123.168.1.0 255.255.255.0 123.168.2.1`: Configura una tercera ruta estática.
- `ip route 123.168.1.0 255.255.255.248 10.0.0.1`: Configura una ruta estática más.
- `ip route 123.168.2.0 255.255.255.248 10.0.0.1`: Configura otra ruta estática.
- `ip route 123.178.2.0 255.255.255.248 123.178.0.3`: Configura una última ruta estática.

### IP Virtual para HSRP y GLBP

**Configuración HSRP para Router R5:**

- `interface e0/1`: Ingresa a la configuración de la interfaz Ethernet 0/1.
- `standby 1 ip 123.178.0.1`: Configura una dirección IP virtual para HSRP.
- `standby 1 version 2`: Establece la versión HSRP.
- `standby 1 priority 150`: Establece la prioridad HSRP.
- `standby 1 preempt`: Habilita la prelación en HSRP.
- `exit`: Sale de la configuración de la interfaz.

**Configuración GLBP para Router R5:**

- `interface e0/1`: Ingresa a la configuración de la interfaz Ethernet 0/1.
- `glbp 1 ip 123.168.0.1`: Configura una dirección IP virtual para GLBP.
- `glbp 1 priority 150`: Establece la prioridad GLBP.
- `glbp 1 preempt`: Habilita la prelación en GLBP.
- `glbp 1 load-balancing round-robin`: Configura el balanceo de carga en GLBP.
- `exit`: Sale de la configuración de la interfaz.

### Configuración VPC

- `ip 123.168.0.4/24 123.168.0.1`: Asigna una dirección IP a VPC con la puerta de enlace predeterminada.
- `save`: Guarda la configuración de VPC.

## Comandos empleados para la verificación del correcto funcionamiento de los protocolos empleados para la realización de la práctica

### Verificación General

- `show running-config`: Muestra casi toda la configuración actual del dispositivo.
  
**Router:**

- `show ip route`: Proporciona información sobre las rutas estáticas configuradas en el router.

**HSRP:**

- `show standby`: Muestra información detallada sobre el estado de HSRP.
- `show standby brief`: Muestra un resumen conciso del estado de HSRP.

**GLBP:**

- `show glbp`: Muestra información detallada sobre el estado de GLBP.
- `show glbp brief`: Muestra un resumen conciso del estado de GLBP.

**Port-Channel (LACP o PAgP):**

- `show etherchannel summary`: Proporciona un resumen de los canales EtherChannel configurados.
- `show run interface 1`: Muestra la configuración de una interfaz específica del Port-Channel.
- `show interfaces 1 switchport`: Muestra información sobre la configuración de la interfaz en el Port-Channel.
- `show lacp neighbor`: Muestra información sobre los vecinos LACP (puede ser PAgP en su lugar).

Estos comandos te ayudarán a verificar y validar la configuración y el estado de tu red. Puedes utilizarlos según sea necesario para obtener información específica sobre el dispositivo y su funcionamiento.
