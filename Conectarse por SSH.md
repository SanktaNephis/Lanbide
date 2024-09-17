# Conectarse por SSH


- [Conectarse por SSH](#conectarse-por-ssh)
  - [Conectarse por SSH en Windows](#conectarse-por-ssh-en-windows)
  - [Arrancar servicio SSH en Linux](#arrancar-servicio-ssh-en-linux)
  - [Configurar el servicio en Linux](#configurar-el-servicio-en-linux)
  
Para conectarse por SSH a un equipo, se deben cumplir los siguientes requisitos:
- Que el servicio de SSH esté encendidos
- Que el servidor/equipo al que vamos a conectarnos esté disponible
- Un cliente SSH en nuestro equipo (la mayoría de SOs ya incluyen uno)
  
  Además, para conectarnos, tendremos que conocer:
  1. La IP o nombre del servidor
  2. Un usuario y contraseña con el que conectarse


## Conectarse por SSH en Windows

```bash
ssh 196.169.10.0@ingrid
```

- **196.169.10.0**: IP del servidor
- **Ingrid**: usuario

## Arrancar servicio SSH en Linux

Para arrancar un servicio en Linux se utiliza el comando `systemctl start`

```bash
systemctl start ssh.service
```

## Configurar el servicio en Linux

Para configurar el servicio en Linux y cambiar propiedades como el número de usuarios que se pueden conectar a la vez, las blacklists y demás, usamos el comando: `**etc/ssh/ssh.config**`

