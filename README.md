# Tren de engranajes revertidos. Tarea2 Grupo3


Este repositorio contiene un código en Python para hacer diversos cálculosx1 en un tren de engranajes revertidos. A continuación se describen las funciones y su funcionalidad:
## Descripción del problema
Se nos presenta un tren compuesto de engranajes revertidos para el cual se nos solicita hacer una serie de cálculos pero cumpliendo ciertas condiciones, la primera de ellas es que la velocidad de salida
del tren debe estar en el rango de 150 a 300 rpm. Además, de tratar de hacer lo más pequeña posible la caja de engranajes.
A paritr de esto, hallamos:
- Números de dientes adecuados para cumplir las condiciones.
- Diámetros de paso.
- Fuerzas y torques en los ejes.
- Velocidades de línea.
- Fuerzas tangenciales, radiales y axiales entre engranajes.
## Funciones

### velocidad_salida(v, n2, n3, n4, n5)

Esta función calcula la velocidad de salida de un tren de engranajes revertidos, dados los siguientes parámetros:
- `v`: Velocidad de entrada en RPM.
- `n2`: Número de dientes del engranaje 2.
- `n3`: Número de dientes del engranaje 3.
- `n4`: Número de dientes del engranaje 4.
- `n5`: Número de dientes del engranaje 5.

La función retorna la velocidad de salida.

### calcular_diametro_paso(num_dientes, m)

Esta función calcula el diámetro de paso de un engranaje, dados los siguientes parámetros:
- `num_dientes`: Número de dientes del engranaje.
- `m`: Módulo de engrane en mm.

La función retorna el diámetro de paso.

### velocidad_engranaje(n2, n3, n4, n5)

Esta función calcula la velocidad de paso de cada engranaje en el tren, dados los siguientes parámetros:
- `n2`: Número de dientes del engranaje 2.
- `n3`: Número de dientes del engranaje 3.
- `n4`: Número de dientes del engranaje 4.
- `n5`: Número de dientes del engranaje 5.

La función retorna un vector con las velocidades angulares de cada engranaje.

### velocidad_linea(w, d)

Esta función calcula la velocidad de línea de un engranaje, dados los siguientes parámetros:
- `w`: Velocidad angular del engranaje en radianes por segundo.
- `d`: Diámetro de paso del engranaje en pulgadas.

La función retorna la velocidad de línea.

### fuerzas_engranajes(p, v)

Esta función calcula la fuerza tangencial de un engranaje, dados los siguientes parámetros:
- `p`: Potencia requerida para transmitir en hp.
- `v`: Velocidad de línea del engranaje en pies por minuto.

La función retorna la fuerza tangencial.

## Uso

1. Ejecuta el programa y se te solicitará ingresar la velocidad de entrada (V en RPM).
2. El programa buscará los números de dientes adecuados para minimizar el tamaño de la caja, cumpliendo con ciertas condiciones.
3. Se calcularán los diámetros de paso, velocidades de línea y fuerzas en los engranajes.
4. Los resultados se mostrarán en la consola y se guardarán en un archivo de Excel llamado "resultados.xlsx".

## Requisitos

El código requiere las siguientes bibliotecas de Python:
- `pandas`
- `numpy`
- `openpyxl`
- `os.path`

Asegurarse de tener estas bibliotecas instaladas antes de ejecutar el código.
