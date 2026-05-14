# 🚀 Arquetipo Base de Microservicios (Duoc UC)

Este repositorio contiene la plantilla (Maven Archetype) estandarizada para la creación de nuevos microservicios con Spring Boot y Java 21. Al usar este arquetipo, los nuevos proyectos heredarán automáticamente la estructura de carpetas, configuraciones (pom.xml) y dependencias base necesarias.

## 📋 Requisitos Previos

Asegúrate de tener instalado en tu sistema local:
* **Java Development Kit (JDK) 21**
* **Apache Maven** (correctamente configurado en las variables de entorno `PATH` y `JAVA_HOME`)
* **Git**

---

## 🛠️ 1. Instalación del Arquetipo (Solo la primera vez)

Para poder generar microservicios en tu computadora, primero debes instalar este arquetipo en tu catálogo local de Maven (`.m2`).

1. Clona este repositorio en tu equipo:
   ```bash
   git clone [URL_DE_TU_REPOSITORIO_GIT]

---

## Crear microservicio

1. Instalar en arquetipo:
    mvn clean install

2. Comando de creación de un microservicio:
    mvn --% archetype:generate -DarchetypeCatalog=local -DarchetypeGroupId=cl.duoc -DarchetypeArtifactId=ms-arquetipo-archetype -DarchetypeVersion=0.0.1-SNAPSHOT -DgroupId=cl.duoc -DartifactId=ms-productos -Dversion=1.0.0 -Dpackage=cl.duoc.productos -DinteractiveMode=false

Parámetros a personalizar:
    
Si deseas crear otro servicio (por ejemplo, ms-ventas), solo debes modificar tres variables al final del comando:

* **DartifactId=ms-ventas (El nombre de la carpeta y del proyecto)**

* **Dpackage=cl.duoc.ventas (El paquete base de Java)**

* **Dversion=1.0.0 (La versión inicial de tu nuevo desarrollo, opcional)**

Tip: El prefijo --% es exclusivo de PowerShell para evitar conflictos con los parámetros. Si usas CMD (Símbolo del sistema) o bash en Linux/Mac, omite el --%.
