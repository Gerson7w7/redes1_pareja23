## **¡Título Importante!**

# Tabla de resumen de todas las direcciones IP utilizadas en la práctica:

<table>
  <thead>
    <tr>
      <th>Dispositivo</th>
      <th>Dirección IP</th>
      <th>Máscara de Subred</th>
      <th>Área</th>
      <th>Nivel</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>VPC4</td>
      <td>192.168.23.1</td>
      <td>255.255.255.0</td>
      <td>Recepción</td>
      <td>Nivel 1</td>
    </tr>
    <tr>
      <td>VPC5</td>
      <td>192.168.23.2</td>
      <td>255.255.255.0</td>
      <td>Recepción</td>
      <td>Nivel 1</td>
    </tr>
    <tr>
      <td>VPC6</td>
      <td>192.168.23.27</td>
      <td>255.255.255.0</td>
      <td>Almacenamiento de paquetes</td>
      <td>Nivel 1</td>
    </tr>
    <tr>
      <td>VPC7</td>
      <td>192.168.23.26</td>
      <td>255.255.255.0</td>
      <td>Almacenamiento de paquetes</td>
      <td>Nivel 1</td>
    </tr>
    <tr>
      <td>VPC8</td>
      <td>192.168.23.51</td>
      <td>255.255.255.0</td>
      <td>Atención al cliente</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC5</td>
      <td>192.168.23.53</td>
      <td>255.255.255.0</td>
      <td>Atención al cliente</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC10</td>
      <td>192.168.23.52</td>
      <td>255.255.255.0</td>
      <td>Atención al cliente</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC11</td>
      <td>192.168.23.54</td>
      <td>255.255.255.0</td>
      <td>Atención al cliente</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC12</td>
      <td>192.168.23.77</td>
      <td>255.255.255.0</td>
      <td>Oficina administrativa</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC13</td>
      <td>192.168.23.76</td>
      <td>255.255.255.0</td>
      <td>Oficina administrativa</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC14</td>
      <td>192.168.23.78</td>
      <td>255.255.255.0</td>
      <td>Oficina administrativa</td>
      <td>Nivel 2</td>
    </tr>
    <tr>
      <td>VPC15</td>
      <td>192.168.23.102</td>
      <td>255.255.255.0</td>
      <td>Gerencia</td>
      <td>Nivel 3</td>
    </tr>
    <tr>
      <td>VPC16</td>
      <td>192.168.23.101</td>
      <td>255.255.255.0</td>
      <td>Gerencia</td>
      <td>Nivel 3</td>
    </tr>
    <tr>
      <td>VPC17</td>
      <td>192.168.23.126</td>
      <td>255.255.255.0</td>
      <td>Operaciones</td>
      <td>Nivel 3</td>
    </tr>
    <tr>
      <td>VPC18</td>
      <td>192.168.23.127</td>
      <td>255.255.255.0</td>
      <td>Operaciones</td>
      <td>Nivel 3</td>
    </tr>
    <tr>
      <td>VPC19</td>
      <td>192.168.23.128</td>
      <td>255.255.255.0</td>
      <td>Operaciones</td>
      <td>Nivel 3</td>
    </tr>
  </tbody>
</table>

# Hardware para Topología de Red

## Primer Piso:
- **Switch**: Cisco Catalyst 2960X-24TS-L (1 unidad)
  - Switch de 24 puertos para segmentación de red y gestión del tráfico.

- **Área de Recepción**:
  - **Computadoras**: Dell OptiPlex 7070 (2 unidades)
    - Computadoras de escritorio para tareas administrativas en el área de recepción.

- **Área de Almacén de Paquetes**:
  - **Computadoras**: HP EliteDesk 800 G5 (2 unidades)
    - Computadoras de escritorio para gestión de paquetes y logística en el almacén.

## Segundo Piso:
- **Switch**: Cisco Catalyst 2960X-24TS-L (1 unidad)

- **Atención al Cliente**:
  - **Computadoras**: Lenovo ThinkCentre M920 (4 unidades)
    - Computadoras de atención al cliente para servicios y soporte.

- **Oficina Administrativa**:
  - **Computadoras**: Dell OptiPlex 7070 (3 unidades)
    - Computadoras de escritorio para tareas administrativas y gestión.

## Tercer Piso:
- **Switch**: Cisco Catalyst 2960X-24TS-L (1 unidad)

- **Gerencia**:
  - **Computadoras**: Apple iMac Pro (2 unidades)
    - Computadoras de alto rendimiento para ejecutivos y gerentes.

- **Operaciones**:
  - **Computadoras**: Lenovo ThinkCentre M920 (3 unidades)
    - Computadoras de escritorio para tareas operativas y administrativas.

## Observaciones Generales:
- **Cableado**: Utiliza cables Ethernet Cat 6 para conectar dispositivos a los switches.

- **Racks y Gabinetes**: Se necesitan racks para organizar switches y componentes de red.

- **UPS**: Instala sistemas de alimentación ininterrumpida (UPS) en cada piso.

- **Servidor**: Considera un servidor para almacenamiento centralizado y administración.

- **Firewall**: Puedes implementar un firewall para protección y control de tráfico.

**Nota:** Las marcas y modelos son ejemplos, asegúrate de elegir opciones adecuadas para tus necesidades.
