---
title: Tutorial - Hibernate con Maven
position: 2
description: Configuración y primer proyecto con Hibernate.
---

# 🚀 Primer Proyecto con Hibernate

Configuraremos Hibernate en un proyecto Maven y realizaremos operaciones CRUD básicas.

## Dependencias (pom.xml)
```xml
<!-- pom.xml -->
<dependency>
    <groupId>org.hibernate</groupId>
    <artifactId>hibernate-core</artifactId>
    <version>6.x</version>
</dependency>
```

## Mapeo de Entidad
```java
@Entity
@Table(name = "usuarios")
public class Usuario {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;
    // ...
}
```
