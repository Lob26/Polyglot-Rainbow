# Spring

# Estructura
```
project-root/
|-- src/
|   |-- main/
|       |-- java/com/yourcompany/calendar/
|                       |-- CalendarApplication.java
|                       |-- controller/
|                           |-- CalendarController.java
|                       |-- model/
|                           |-- Task.java
|                       |-- service/
|                           |-- CalendarService.java
|                       |-- repository/
|                           |-- TaskRepository.java
|-- resources/
|   |-- application.properties
|-- pom.xml
```
# Modelo
```java
package com.yourcompany.calendar.model;

import javax.persistence.Entity;
import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Id;
import java.util.Date;

import lombok.Getter;
import lombok.Setter;

@Entity @Getter @Setter
public class Task {
    @Id @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    private String title;
    private Date dueDate;

    // Constructors
}
```
# To learn
- Spring Boot
- Controladores en Spring
- Servicios en Spring
- JPA e Hibernate
- Spring Data JPA
- Maven
- Base de Datos Relacional {Configuracion y uso de db en Spring Boot}
- Manejo de Fechas
- APIs RESTful
- OPCIONAL Conceptos de Seguridad
