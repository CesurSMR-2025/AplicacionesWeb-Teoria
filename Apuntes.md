# Unidad 1: Introducción a las Aplicaciones Web

## 1. ¿Qué es una Aplicación Web?
- Una **aplicación web** es un programa que se ejecuta en un servidor y al que accedemos mediante un **navegador web**.  
- Ejemplos: Gmail, Google Docs, Netflix, Amazon...  
- Se diferencia de una **página web estática** (como un blog sencillo o un curriculum online) en que es **interactiva**: el usuario puede enviar información y recibir respuestas personalizadas.

---

## 2. Página Web vs Aplicación Web
| Característica         | Página Web (Web Estática)        | Aplicación Web (Web Dinámica)      |
|-------------------------|----------------------------------|-------------------------------------|
| Contenido              | Fijo (no cambia mucho)           | Dinámico (va cambiando)            |
| Interactividad         | Muy limitada                     | Alta (formularios, botones, chats) |
| Ejemplo                | Blog personal, web informativa   | Gmail, banca online, e-commerce    |

---

## 3. Frontend y Backend
Las aplicaciones web siguen un modelo **cliente-servidor**, en el que el **cliente** (navegador) y el **servidor** (donde se aloja la aplicación) interactúan entre sí.

Dentro de este modelo, distinguimos dos partes principales:

- **Frontend**:
  - Parte de la aplicación web que se ejecuta en el cliente(navegador).
  - Parte visible para el usuario (interfaz).
  - Al tener que ser compatible con todos los clientes/navegadores las tecnologias estan estandarizadas.
  - Las tecnologías básicas utilizadas son siempre:
    - **HTML**: estructura.
    - **CSS**: estilo (colores, tamaños, fuentes).
    - **JavaScript**: algo de lógica e interactividad.

- **Backend**:
  - Parte de la aplicación web que se ejecuta en el servidor.
  - La mayoría de la lógica de la aplicación ocurre aquí, en el **servidor**. Como por ejemplo procesar datos, acceder a la base de datos o autenticar usuarios.
  - Algunas lenguajes comunes son Java, Python, PHP o JavaScript

---

## 4. Modelo Cliente-Servidor
- **Cliente**: el navegador (Chrome, Firefox, Edge…).
- **Servidor**: ordenador remoto que ejecuta la aplicación web.
- Funcionamiento básico:
  1. El cliente hace una **petición (request)**.
  2. El servidor procesa la petición y devuelve una **respuesta (response)**.
  3. El navegador interpreta el resultado y lo muestra al usuario.

**Esquema:**

<br>
![Frontend-Backend](../images/Frontend-Backend.png)

---

## 5. Servidor Web vs Servidor de Aplicaciones
Aunque a veces se usan indistintamente, hay una diferencia importante entre ambos:

### Servidor Web
- Es un **servidor HTTP** (o  HTTPS).  
- Recibe peticiones HTTP (o HTTPS) del navegador y responde con los recursos web solicitados.
- Su función principal es **enviar el frontend** al cliente: HTML, CSS, JavaScript, imágenes u otros recursos.  
- Cabe aclarar que el frontend no se almacena en el cliente, sino que se descarga desde el servidor web cada vez que se accede a la aplicación.
- Ejemplos de servidores web: **node**, **Apache**, **Nginx**, **Live Server**.

### Servidor de Aplicaciones
- Se encarga de **ejecutar el backend**: la lógica de la aplicación.  
- Procesa datos, realiza cálculos, valida usuarios, se comunica con bases de datos...  
- Genera contenido dinámico y se lo pasa al servidor web para que llegue al navegador.  
- Ejemplos: **Tomcat**, **Node.js (framework)**.

---

## 6. Papel del Navegador
- Interpreta el **código HTML, CSS y JS** en una interfaz visual.
- Envía y recibe información del servidor web.
- Permite ejecutar código JavaScript en el lado del cliente (el navegador).

---

## 7. Protocolos Importantes
- **DNS (Domain Name System)**: sistema que traduce nombres de dominio legibles por humanos (como www.ejemplo.com) en direcciones IP numéricas que los ordenadores utilizan para localizarse en la red.
- **HTTP/HTTPS**: protocolo para la transferencia de páginas web.
  - HTTPS añade seguridad (cifrado con TLS).
- **TLS/SSL**: protocolos para asegurar la comunicación en la web mediante cifrado.
- **SMTP, IMAP, POP3**: protocolos relacionados con el correo electrónico.
- **WebSocket**: permiten comunicación bidireccional en tiempo real (ejemplo: chats).
- **OAuth**: protocolo de autorización para permitir acceso seguro a recursos protegidos.
- **TCP y UDP**: protocolos de transporte que gestionan cómo se envían los datos a través de la red.
- **IP (Internet Protocol)**: protocolo que define cómo se direccionan y envían los paquetes de datos a través de la red.
---

## 8. Arquitectura en Capas de Aplicaciones Web**
Organiza cómo se estructura el **código y la lógica** de una aplicación web.  
Suele dividirse en **3 capas principales**:

- **Capa de Presentación (Frontend)**  
  - Lo que ve el usuario (interfaz).  
  - Tecnologías: HTML, CSS, JavaScript.  

- **Capa de Lógica o Negocio (Backend)**  
  - Procesa la lógica de la aplicación.  
  - Se encarga de cálculos, validaciones, autenticaciones... 

- **Capa de Datos**  
  - Bases de datos donde se guardan los registros.  
  - Ejemplos: MySQL, PostgreSQL, MongoDB, Redis... 

**Esquema típico de 3 capas:**
<br>

![](../images/Tres_capas.png)

Cabe mencionar que no se representa de forma explicita el servidor web, pero este es el que sirve el frontend al navegador para comunicarse con el backend.

---

## 8. Evolución de la Web
- **Web 1.0 o Web Estática** (años 90):
  - Páginas estáticas.
  - Información unidireccional.
  - Ejemplo: primeras webs de periódicos.

- **Web 2.0 o Web Social** (2000s):
  - Contenido dinámico e interactivo.
  - Redes sociales, blogs, wikis.
  - El usuario no solo lee, también **participa**.

- **Web 3.0 o Web Semántica** (actualidad):
  - Información etiquetada con metadatos para ser entendida por máquinas.
  - Contenido personalizado.
  - Integración con inteligencia artificial.
  - Descentralización y blockchain.
  - Aplicaciones descentralizadas.
  - Interoperabilidad entre plataformas (distintas aplicaciones pueden comunicarse y compartir datos).

---

## 9. Herramientas y Lenguajes Utilizados
Es habitual el uso de diversas herramientas y lenguajes en el desarrollo web. Habitualmente se utilizan librerías y frameworks, que son colecciones de código ya escrito, para facilitar el desarrollo.

- **Frontend**:
  - HTML, CSS, JavaScript.
  - Frameworks: React, Angular, Vue.js.
- **Backend**:
  - Lenguajes: Python, Java, PHP, C#, Go.
  - Frameworks: Node.js, Django, Spring, Laravel.
- **Bases de datos**:
  - Relacionales: MySQL, PostgreSQL.
  - No relacionales (NoSQL (Not Only SQL)): MongoDB, Redis.
- **Otros**:
  - Git/GitHub para control de versiones.
  - Docker virtualización ligera y despliegue de aplicaciones.
  - Servidores web: Apache, Nginx, Node.js.

---