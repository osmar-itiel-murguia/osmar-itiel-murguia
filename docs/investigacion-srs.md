# SRS
## ¿Qué es un SRS/ERS y qué problemas evita en un proyecto? 
Especificación de Requisitos de Seguridad por sus siglas “ERS” es un documento técnico que define los requisitos  técnicos y de seguridad para que cumpla con las regulaciones  necesarias, normas aplicables y el estado del sistema.
La documentación clara y precisa es fundamental en el desarrollo de software porque alinea las expectativas entre el cliente y los programadores mediante una única interpretación posible, al tiempo que frena las desviaciones de alcance (scope creep) al exigir negociaciones aparte para cualquier función no contemplada. Asimismo, permite estimar tiempos y presupuestos realistas desde el inicio, evitando sobrecostos y retrasos al detectar errores tempranamente antes de escribir el código, mientras proporciona criterios objetivos para que el equipo de pruebas (QA) valide el producto final y actúa como memoria técnica indispensable para reducir la dependencia de personas clave y facilitar el mantenimiento futuro del sistema.
//Utilice AI en el segundo texto para aumentar de manera rápida la información que escribí. 

## ¿Qué secciones propone el estándar IEEE 830 y qué va en cada una?
-	Introducción
    -	Proporciona un adelanto del documento de especificación de requerimientos en software, por ejemplo:
        -	Propósito: define le propósito y a quien va dirigido
        -	Ámbito: nombra al futuro sistema, explica su función y lo que no hará, describe beneficios, objetivos y metas a futuro.
        -	Definiciones: define los acrónimos, términos y abreviaturas usadas
        -	Referencias: lista de los documentos reverenciadores
        -	Visión general: descriptiva breve de la  organización	
-	Descripción General
    -	Se describen todos aquellos factores que afectan al producto y a sus requerimientos.
        -	Perspectiva del producto: relacionado con el futuro sistema con otros productos
        -	Funciones del producto: un resumen de las funciones principales
        -	Característica de usuario: tipo de usuario a que se dirige
        -	Restricciones: se indica cualquier limitante de hardware o de seguridad entre otras.
        -	Suposiciones y dependencias: cualquier factor que pueda alterar o afectar al sistema.
-	Requerimientos específicos:
    -	Contiene todos los requerimientos con un detallado suficiente para permitir diseñar un sistema que satisfaga dichos requerimientos
        -	Interfaces externas: define los requerimientos que afecten a la interfaz de usuario.
        -	Funciones: especificación de todas las funciones que el sistema llevara a cabo. Algunas de las formas sugeridas por el estándar radican en una jerarquización. Por ejemplo: tipo de usuario, por objetos, por objetivos, por funcionalidad, etc.
        -	Requerimientos de rendimiento: incluye requerimientos relacionados con la carga esperada a soportar por el sistema
        -	Restricciones de diseño: restricciones que afecten al diseño de la aplicación, como estándares internos o limitantes de hardware, etc.
        -	Atributos del sistema: detalles como fiabilidad, mantenibilidad, seguridad, mecanismos de restricción, etc.
-	Apéndices: 
    -	Incluye la información relacionada a la ERS, peo non forme parte, como análisis de costo, restricciones especiales acerca del  lenguaje de  programación.
-	Índice
    -	Se proporciona un índice para poder tener un acceso rápido a la documentación presentada en la ERS.

## ¿Cuáles son las características de un buen requerimiento (no ambiguo, verificable, etc.)? Busca un ejemplo bueno y uno malo. 
•	Malo
    o	Características:
        	Ambiguos
        	Inconsistentes
        	Incorrectos
        	Obsoletos
        	Inviables
    o	Consecuencias con los Requisitos mal estructurados:
        	Difíciles de rastrear
        	Descripción ambigua 
        	Difíciles de verificar 
    o	Ejemplos:
        	El sistema debe tener buena usabilidad: Es vago. No está claro cómo medir la usabilidad. Cada grupo o rol de usuario interactúa con el producto de manera diferente.*citado de la página*
        	El tiempo de respuesta debe ser inferior a 5 segundos: Cinco segundos es una medida objetiva pero no hay contexto. La característica del producto, el escenario, el estado del sistema o la configuración son ejemplos de contexto. *citado de la página*
    o	¿Cómo evitarlo?
        	El desarrollo de requisitos debe involucrar a todas las partes interesadas, incluidos evaluadores y expertos operativos. Los debates deben promover perspectivas diversas. Involucrar a todos los grupos de usuarios. La idea es solucionar los problemas desde el principio. Las inspecciones formales y las revisiones informales deben complementarse entre sí.

