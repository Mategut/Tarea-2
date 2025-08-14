# Tarea 2

## 1. Código ASCII

### Historia
El código **ASCII** (*American Standard Code for Information Interchange*) fue desarrollado en 1963 por el Comité Americano de Estándares (ANSI) como un estándar para representar caracteres en computadoras y dispositivos de comunicación.  
Originalmente usaba 7 bits para representar 128 caracteres, incluyendo letras, números, signos de puntuación y caracteres de control. Posteriormente se amplió a 8 bits (ASCII extendido) para incluir más símbolos.

### Funcionamiento
ASCII asigna a cada carácter un valor numérico. Por ejemplo:  
- Letra `A` → valor decimal **65**  
- Número `0` → valor decimal **48**  

Esto permite que los dispositivos transmitan y procesen texto como datos binarios.

### Descripción breve
ASCII es un sistema de codificación que traduce letras, números y símbolos a valores binarios para que puedan ser almacenados o transmitidos por sistemas digitales.

---

## 2. Pines de conectores DB9 y DB25 del protocolo RS232

### Conector DB9
| Pin | Nombre | Función |
|-----|--------|---------|
| 1   | DCD    | Detección de portadora |
| 2   | RXD    | Recepción de datos |
| 3   | TXD    | Transmisión de datos |
| 4   | DTR    | Terminal listo |
| 5   | GND    | Tierra |
| 6   | DSR    | Equipo listo |
| 7   | RTS    | Solicitud para enviar |
| 8   | CTS    | Listo para enviar |
| 9   | RI     | Indicador de timbre |

### Conector DB25
| Pin | Nombre | Función |
|-----|--------|---------|
| 1   | GND Protector | Tierra chasis |
| 2   | TXD | Transmisión de datos |
| 3   | RXD | Recepción de datos |
| 4   | RTS | Solicitud para enviar |
| 5   | CTS | Listo para enviar |
| 6   | DSR | Equipo listo |
| 7   | GND Señal | Tierra |
| 8   | DCD | Detección de portadora |
| 20  | DTR | Terminal listo |
| 22  | RI | Indicador de timbre |

> Nota: Algunos pines del DB25 no son usados o se reservan para funciones especiales.

---

## 3. Formato del protocolo RS232

El protocolo **RS232** es un estándar para la transmisión serial de datos entre equipos.

**Características principales:**
- Comunicación asíncrona, un bit a la vez.
- Velocidades típicas: 300 bps a 115200 bps.
- Niveles de voltaje:
  - Lógico “1” = -3V a -15V
  - Lógico “0” = +3V a +15V
- Formato de trama típico:
  - 1 bit de inicio (`0`)
  - 5 a 9 bits de datos
  - Bit de paridad (opcional)
  - 1 o 2 bits de parada (`1`)
