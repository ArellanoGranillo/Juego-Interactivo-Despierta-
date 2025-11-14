🌙 Juego de Decisiones — “El Despertar”

Este proyecto es una aplicación web desarrollada con Java Servlets, JSP, Tomcat 11 y JDK 17.
El jugador despierta dentro de un sueño misterioso y solo podrá despertar si toma las decisiones correctas. Cada error lo regresa al inicio, mientras que cada triunfo se registra en un sistema interno de estadísticas que se conserva durante la ejecución del servidor.

El proyecto incluye un sistema completo de tests unitarios con JUnit y Mockito, asegurando que la lógica del juego y el conteo de estadísticas funcionen correctamente.

🎮 ¿Cómo funciona el juego?

El jugador escribe su nombre y comienza una aventura basada en decisiones.

Cada “escena” o desafío se gestiona con Servlets.

Si escoge mal, pierde y vuelve al menú principal.

Si escoge bien, avanza.

Al final del juego se registra si el jugador:

Ganó

Perdió

El servidor guarda las partidas que pierde o gana el jugador.

🧠 Características principales

✔ Juego interactivo basado en decisiones
✔ Flujo controlado mediante Servlets (GET/POST)
✔ Manejo de sesiones por jugador
✔ Compatible con Tomcat 11 + JDK 17
✔ Suite de pruebas unitarias (JUnit + Mockito)

🧪 Pruebas Unitarias Incluidas

El proyecto contiene una suite diseñada para validar:

✔ Registro correcto de victorias

Verifica que si el jugador acepta el desafío final, su contador de victorias aumenta.

✔ Manejo del caso “jugador no registrado”

Si el jugador no tiene sesión, se redirige a nombre.jsp.

✔ Elección de perder

Si el jugador rechaza el desafío, se redirige a perder.jsp.

✔ Elección correcta

Si responde afirmativamente, continúa hacia index.jsp.

Estas pruebas simulan completamente un entorno web usando:

HttpServletRequest

HttpServletResponse

HttpSession

ServletContext

ServletConfig

🚀 Tecnologías usadas

Java 17

Jakarta EE (Servlets 6)

Tomcat 11

JSP + JSTL

JUnit 5

Mockito

Maven

▶️ Cómo ejecutar

Instalar Tomcat 11

🌙 Juego de Decisiones — “El Despertar”

Este proyecto es una aplicación web desarrollada con Java Servlets, JSP, Tomcat 11 y JDK 17.
El jugador despierta dentro de un sueño misterioso y solo podrá despertar si toma las decisiones correctas. Cada error lo regresa al inicio, mientras que cada triunfo se registra en un sistema interno de estadísticas que se conserva durante la ejecución del servidor.

El proyecto incluye un sistema completo de tests unitarios con JUnit y Mockito, asegurando que la lógica del juego y el conteo de estadísticas funcionen correctamente.

🎮 ¿Cómo funciona el juego?

El jugador escribe su nombre y comienza una aventura basada en decisiones.

Cada “escena” o desafío se gestiona con Servlets.

Si escoge mal, pierde y vuelve al menú principal.

Si escoge bien, avanza.

Al final del juego se registra si el jugador:

Ganó

Perdió

El servidor guarda sus estadísticas en un Map<String, int[]>, donde:

int[0] = derrotas

int[1] = victorias

🧠 Características principales

✔ Juego interactivo basado en decisiones
✔ Flujo controlado mediante Servlets (GET/POST)
✔ Estadísticas globales almacenadas en ServletContext
✔ Manejo de sesiones por jugador
✔ JSPs para las vistas
✔ Compatible con Tomcat 11 + JDK 17
✔ Suite de pruebas unitarias (JUnit + Mockito)

🧪 Pruebas Unitarias Incluidas

El proyecto contiene una suite diseñada para validar:

✔ Registro correcto de victorias

Verifica que si el jugador acepta el desafío final, su contador de victorias aumenta.

✔ Manejo del caso “jugador no registrado”

Si el jugador no tiene sesión, se redirige a nombre.jsp.

✔ Elección de perder

Si el jugador rechaza el desafío, se redirige a perder.jsp.

✔ Elección correcta

Si responde afirmativamente, continúa hacia index.jsp.

Estas pruebas simulan completamente un entorno web usando:

HttpServletRequest

HttpServletResponse

HttpSession

ServletContext

ServletConfig

🚀 Tecnologías usadas

Java 17

Jakarta EE (Servlets 6)

Tomcat 11

JSP + JSTL

JUnit 5

Mockito

Maven

▶️ Cómo ejecutar

Instalar Tomcat 11

Crear artefacto .war o usar IntelliJ > "Run on Tomcat"

Abrir en navegador:
http://localhost:8080/proyectoKaren3_war/