-	Bueno 
    -	    Características
        -	Completo
        -	Claro
        -	Factible
        -	Necesario
        -	No ambiguo
        -	Modificable
    -	Elicitación de Requerimientos:
        -	Proceso
            -	Revisar y entender la situación actual
            -	El dominio del problema para comprender el contexto, los problemas y las relaciones desde el punto de vista del usuario.
            -	Identificar las fuentes de información para la identificación de los requisitos. 
            -	El entorno de operación (Observación a los usuarios y funcionalidad típica con el fin proporcionar información para el sistema futuro).
            -	Entorno de la organización.
            -	Hacer uso de diferentes técnicas y herramientas para la identificación de la información.
            -	Observar las estructuras y los patrones, tanto en la operación como en la organización.
    -	Riesgos:
        -	Los clientes no conocen o no tienen claro lo que quieren.
        -	Los clientes no quieren comprometerse a tener un conjunto de requerimientos escritos.
        -	Los clientes insisten en establecer nuevos requerimientos una vez que se han fijado la planificación y el coste.
        -	La comunicación con los clientes es lenta.
    -	Ejemplo:
        -	El sistema de frenado debe detener por completo un vehículo que circula a una velocidad de 100 km/h en una distancia máxima de 40 metros sobre pavimento seco y plano, dentro de los 3 segundos posteriores a que el conductor presione el pedal de freno con una fuerza de 200 Newtons."
//use IA para el ejemplo

## ¿Qué plantillas y herramientas existen para escribir y versionar un SRS?

ISO/IEC/IEEE 29148: Es el estándar internacional para la ingeniería de requisitos en todo el ciclo de vida del sistema y del software. En lugar de describir los métodos de desarrollo de productos, proporciona un marco común para obtener, analizar, documentar, revisar, validar, verificar y gestionar los requisitos de las necesidades iniciales de las partes interesadas a través de la entrega del sistema y el mantenimiento continuo. 

Plantilla de Volere: La plantilla de especificación de requisitos de Volere es un documento estructurado que ayuda a los analistas de negocios y gerentes de proyectos a recopilar y organizar los requisitos del proyecto. 
Esta plantilla le proporciona un formato estructurado para registrar qué debe hacer su software, quién lo usa, qué límites existen y qué problemas podría enfrentar en el futuro. Pero no ofrece un proceso paso a paso para obtener requisitos. 

Plantilla Ágil (Historias de Usuario y Given-When-Then): Los criterios de aceptación Dar / Cuando / Entonces ofrecen un enfoque estructurado para definir el comportamiento esperado de las historias de usuario en el desarrollo ágil. Al dividir los criterios en tres secciones distintas – Dar, Cuándo y Entonces –, los equipos pueden lograr mayor claridad, capacidad de prueba y alineación, lo que en última instancia conduce a un desarrollo de productos más exitoso. Incorporar este formato en su proceso Agile puede ayudar a su equipo a ofrecer software de alta calidad que cumpla con las expectativas de los usuarios. 

Plantilla de Karl Wiegers: Karl Wiegers es uno de los referentes más citados en ingeniería de requisitos. Su enfoque adapta la estructura del estándar IEEE 830 hacia un formato más práctico orientado a reglas de negocio y atributos de calidad.
//aquí si use IA, aunque si avale  la información. Pero no tengo un link web donde avale la información

## REFERENCIAS:
-  CPI,( 20 de agosto de 2026) Especificación de Requisitos de Seguridad (ERS), https://cpi.com.ar/blogs/safety/especificacion-de-requisitos-de-seguridad-ers
-  Ayala Cifuentes, G. P. (2009). Cómo mejorar las metodologías actuales de requerimientos basados en los estándares IEE 830, 1233 y 1362 [Tesis de pregrado, Universidad de las Américas]. Repositorio Institucional.
-  Arvindpdmn,( 07 de febrero de 2026), Requisitos incorrectos, devopedia, https://devopedia.org/bad-requirements
-  Paola Andrea Marmolejo Hurtado(),UNAD, https://repository.unad.edu.co/reproductor-ova/10596_35614/objetivos.html
-  Modern requirements,( 16 de julio de 2026), Explicación de la norma ISO 29148: qué requiere y cómo ayudan los requisitos modernos, https://www.modernrequirements.com/blogs/iso-29148-explained/
-  Modern requirements,(19 de noviembre de 2025), Plantilla de especificación de requisitos de Volere – ¿Qué es y qué necesita saber al respecto?, https://www.modernrequirements.com/blogs/volere-requirements-specification-template/
-  Paradigma Visual,( 15 de septiembre de 2023), Give / When / Then Acceptance Criteria for User Stories in Agile Development, https://guides.visual-paradigm.com/give-when-then-acceptance-criteria-for-user-stories-in-agile-development/
 



# REQUISITOS 

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
