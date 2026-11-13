# SRS 
## Introducción:
- El propósito de este proyecto es desarrollar un videojuego interactivo centrado en la exploración de cuerpos de agua (ríos, lagos y zonas costeras) para la recolección y venta de residuos sólidos. A través de sus mecánicas de juego, se busca concientizar a los jugadores sobre la grave problemática de la contaminación hídrica, fomentando la educación ambiental y demostrando de manera lúdica el impacto positivo de la limpieza y el reciclaje en los ecosistemas acuáticos.

## Alcance:
- El videojuego está diseñado para ser accesible a todo público (clasificación apta para todas las edades), sin requerir conocimientos previos avanzados en videojuegos ni en gestión ambiental. El producto abarcará desde la navegación y exploración de distintos entornos acuáticos hasta un sistema económico básico de recolección, clasificación y venta de basura para mejorar el equipo del jugador. Su diseño intuitivo garantiza que cualquier persona pueda jugarlo, divertirse y aprender sobre el cuidado del agua de forma sencilla.

## Glosario:
- Cuerpo de agua: Cualquier extensión de agua que se encuentra en la superficie terrestre, como ríos, lagos, lagunas, embalses o mares, donde se desarrolla la exploración del juego.
- Mecánica de juego (Gameplay): Reglas y acciones principales que el jugador realiza dentro del entorno virtual (ej. nadar, sumergirse, recolectar objetos, vender residuos).
- Interfaz de Usuario (UI - User Interface): Conjunto de elementos visuales en pantalla que permiten la comunicación entre el jugador y el sistema (menús, botones, barras de estado, contadores de dinero o basura).
- Experiencia de Usuario (UX - User Experience): Nivel de facilidad, comodidad e intuición que percibe el jugador al interactuar con los controles y pantallas del videojuego.
- HUD (Head-Up Display): Información visual que permanece visible en la pantalla durante la partida activa (como la cantidad de basura recolectada, el nivel de oxígeno o el saldo disponible).
- Pantalla de carga (Loading Screen): Interfaz temporal que se muestra mientras el sistema prepara los gráficos, sonidos y escenarios antes de iniciar una partida o cambiar de nivel.
- NPC (Non-Playable Character): Personaje no jugable controlado por el sistema (por ejemplo, el comerciante o encargado del centro de acopio al que se le vende la basura).
- Activos digitales (Assets): Todos los recursos audiovisuales y técnicos que componen el juego, tales como modelos 3D, sprites 2D, texturas, efectos de sonido y música.

# Descripción general
## Usuarios:
- El usuario principal del sistema es el Jugador, quien interactúa directamente con la aplicación para explorar, recolectar residuos y gestionar sus ganancias. A continuación, se delimita lo que el usuario puede y no puede hacer dentro de la interfaz y el sistema:
## Restricciones:
- Accesibilidad técnica: Al estar dirigido a todo público, el juego debe mantener requisitos de hardware bajos o moderados para ejecutarse fluidamente en equipos convencionales sin necesidad de tarjetas gráficas de gama alta.
- Contenido apropiado: Queda estrictamente prohibido incluir lenguaje ofensivo, violencia o elementos visuales perturbadores; toda la estética y narrativa deben mantenerse aptas para menores de edad.
- Simplicidad en los controles: La curva de aprendizaje no debe superar los primeros minutos de juego, limitando el uso a controles básicos y bien señalizados en pantalla.
- Tiempo y recursos de desarrollo: El alcance gráfico y la cantidad de escenarios estarán limitados al cronograma y presupuesto asignado al equipo de desarrollo.

## Supuestos:
- Disponibilidad de equipo: Se asume que el usuario cuenta con un dispositivo funcional (computadora o dispositivo móvil) con periféricos básicos operativos (teclado/ratón o pantalla táctil) y salida de audio.
- Comprensión intuitiva: Se presupone que los usuarios reconocerán de manera natural los íconos universales de la interfaz (botones de pausa, configuración, inicio y cierre) sin requerir un manual técnico extenso.
- Interés lúdico-educativo: Se asume que la combinación de recompensas dentro del juego (ganar dinero virtual por limpiar) motivará al jugador a completar los objetivos y a reflexionar sobre el mensaje ambiental.
- Entorno de ejecución: Se da por hecho que el sistema operativo del usuario se encuentra actualizado y cumple con los controladores básicos necesarios para ejecutar motores gráficos estándar.

# Requerimientos 
## Funcionales:
- F-1: Gestión de Inventario y Guardado Persistente:
    - El sistema debe registrar, almacenar y persistir de forma automática el progreso del usuario (saldo de dinero virtual, mejoras de equipo adquiridas, porcentaje de limpieza del cuerpo de agua e ítems desbloqueados) al completar eventos clave o cambiar de zona.
      
- F-2: Cálculo y Procesamiento de Recompensas:
    - El sistema debe procesar las transacciones de venta de residuos aplicando una tabla de tarifas predefinidas según la categoría y rareza del material (plástico, metal, orgánico, tóxico), actualizando el saldo del jugador de manera inmediata.
      
-  F-3: Validación de Progresión y Desbloqueo de Niveles:
    - El sistema debe evaluar de forma continua las condiciones de victoria de un escenario (alcanzar obligatoriamente el 95% de limpieza o recolectar la cuota de peso en residuos establecida) para habilitar de manera automática el acceso al siguiente mapa.

- F-4: Mecánica de Recolección de Residuos:
    -  El jugador debe poder utilizar las herramientas iniciales (redes y ganchos) mediante controles de entrada para capturar los residuos flotantes o sumergidos y transferirlos al inventario activo.

-  F-5: Simulación Física del Entorno Acuático:
    - El motor del sistema debe calcular el comportamiento físico básico de los residuos, aplicando parámetros de flotabilidad, detección de colisiones con el entorno y una distribución aleatoria inicial sobre las superficies acuáticas al iniciar el nivel.


## No Funcionales:
- NF-1: Experiencia de Usuario (UX) y Estética Visual:
    -  El diseño de la interfaz debe emplear una paleta de colores coherente y una distribución limpia de elementos que mantengan una alta legibilidad, orientando la experiencia hacia la concientización ambiental del jugador.
      
- NF-2: Usabilidad y Curva de Aprendizaje:
    - El sistema debe incorporar un tutorial interactivo obligatorio en la primera partida que instruya al usuario en los controles de movimiento y recolección en un tiempo máximo de dos minutos.
      
-  NF-3: Accesibilidad y Configuración de Interfaz:
    - El sistema debe incluir un panel de opciones que permita al usuario personalizar de forma independiente el volumen del audio (música de fondo y efectos especiales) y modificar el tamaño de las tipografías en los menús principales.
