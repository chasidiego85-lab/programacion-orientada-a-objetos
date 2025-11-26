

# Proyecto GPIO con Raspberry Pi – LEDs y Botones

## 📌 Descripción general

Este proyecto contiene varios programas en Python para controlar **LEDs** y **botones** usando los pines GPIO de una Raspberry Pi. Se incluyen versiones que trabajan con la numeración **BCM** y **BOARD**, además de un **menú principal** para ejecutar todos los módulos.


## 🧰 Requisitos

* Raspberry Pi con GPIO
* Python 3
* Librería RPi.GPIO
* 1 LED
* 1 resistencia de 220Ω – 330Ω
* 1 pulsador (botón)
* Cables de conexión

---

## ⚙️ Instalación de la librería

```bash
sudo apt update
sudo apt install python3-rpi.gpio
```

---

## 🔌 Conexiones del circuito

### ✅ Para LED

* Ánodo (pierna larga) → pin GPIO
* Cátodo → resistencia → GND

### ✅ Para botón

* Un pin del botón → GPIO
* El otro pin → GND

---

## 🟢 Programa: LED con BCM (funledbcm.py)

Hace parpadear un LED usando la numeración **BCM**.

Ejecutar:

```bash
sudo python3 funledbcm.py
```

---

## 🔵 Programa: LED con BOARD (funledboard.py)

Controla el parpadeo de un LED con numeración física de pines.

Ejecutar:

```bash
sudo python3 funledboard.py
```

---

## 🔘 Programa: Botón + LED con BCM (funbutbcm.py)

Enciende o apaga el LED al presionar un botón.

Ejecutar:

```bash
sudo python3 funbutbcm.py
```

---

## 🔘 Programa: Botón + LED con BOARD (funbutboard.py)

Controla el LED con un botón usando numeración BOARD.

Ejecutar:

```bash
sudo python3 funbutboard.py
```

---

## 🧭 Programa principal con menú (modulofun.py)

Permite elegir qué programa ejecutar desde un solo menú.

Ejecutar:

```bash
sudo python3 modulofun.py
```

Opciones del menú:

```
1) LED BCM
2) LED BOARD
3) Botón BCM
4) Botón BOARD
```

---

## 🔀 Diferencia entre BCM y BOARD

* **BCM**: usa la numeración interna del chip.
* **BOARD**: usa la numeración física de los pines de la Raspberry Pi.

---



