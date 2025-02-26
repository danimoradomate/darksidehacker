---
layout: page
title: Jetson Nano for Computer Vision
description: Course Page
img: assets/img/jetson.png
importance: 1
category: work
giscus_comments: true
---

## Bienvenidos a todos

Esta sección concentrare toda la información que vayamos generando en el curso. Al final de esta pagina he habilitado una sección de comentarios por si desean contribuir o reportar algun error. Solo compartiendo, colaborando y haciendo es como creo que nuestro aprendizaje puede mejorar.

---

### Instalación de JetPack para Jetson Nano

<ul>
    <li><a href="https://www.waveshare.com/wiki/JETSON-NANO-DEV-KIT-MANUAL">JETSON-NANO-DEV-KIT</a> </li>
    <li><a href="https://jetsonhacks.com/">Jetson Hacks</a></li>
</ul>

### Repositorios que revisaremos

<ul>
<li><a href="https://github.com/dusty-nv/jetson-inference">Jetson Inference</a></li>
<li><a href="https://github.com/dusty-nv/jetson-utils">Jetson Utils</a></li>
<li><a href="https://github.com/dusty-nv/ros_deep_learning">ROS</a></li>
</ul>
### Material de apoyo 
<ul>
<li><a href="https://docs.docker.com/">Docker Documentation</a></li>
<li><a href="https://developer.nvidia.com/embedded/dlc/Jetson_Nano_Developer_Kit_User_Guide">Jetson User Guide</a></li>
</ul>

Nota: Esta pagina se estara actualizando constantemente.

#### _Semana 1: Introducción a la Jetson Nano y preparación del entorno_

- Instalación del sistema operativo y configuración básica.
- Generar claves <a href="https://gusman.me/blog/2025/code/">SSH </a>
- Instalar <a href="https://knowledge.broadcom.com/external/article/344595/downloading-and-installing-vmware-workst.html"> VMWare WorkStation Pro </a>
- Instalar <a href="https://releases.ubuntu.com/18.04/">Ubuntu 18 24.04</a>
- Instalar <a href="https://developer.nvidia.com/sdk-manager">SDK Manager</a>
  Nota: Solo instalar el S.O. de la Jetson Nano en SDKManager, sin complementos.
  En este enlace he colocado una guia de dependencias para instalar una vez instalado JetPack
- Instalar <a href="https://gusman.me/blog/2025/setting_up_jetson_nano/">Setting Up Jetson Nano</a>

---

#### _Semana 2: Fundamentos de Programación Orientada a Objetos (POO) en C++_

- Introduccion a C++
- <a href="https://gusman.me/blog/2025/cmake/">Setting Up CMake </a>(Configuracion de proyectos en C++)
- Clases y objetos en C++.

---

#### _Semana 3: Manejo de memoria y apuntadores en C++_

- Conceptos de apuntadores y memoria dinámica.
- Ejercicios prácticos.

---

#### _Semana 4: Introducción a Jetson Inference y configuración del proyecto_

- Instalación y configuración de Jetson Inference.
- Primeros pasos con Jetson Inference en C++.

---

#### _Semana 5: Procesamiento de imágenes y videos con Jetson Inference_

- Captura y procesamiento de imágenes.
- Uso de videoSource y videoOutput.
- Integración con OpenCV.

---

#### _Semana 6: Clasificación de imágenes con Jetson Inference_

- Modelos preentrenados para clasificación.
- Uso de imageNet para clasificación.
- Ejercicio práctico de clasificación en tiempo real.

---

#### _Semana 7: Detección de objetos con Jetson Inference_

- Modelos preentrenados para detección de objetos.
- Uso de detectNet para detección.
- Ejercicio práctico de detección en tiempo real.

---

#### _Semana 8: Optimización y rendimiento_

- Buenas prácticas de optimización de código.
- Uso de CUDA y TensorRT
- Ejercicios prácticos de optimización.

---

#### _Semana 9_:

Preprocesamiento del dataset
Entrenar redes neuronales convolucionales en una GPU.

---

#### _Semana 10: Final_

Medidas de rendimiento de los clasificadores para vision por computadora
