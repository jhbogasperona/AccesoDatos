---
title: Teoría - Conceptos de Persistencia
position: 1
description: Fundamentos sobre la persistencia de datos y sistemas de gestión en entornos Java.
---

# 📚 Conceptos de Persistencia

¡Hola! En esta primera unidad vamos a sentar las bases de lo que significa "hacer que los datos se queden con nosotros". Como futuro desarrollador de DAM, entender la persistencia es vital, ya que la gran mayoría de las aplicaciones reales no sirven de nada si al cerrarlas perdemos toda la información.

## 1. ¿Qué es la Persistencia?

La **persistencia** es la capacidad de una aplicación para que sus datos sobrevivan al ciclo de vida del proceso que los creó. En términos simples: si apagas el ordenador o cierras la app, los datos siguen ahí cuando vuelves.

En el ecosistema Java, esto implica mover datos desde la **memoria volátil** (objetos en la JVM) a un **soporte de almacenamiento estable** (disco duro, base de datos, nube).

## 2. Niveles de Persistencia

No siempre necesitamos una base de datos compleja. Dependiendo de la necesidad, utilizaremos distintos niveles:

*   **Ficheros Planos/Binarios:** Ideal para configuraciones locales o pequeñas cantidades de datos (lo veremos en la UT-2).
*   **Bases de Datos Relacionales (RDBMS):** El estándar de la industria para datos estructurados (MySQL, PostgreSQL). Usaremos JDBC y ORM para interactuar con ellas.
*   **Bases de Datos NoSQL:** Para datos no estructurados o de gran volumen (MongoDB).

## 3. El Desafío: El "Desajuste de Impedancia"

Aquí es donde las cosas se ponen interesantes. Como programadores Java, trabajamos con **objetos** (clases, herencia, colecciones). Sin embargo, las bases de datos relacionales trabajan con **tablas** (filas y columnas). 

:::important Impedance Mismatch
El desajuste de impedancia es la diferencia conceptual entre el modelo orientado a objetos y el modelo relacional. A lo largo del curso aprenderemos herramientas como **Hibernate** para solucionar este problema de forma elegante.
:::

## 4. Evolución de la Persistencia en Java

Para que te ubiques en el tiempo, estas son las tecnologías que han marcado el camino:

1.  **JDBC (Java Database Connectivity):** La base de todo. Código SQL "a pelo" dentro de Java. Potente pero muy repetitivo.
2.  **EJB (Enterprise JavaBeans):** Un intento antiguo y complejo de automatizar la persistencia.
3.  **Hibernate / JPA:** El estándar actual. Mapeamos clases a tablas mediante anotaciones y la librería se encarga de generar el SQL por nosotros.

---

:::tip Próximo Paso
Ahora que entiendes el "qué" y el "por qué", es hora de preparar tu "laboratorio" de desarrollo. ¡Vamos al tutorial de configuración!
:::
