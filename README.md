# Forex-Alert 
Proyecto CC: Sistema de cálculo de tendencias en el mercado de divisas
***
## Descripción del proyecto 
El objetivo de este proyecto es desarrollar un servicio en la nube que permita a inversionistas del mercado Forex consultar por las tendencias de los valores de las monedas en distintos periodos de tiempo. Entre las funcionalidades de este producto se encuentran:
1. Alta de usuarios: La aplicación permitirá crear, editar y eliminar cuentas de usuario.
2. Creación de base de datos de valores de divisas: El sistema contará con una BD actualizada con las tasas de cambio para los principales pares de divisas
3. Interfaz de consulta de tendencia: El sistema responderá a consultas de tendencias de las divisas para distintos períodos de tiempo. 

## Alcance
El alcance del proyecto es solo la construcción del backend del sistema. La información de las tasas de cambio se obtendrá de la API REST expuesta por Free Forex API que ofrece información actualizada cada 15 segundos.

## Arquitectura
La aplicación será desarrollada siguiendo una arquitectura de [microservicios](https://en.wikipedia.org/wiki/Microservices). Las peticiones de clientes serán recibidas por un API Gateway REST utilizando JSON. Dicho Gateway enrutará las peticiones al microservicio que corresponda. 
La información del valor de las divisas se obtendrá consultando de manera recurrente la API REST de [Free Forex API](https://www.freeforexapi.com/) de manera agendada cada 15 segundos.
![Arquitectura](docs/image/arquitectura.png "Arquitectura")

## Lenguaje
Se utilizaría RUBY en el desarrollo de los servicios por la facilidad de desarrollo y la gran cantidad de material de apoyo que hay en la red. Esto se confirmará a medida que avance el curso

## Base de datos
Para el almacenamiento se utilizará una BD NoSQL como mongoDB independiente pada cada microservicio. Esto para obtener mejores tiempos de respuesta (Esto se confirmará a medida que avance el curso).






