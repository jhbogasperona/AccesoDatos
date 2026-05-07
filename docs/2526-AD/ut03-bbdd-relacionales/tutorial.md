---
title: Tutorial - JDBC Repository
position: 2
description: Implementación del patrón Repository con JDBC.
---

# 🏗️ JDBC Repository Pattern

Aprenderemos a separar la lógica de negocio de la persistencia usando un Repositorio JDBC.

## Arquitectura
```mermaid
graph LR
    A[View] --> B[ViewModel]
    B --> C[Repository Interface]
    C --> D[JDBC Implementation]
    D --> E[(MySQL)]
```

## Ejemplo de Conexión
```java
// src/main/java/database/DatabaseManager.java
public class DatabaseManager {
    // Configuración de la conexión con strings.xml
}
```
