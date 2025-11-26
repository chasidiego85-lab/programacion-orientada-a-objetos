# Proyecto: Robots con Python, Raspberry Pi y Telegram Bot

## 📌 Descripción

Este proyecto implementa diferentes tipos de robots utilizando Python, Programación Orientada a Objetos (POO), control de hardware con Raspberry Pi (GPIO), sensor de temperatura y humedad (DHT11), y comunicación mediante un Bot de Telegram.

El sistema incluye:

* Clases básicas para comprender la creación de objetos.
* Simulación de robots con herencia.
* Registro de interacciones en archivos de texto.
* Control remoto de robots mediante comandos enviados por Telegram.

---

## 🧩 Estructura del proyecto

### 1. Clases básicas

Se crean clases simples (`MiClase`, `fieles`) para practicar el concepto de instanciación de objetos.

### 2. Clase Robot (versión inicial)

Se define una clase `Robot` con atributos básicos y métodos de movimiento vacíos para estructura base.

### 3. Robots con herencia

Se implementan distintos tipos de robots mediante herencia:

* `robot_exp`: Robot explorador
* `robot_obr`: Robot obrero
* `Robot_medico`: Robot médico

### 4. Simulación

Función que prueba el funcionamiento de los robots:

* Encendido
* Ejecución de tareas
* Apagado

### 5. Registro de eventos

Se implementa un sistema de logs que guarda:

* Hora del evento
* Origen (Usuario/Bot)
* Mensaje enviado

Los registros se guardan automáticamente en un archivo `.txt`.

### 6. Control por Telegram

Se agregan comandos usando un bot de Telegram:

* `hola`: muestra mensaje de bienvenida
* `menu`: muestra opciones
* `a`: inicia Robot LED
* `b`: inicia Robot Explorador
* `c`: inicia Robot Médico

### 7. Control de hardware con Raspberry Pi

Se integran:

* GPIO para control de LEDs
* Botón físico
* Sensor DHT11 para temperatura

### 8. Integración con Telegram Bot

Se utiliza la librería `telepot` para enviar y recibir mensajes desde Telegram.

---

## 📝 Convención de commits usada

Este proyecto utiliza la convención **Conventional Commits**.

Ejemplos:

```
feat: add basic classes and object instances
feat: add Robot class with movement methods
feat: implement robot inheritance for explorer, worker and medical robots
feat: add robot simulation function
chore: add delay and console clear after simulation
feat: add text file logging system
feat: implement Telegram command handler for robot control
feat: integrate GPIO LED and DHT11 sensor support
feat: add Telegram bot messaging interface
```

---

## 🛠️ Requisitos

* Python 3.x
* Raspberry Pi (opcional para pruebas físicas)
* Librerías:

  * `RPi.GPIO`
  * `adafruit_dht`
  * `telepot`

---

## 🚀 Cómo ejecutar

1. Clonar el repositorio:

```
git clone <URL_DEL_REPOSITORIO>
```

2. Instalar dependencias:

```
pip install telepot adafruit-circuitpython-dht RPi.GPIO
```

3. Ejecutar el programa:

```
python main.py
```

---


Diego Mauricio (Alias El Chasi)

