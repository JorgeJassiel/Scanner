# Scanner
 Descripción

Este proyecto implementa un escáner de puertos combinado con un capturador de banners (banner grabber) como herramienta educativa para entender conceptos de:
- Sockets de red
- Escaneo de puertos TCP
- Captura de banners de servicios
- Timeouts y manejo de conexiones

Características

- Escanea puertos del 1 al 200 en una IP objetivo
- Detecta puertos abiertos usando `connect_ex()`
- Captura banners de servicios en puertos abiertos
- Timeout configurable de 2 segundos
- Interfaz clara y resultados formateados

Requisitos

- Python 3.x
- Librería socket (incluida en la instalación estándar de Python)

Instalación

1. Clona el repositorio:

git clone https://github.com/tuusuario/port-scanner-banner-grabber.git
cd port-scanner-banner-grabber
(Opcional) Crea un entorno virtual:

python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
Instala las dependencias (si aplica):

pip install -r requirements.txt
 Uso
 
Abre el archivo port_scanner.py y modifica la IP objetivo:
ip_objetivo = '64.76.20.99'  # Cambia por la IP que deseas escanear
Ejecuta el script:

python port_scanner.py

Ejemplo de salida:

Escaneando 64.76.20.99 de puerto 1 a 200...
--------------------------------------------------
Puerto 80: ABIERTO
 Banner: HTTP/1.1 200 OK
--------------------------------------------------
Puerto 443: ABIERTO
 Banner: No disponible
--------------------------------------------------
Escaneo completado
