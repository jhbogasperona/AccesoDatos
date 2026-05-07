---
title: Tutorial - MongoDB con Java
position: 2
description: Conexión y CRUD básico con MongoDB.
---

# 🚀 MongoDB Java Tutorial

Conectaremos nuestra aplicación Java con una base de datos MongoDB local o en la nube (Atlas).

## Driver MongoDB
```xml
<dependency>
    <groupId>org.mongodb</groupId>
    <artifactId>mongodb-driver-sync</artifactId>
    <version>5.x</version>
</dependency>
```

## Operación Insert
```java
Document doc = new Document("name", "Juan")
                .append("especialidad", "DAM");
collection.insertOne(doc);
```
