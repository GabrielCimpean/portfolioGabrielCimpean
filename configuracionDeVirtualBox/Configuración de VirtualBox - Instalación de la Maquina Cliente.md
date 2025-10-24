# Configuración de VirtualBox - Instalación de la Maquina Cliente

[TOC]

## 1- Configuración de Virtual Box 

Lo primero escogemos el modo *Expert*

<img src="./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919104458840.png" alt="image-20250919104458840" style="zoom: 67%;" />

Vamos a añadir una Red de tipo NAT para poder conectar varias máquinas virtuales

<img src="./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919104800409.png" alt="image-20250919104800409"  />

Configuramos la red:

<img src="./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919105006338.png" alt="image-20250919105006338" style="zoom: 80%;" />

## 2 - Creación de la nueva máquina Cliente Ubuntu

Establecemos los parámetros de la Nueva Máquina:

<img src="./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919110047790.png" style="zoom:50%;" />

![image-20250919110626586](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919110626586.png)

![image-20250919110702591](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919110702591.png)

Podemos ver la nueva máquina:

<img src="./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919110816662.png" alt="image-20250919110816662" style="zoom: 67%;" />

Cambiamos algunos ajustes:

- En la **Descripción** guardamos el usuario y la contraseña de la máquina.

  <img src="./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919111340972.png" alt="image-20250919111340972" style="zoom: 80%;" />

- Deshabilitamos el **Audio**:

  ![image-20250919111508840](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919111508840.png)

- El adaptador de **Red** debe ser `Red NAT`:

  ![image-20250919111735724](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919111735724.png)

> Configuración finalizada, ya podemos INICIAR la máquina!!

## 3- Instalación de la máquina virtual

Nos van apareciendo diferentes opciones:

![image-20250919121040422](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919121040422.png)

![image-20250919121223012](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919121223012.png)

## 4 - Instalación de las Guest Additions

![image-20250919123638867](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919123638867.png)

Ejecutamos el comando:

```
sudo apt install bzip2 tar
```

![image-20250919124127356](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919124127356.png)

Restan algunos paquetes por instalar

```
sudo apt install gcc make perl
```

![image-20250919124459682](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919124459682.png)

Ejecutamos el programa

![image-20250919124542276](./Configuración de VirtualBox - Instalación de la Maquina Cliente.assets/image-20250919124542276.png)

### **Para utilizar carpetas compartidas**

Instalamos las utilidades 

```bash
$ sudo apt install virtualbox-guest-utils
```

También ejecutamos este comando:

```bash
$ sudo usermod -aG vboxsf cliente
```

