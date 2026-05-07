---
title: Tutorial - CRUD con Ficheros
position: 2
description: Tutorial práctico de persistencia en ficheros binarios.
---

# 🚀 CRUD con Ficheros

Implementaremos un sistema de gestión de alumnos persistido en un fichero binario.

## Prerrequisitos
- Proyecto Maven configurado.
- Conocimientos básicos de Java (Clases y Listas).

## Diagrama de Arquitectura (MVVM)
```mermaid
sequenceDiagram
    participant V as View (Main)
    participant VM as ViewModel
    participant R as Repository
    participant F as FileSystem

    V->>VM: getAlumnos()
    VM->>R: loadData()
    R->>F: readObject()
    F-->>R: List<Alumno>
    R-->>VM: AlumnosState.Success
    VM-->>V: Update UI
```

## Implementación del Repositorio
```java
// src/main/java/repository/AlumnoRepository.java
public class AlumnoRepository {
    // Lógica de lectura/escritura en fichero
}
```
