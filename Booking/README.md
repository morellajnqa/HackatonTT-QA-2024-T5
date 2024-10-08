﻿# Proyecto de Pruebas en la API RESTful

Este proyecto contiene pruebas automatizadas para una API RESTful utilizando la biblioteca `pytest`. Las pruebas están diseñadas para verificar el correcto funcionamiento del endpoint de creación de una nueva reserva de una API de ejemplo.

## Tipos de pruebas:

- **Pruebas de Validación de Datos de Entrada:**
	- Campos Vacíos: Verifican que el sistema maneje adecuadamente campos como firstname o lastname que están vacíos.
	- Datos Inválidos: Comprobar la respuesta del sistema cuando se ingresan caracteres especiales o numéricos en campos que deberían ser texto.


- **Pruebas de Validación de Formato:**
	- Fechas en Formatos Incorrectos: Aseguran que el sistema gestione correctamente formatos de fecha no válidos para checkin y checkout.


- **Pruebas de Validación de Tipos de Datos:**
	- Valores Numéricos Incorrectos: Verifican la respuesta del sistema ante valores no numéricos en campos que deberían ser numéricos, como totalprice.

Cada prueba asegura que la API maneje adecuadamente entradas inválidas y responda con errores apropiados, como un código de estado 400 Bad Request.

## Contenido del Proyecto

- `test_new_booking.py`: Contiene las pruebas automatizadas para el endpoint de reservas. Se ejecutan las pruebas con el comando pytest
- `configuration.py`: Archivo de configuración con URLs y otras constantes.
- `data.py`: Archivo de datos que incluye valores de prueba y configuraciones necesarias para las pruebas.
- `requirements.txt`: Archivo con las dependencias del proyecto.

## Requisitos

Antes de ejecutar las pruebas, asegúrate de tener instalado Python y las siguientes dependencias pytest y request para ejecutar las pruebas.
