# Forex-Alert 
Proyecto CC: Sistema de alarmas de mercado de divisas Forex
***
## Descripción del proyecto 
El objetivo de este proyecto es desarrollar un servicio en la nube que permita a inversionistas del mercado Forex crear alertas sobre umbrales importantes de cambios en los valores de las monedas. Entre las funcionalidades de este producto se encuentran:
1. Alta de usuarios
2. Creación de alarmas de mercado Forex
4. Desactivar alarmas
5. Notificación a usuarios de acuerdo a alarmas activas.

## Alcance
El alcance del proyecto es solo la construcción del backend

## Arquitectura
La aplicación será desarrollada siguiendo una arquitectura de microservicios que utilizaran API REST en su comunicación. Se construirá un microservicio para cada una de las funcionalidades ya expuestas.
La información del valor de las divisas se obtendrá consultando de manera recurrente (tiempo a definir) la API REST de alphavantage.

## Lenguaje
Se utilizaría RUBY en el desarrollo de los servicios por la facilidad de desarrollo y la gran cantidad de material de apoyo que hay en la red. Esto se confirmará a medida que avance el curso

## Base de datos
Para el almacenamiento se utilizará una BD NoSQL como mongoDB. Esto para obtener mejores tiempos de respuesta (Esto se confirmará a medida que avance el curso)




