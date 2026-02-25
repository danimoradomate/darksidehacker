---
layout: post
title: "Capítulo 2: Instalación de Jetson SDK Components"
date: 2026-02-25 12:00:00 -0600
description: "Guía para la instalación de componentes del SDK en la Jetson Nano"
tags: [jetson, tutorial]
categories: blog
featured: false
related_posts: false
giscus_comments: false
---

**Identificación de la dirección IP:**
Acceda a la terminal y ejecute el comando `ifconfig` para visualizar los parámetros de red de la Jetson Nano. Es fundamental identificar la dirección IP correspondiente a la interfaz de red activa; en este caso, al estar conectado de forma inalámbrica, deberá localizar la sección de la interfaz Wi-Fi para obtener el dato necesario, tal como se muestra en la fig. 31.

![Figura 31: Dirección IP](/assets/img/image031.png)
*Figura 31: Dirección IP*

---

**Configuración final en el SDK Manager:**
Inicie el entorno de WSL en su PC abriendo una terminal de Ubuntu a través de PowerShell. Una vez dentro de Linux, ejecute nuevamente el SDK Manager y seleccione las opciones indicadas en la fig. 32. En el Paso 2, es fundamental desmarcar la casilla de Jetson Linux, ya que esta opción corresponde al flasheo del sistema operativo, proceso que se completó con éxito en las etapas anteriores (fig. 33).

![Figura 32: Paso 1](/assets/img/image032.png)
*Figura 32: Paso 1*

![Figura 33: Paso 2](/assets/img/image033.png)
*Figura 33: Paso 2*

---

**Vinculación remota e instalación de componentes:**
Proceda al Paso 3; una vez finalizada la descarga y al intentar avanzar, el sistema solicitará la contraseña de su entorno Ubuntu local para otorgar los permisos necesarios. A continuación, se desplegará una ventana de configuración donde deberá ingresar la dirección IP de la Jetson Nano obtenida previamente, junto con el nombre de usuario y la contraseña asignados al dispositivo (fig. 34). Esta información permitirá que el SDK Manager establezca una conexión remota para transferir e instalar los componentes de software de manera directa.

![Figura 34: Conexión ethernet](/assets/img/image034.png)
*Figura 34: Conexión ethernet*

---

**Finalización de la instalación:**
Durante esta etapa, es imperativo asegurarse de que la Jetson Nano permanezca encendida y con una conexión de red estable para garantizar que la transferencia de datos sea exitosa. Una vez concluido el proceso, el sistema mostrará un mensaje de confirmación indicando que todos los componentes se han instalado correctamente, tal como se observa en la figura 35.

![Figura 35: Instalación completada](/assets/img/image035.png)
*Figura 35: Instalación completada*
