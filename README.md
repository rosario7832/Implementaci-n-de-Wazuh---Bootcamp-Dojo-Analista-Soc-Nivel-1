# Laboratorio: SIEM con Wazuh

## Descripción
Implementación práctica de un **SIEM open source** en un entorno local con fines educativos y de capacitación en ciberseguridad.

## Objetivos
- Implementar el SIEM open source **Wazuh** en un entorno local.  
- Instalar agentes de recolección de logs en equipos/servicios.  
- Familiarizarse con las principales funcionalidades del SIEM.  
# Laboratorio: SIEM con Wazuh

## Parte I - Importar la OVA de Wazuh

1. **Descargar la OVA desde el sitio oficial de Wazuh:**  
   👉 [Wazuh Virtual Machine](https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html)

2. **Abrir VirtualBox (o tu software de virtualización preferido).**

3. **Importar la OVA:**
   - En VirtualBox, ir a **Archivo > Importar servicio virtualizado**.  
   - Seleccionar el archivo `.ova` descargado.  
   - Revisar y ajustar los parámetros de hardware (CPU, RAM, disco) según los recursos disponibles.  

4. **Iniciar la máquina virtual Wazuh.**

<img src="https://i.imgur.com/vynkWp6.png" height="75%" width="70%"/>

- Usuario = wazuh-user
- contraseña = wazuh
  
 ***Validamos la IP que mantiene la máquina de Wazuh con el comando: ip addr***
 
 <img src="https://i.imgur.com/4lQx3WD.png" height="75%" width="70%"/>
 Nota: la IP a utilizar es la identificada como inet en la interfaz eth0


5. **Acceder a la interfaz web de Wazuh:**  
   - Una vez la VM esté corriendo, abre el navegador y dirígete a:  
     ```
     https://192.168.50.206
     ```
Credenciales para loguearse como administrador
   - Usuario = admin  
   - contraseña = admin
