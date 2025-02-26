---
layout: post
title: Setting Up Jetson Nano Waveshare
date: 2025-02-17 15:09:00
description: Setting Up Jetson Nano Waveshare
tags: formatting code
categories: sample-posts
featured: true
giscus_comments: true
---

En esta publicación requiere de su ayuda para construir un setup con todas las dependencias instaladas para nuestra aplicacion especifica.

Mostrare los pasos empiricos que hemos seguido para la configuración de esta versión de la Jetson Nano de Waveshare, que nos ha generado muchos quebraderos de cabeza.

(He dejado abiertos los comentarios para que comenten cualquier hallazgo que encuentren y lo documenten)

Tenemos que lograr la instalación de los siguientes paquetes

        -TensorFlow 1.15.5
        -PyTorch v1.10.0
        -torchvision v0.11.0
        -torchaudio v0.10.0
        -onnx 1.11.0
        -CuPy 9.2.0
        -numpy 1.19.5
        -numba 0.53.1
        -OpenCV 4.5.0 (with CUDA)
        -pandas 1.1.5
        -scipy 1.5.4
        -scikit-learn 0.24.2
        -JupyterLab 2.2.9

Opcional:
ROS
Darknet
Deepstream 6.0.1
OpenCV con soporte CUDA
Go Lang para ARM
Julia for ARM

---

Paso 1. Actualizar el sistema

```bash
sudo apt-get update
```

Confirmamos el upgrade

```bash
sudo apt-get upgrade && sudo apt-get install python-pip python3-pip
```

Por defecto el soporte para conectar HDD externos no viene instalado por default, la siguiente instrucción lo hara:

```bash
sudo apt install exfat-fuse exfat-utils
```

Finalmente, removeremos libreoffice y thunderbird:

```bash
sudo apt remove --purge* libreoffice && sudo apt remove --purge* thunderbird
```

```bash
sudo apt autoremove
```

A continuación instalaremos JTOP, similar a HTOP, una herramienta capaz de monitorizar los recursos de nuestro sistema de forma visual.

```bash
sudo pip3 install -U jetson-stats
```

Y eso es todo, finalmente para probar que se está ejecutando correctamente, lo llamaremos con el siguiente comando. (Después de realizar un reinicio)

```bash
sudo reboot
```

Una vez reiniciado esperamos unos minutos y accedemos de nuevo con SSH y verificamos que Jtop se haya instalado.

```bash
jtop
```

---

Instalar TensorFlow

---

Instalar Pytorch

Instalar GO en ARM

Esta parte es completamente opcional, instalar GO y puede ser una guía genérica para instalar este lenguaje de programación que desafortunadamente no tiene soporte con CUDA a pesar de funcionar muy eficientemente.

Lo primero es ubicarse en una carpeta temporal como Downloads:

```bash
sudo reboot
```

```bash
cd Downloads
wget https://go.dev/dl/go1.23.5.linux-arm64.tar.gz
```

Extraemos el paquete:

```bash
sudo tar -C /usr/local -xzf ./go1.23.5.linux-arm64.tar.gz
```

Añade la ruta a go en tu archivo .bashrc.
Bash

```bash
echo 'export PATH="$PATH:/usr/local/go/bin"' >> ~/.bashrc
source ~/.bashrc
```

Para verificar la instalación ejecutamos:

```bash
go version
```

Finalmente se deberá obtener la salida como esta para asegurarnos de que se instaló correctamente:

go version go1.23.5 linux/arm64
