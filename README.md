# 🧩 Práctica: Configuración de red inalámbrica en Packet Tracer

Este laboratorio tiene como objetivo **configurar un router inalámbrico (WR)**, conectar dispositivos cableados e inalámbricos, y **ampliar la cobertura** mediante un punto de acceso adicional.

---

## 🛠️ Pasos realizados

### 1. Conexión inicial
- Conecté la **PC Admin** al **router inalámbrico (WR)**.
- Esperé a que se sincronizara correctamente la conexión.

### 2. Configuración de red en Admin
- Configuré la PC **Admin** para obtener una dirección IP por **DHCP**.
- La PC recibió la IP `192.168.0.100/24` con puerta de enlace `192.168.0.1`.

### 3. Acceso a la interfaz web del router
- Ingresé desde **Admin** a la interfaz web de **WR** mediante la IP `192.168.0.1`.
- En **Network Setup > Basic Setup**, verifiqué el **rango DHCP**.
- Confirmé que la IP asignada a Admin estaba dentro del rango configurado.

### 4. Configuración de la interfaz WAN del WR
- En el puerto **Internet**, cambié el método de dirección IP de:
  - `Automatic Configuration - DHCP` ➜ `Static IP`.
- Asigné los siguientes parámetros:
  - **IP de Internet:** `209.165.200.225`  
  - **Máscara de subred:** `255.255.255.252`  
  - **Puerta de enlace predeterminada:** `209.165.200.226`  
  - **Servidor DNS:** `209.165.201.1`

### 5. Verificación de conectividad
- Verifiqué la conectividad navegando hasta el servidor `www.cisco.pka`.

### 6. Configuración inalámbrica
- Configuré los parámetros para la red de **2.4 GHz**:
  - Cambié el **SSID** (nombre de la red).  
  - Seleccioné el **canal 6 - 2,437 GHz**.  
  - Desactivé ambas bandas de **5 GHz**.
- En **Wireless Security**, configuré:
  - **Seguridad:** WPA2  
  - **Cifrado:** AES  
  - **Clave:** `Cisco123!`

### 7. Conexión de clientes inalámbricos
- Conecté las **laptops 1 y 2** a la red configurada.
- Probé la conectividad y acceso a la red inalámbrica.

### 8. Configuración administrativa
- En **Administration > Management**, cambié la contraseña de acceso del router a `cisco`.

### 9. Ajuste de DHCP
- Modifiqué el intervalo de direcciones del **servidor DHCP** en WR para un mejor control de la red.

### 10. Ampliación de cobertura
- Agregué un **punto de acceso (AP)** y lo configuré correctamente.
- Conecté la **Laptop3** al nuevo AP (`CH1`) y verifiqué la conectividad.

---

## 📡 Resultados
- Todos los dispositivos cableados e inalámbricos se conectaron correctamente.  
- El router y el punto de acceso amplían la cobertura Wi-Fi de manera estable.  
- Se verificó acceso a Internet y gestión desde la interfaz web.

---

## 🧠 Tecnologías y conceptos aplicados
- Cisco Packet Tracer  
- Redes LAN inalámbricas (WLAN)  
- Configuración de router y AP  
- DHCP y direccionamiento estático  
- Seguridad inalámbrica WPA2/AES  
