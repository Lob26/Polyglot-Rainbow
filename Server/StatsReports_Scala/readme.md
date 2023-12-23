# Akka HTTP + Slick
# Estructura
```
project-root/
|-- src/
|   |-- main/
|       |-- scala/com/yourcompany/
|                   |-- statistics/
|                       |-- StatisticsService.scala
|                       |-- routes/
|                           |-- StatisticsRoutes.scala
|                       |-- models/
|                           |-- Task.scala
|                       |-- repository/
|                           |-- TaskRepository.scala
|                       |-- Main.scala
|-- resources/
|   |-- application.conf
|-- build.sbt
```
# Modelo
```scala
package com.yourcompany.statistics.models

case class Task(id: Long, title: String, completed: Boolean, executionTime: Option[Long])
```
# To learn
- Akka HTTP
- Slick
- Actores en Akka
- Manejo de JSON en Scala
- Configuracion de Aplicacion
- APIs RESTful en Scala
- Inyeccion de dependencias {Guice}
- Manejo de fechas y horas en Scala {- java.time -scala-time}
- Programacion Funcional en Scala
- OPCIONAL Conceptos de Rendimiento y Escalabilidad
