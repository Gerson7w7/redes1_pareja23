## **¡Manual técnico!**

# Tabla de resumen de todas las direcciones IP utilizadas en la práctica:

<table>
  <thead>
    <tr>
      <th>Dispositivo</th>
      <th>Dirección IP</th>
      <th>Máscara de Subred</th>
      <th>Puerta de Enlace Predeterminada</th>
      <th>VLAN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>SEGURIDAD</td>
      <td>172.16.27.2</td>
      <td>172.16.27.24</td>
      <td>172.16.27.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>INVEST</td>
      <td>172.16.26.2</td>
      <td>255.255.255.0</td>
      <td>172.16.26.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ADMINISTRACION</td>
      <td>172.16.24.2</td>
      <td>255.255.255.0</td>
      <td>172.16.24.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ACADEMICO</td>
      <td>172.16.25.2</td>
      <td>255.255.255.0</td>
      <td>172.16.25.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SW</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ESW1</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ESW2</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SW3</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SW4</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SW5</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SW6</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>No aplica</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ADM1</td>
      <td>172.16.24.3</td>
      <td>172.16.24.24</td>
      <td>172.16.24.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SEG1</td>
      <td>172.16.27.3</td>
      <td>172.16.27.24</td>
      <td>172.16.27.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>INV1</td>
      <td>172.16.26.3</td>
      <td>172.16.26.24</td>
      <td>172.16.26.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ACA2</td>
      <td>172.16.25.4</td>
      <td>172.16.25.24</td>
      <td>172.16.25.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>SEG2</td>
      <td>172.16.27.4</td>
      <td>172.16.27.24</td>
      <td>172.16.27.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ACA1</td>
      <td>172.16.25.3</td>
      <td>172.16.25.24</td>
      <td>172.16.25.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>ADM2</td>
      <td>172.16.24.4</td>
      <td>255.255.255.0</td>
      <td>172.16.24.1</td>
      <td>VLAN</td>
    </tr>
    <tr>
      <td>INV2</td>
      <td>172.16.26.4</td>
      <td>255.255.255.0</td>
      <td>172.16.26.1</td>
      <td>VLAN</td>
    </tr>
  </tbody>
</table>

# Captura de la implementación de la topología.

![No image](topologia.png)

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
