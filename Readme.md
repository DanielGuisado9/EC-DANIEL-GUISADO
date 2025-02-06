
# Ejercicio1
## Análisis del problema
📌 Ejercicio 1: Implementación de una Web del Tiempo con la API de AEMET
🎯 Contexto
El objetivo de este ejercicio es desarrollar una aplicación web del tiempo que permita a los usuarios consultar información meteorológica de diferentes ubicaciones de España, utilizando la API de AEMET (Agencia Estatal de Meteorología).

La interfaz estará inspirada en la web de https://www.eltiempo.es/sevilla.html, proporcionando datos detallados como:
Estado actual del tiempo.
Pronóstico por horas y días.
Mapa meteorológico interactivo.
Índices de calidad del aire y avisos meteorológicos.
⚙️ Requerimientos Funcionales
1️⃣ Consulta del tiempo actual por provincia
Introducción de la ubicación en un buscador (sólo por provincia).
Visualización del estado actual (temperatura, condición climática y velocidad del viento).
Iconos dinámicos según la condición climática (soleado, nublado, lluvia, etc.).
Ejemplo en eltiempo.es
2️⃣ Pronóstico detallado por horas y días
Representación visual de la evolución del tiempo (gráficos de temperatura, precipitaciones, etc.).
Predicción por días con intervalos de mañana (8:00), tarde (15:00) y noche (21:00).
Predicción de mínimo 48 horas, es decir, dos días posterior al actual.
Ejemplo en eltiempo.es

🔗 Documentación de la API de AEMET
Para obtener los datos meteorológicos, se utilizará la API de AEMET, que proporciona información detallada sobre el clima en tiempo real y pronósticos.
Registro y obtención de API Key:
Acceder a AEMET API y obtener la clave de acceso.
Usar POSTMAN para verificar manualmente la llamada al endpoint.
Seguir la documentación de SWAGGER:
Acceder a AEMET API SWAGGER para obtener toda la información relevante a volcar en Postman para verificar el correcto funcionamiento de nuestra petición.
🛠️ Tecnologías Recomendadas
React.js / Angular: Para la implementación de componentes.
Axios / Fetch API: Para las llamadas a la API de AEMET.
Leaflet.js: Para la visualización de mapas meteorológicos.
Chart.js: Para la representación gráfica del pronóstico.


## Diseño de la propuesta de solución del problema


## Pruebas de la resolución del problema


 

# Ejercicio2
## Análisis del problema
📌 Ejercicio 2: Funcionalidades Interactivas por Categoría
El objetivo de este ejercicio es que el alumnado desarrolle funcionalidades interactivas avanzadas basadas en su categoría de proyecto. Se espera que implementen componentes reutilizables que permitan mejorar la experiencia del usuario mediante dashboards, comparadores, rankings, planificadores o encuestas.
Cada categoría del proyecto incluye tres funcionalidades clave, que deben ser desarrolladas siguiendo las buenas prácticas de modularidad y reutilización de código.

📅 Categoría 4: Sitio de Reservas (Restaurantes / Peluquerías)
⚙️ Descripción de las funcionalidades
1️⃣ Planificadores Inteligentes
Sistema de gestión de citas con recordatorios automáticos.
Visualización de disponibilidad en calendario interactivo.
2️⃣ Rankings por Popularidad o Actividad
Clasificación de los restaurantes/servicios más reservados por ubicación.
Ranking basado en reseñas y puntuaciones de clientes.
3️⃣ Sistemas de Encuestas o Votaciones
Encuestas de satisfacción post-reserva.
Sección de opiniones de clientes sobre la calidad del servicio.





## Diseño de la propuesta de solución del problema
- He hecho uso de módulos propiamentes de angular como ngfor,ngmodel,ngif,etc.Algunos no me los aceptaba así que tenía que importar módulos especiales como CommonModule y ReactiveFormsModule.
- Inicio de Sesión: Permite a los usuarios ingresar con correo y contraseña. Incluye opciones de "Recordarme" y enlaces para registrarse o recuperar la contraseña.
- Registro: Formulario para crear una nueva cuenta con nombre, correo y contraseña. Incluye validaciones básicas.
- Recuperación de Contraseña: Envía un enlace de recuperación al correo ingresado si está registrado. Muestra mensajes claros en caso de éxito o error.
- Habrá dos servicios,en los que en uno consumirán todos los componentes de lo que es la página principal y la pestaña de reservas y el otro servicio lo consumirán los componentes de registrar usuarios,iniciar sesión y recuperar contraseña.En este caso consume de AuthServer
 

## Pruebas de la resolución del problema
- ✅ Prueba 1: Planificador de reservas
Seleccionar una fecha y hora de reserva.
Verificar que el sistema muestra la disponibilidad adecuada y permite la confirmación.


 ![gif](./recursos/Prueba_Login.gif)

- ❌ Prueba 2: Error en Inicio de Sesión
Ingresar credenciales incorrectas.
Verificar que aparece una notificación de error.


![gif](./recursos/Prueba2_Login.gif)

- 🆕 Prueba 3: Registro con Validaciones
Ingresar datos inválidos (correo incorrecto, contraseñas que no coinciden).
Verificar que se muestran mensajes de error en tiempo real.
Corregir los datos y completar el registro.
Verificar notificación de éxito y redirección al login.


 ![gif](./recursos/Prueba_Registro.gif)

- 🔐 Prueba 4: Recuperación de Contraseña
Ingresar un correo registrado.
Verificar que se envía un aviso de correo de recuperación enviado.
Probar con un correo no registrado y verificar el mensaje de error.


 ![gif](./recursos/Prueba_RecuperarContraseña.gif)





