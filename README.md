
<div align="center">
  <h1 align="center">
     Challenge LiterAlura
    <br />
    <br />
    <a href="https://github.com/24Kuant/java-challenge-literalura">
      <img src="https://github.com/24Kuant/java-challenge-literalura/blob/main/src/main/resources/fondo.png" alt="♨️ imagen-LiterAlura ⚙️">
    </a>
  </h1>
</div>

# 🧪 Literalura — Challenge: Java + Spring Boot + PostgreSQL

> Aplicación de consola desarrollada como parte de un reto técnico. Consulta libros desde una API pública, los persiste en base de datos y permite consultas locales.

---

## 📌 Objetivo del proyecto

Implementar una aplicación Java que:

- 🔗 Consuma datos de una API externa (Gutendex).
- 📦 Persista información estructurada en PostgreSQL.
- 🧭 Permita consultas dinámicas desde una consola interactiva.
- 🧹 Siga principios de código limpio y diseño orientado a objetos.

---

## 🛠️ Tecnologías y herramientas

- **Lenguaje:** Java 17
- **Framework principal:** Spring Boot
- **Persistencia:** JPA + Hibernate
- **Base de datos:** PostgreSQL
- **Gestión de dependencias:** Maven
- **Modelo de entrada:** Gutendex API (https://gutendex.com)
- **Interfaz de usuario:** Consola interactiva

---

## 🔧 Instalación y ejecución

### 1. Clona el proyecto
```bash
git clone https://github.com/tu-usuario/literalura.git
cd literalura
```

### 2. Configura tu base de datos PostgreSQL
Crea una base de datos llamada `literalura` y ajusta las credenciales en `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/literalura
spring.datasource.username=TU_USUARIO
spring.datasource.password=TU_PASSWORD
spring.jpa.hibernate.ddl-auto=update
```

### 3. Ejecuta el proyecto
```bash
./mvnw spring-boot:run
```

---

## 💻 Funcionalidades implementadas

| Funcionalidad                     | Descripción |
|----------------------------------|-------------|
| 📚 Búsqueda de libros por título | Consulta la API de Gutendex por título |
| 🌍 Importar libros               | Registra libros seleccionados en base de datos |
| 🔎 Consultas locales             | Filtra por idioma, autor, año, etc. |
| 🧹 Interfaz limpia de consola    | Navegación simple mediante menú interactivo |
| 🔄 Actualización automática      | Los datos se actualizan en tiempo real desde la API |

---

## 📌 Estructura del proyecto

```
literalura/
├── model/          → Entidades: Libro, Idioma, Autor, etc.
├── repository/     → Repositorios JPA
├── client/         → Cliente REST para la API Gutendex
├── service/        → Lógica de negocio y persistencia
├── principal/      → Menú interactivo de consola
└── application/    → Punto de entrada (main class)
```

---

## 🧠 Valor técnico entregado

- ✅ Implementación clara de arquitectura en capas.
- ✅ Uso eficiente de REST + Spring WebClient.
- ✅ Persistencia sólida con JPA y PostgreSQL.
- ✅ Separación de responsabilidades.
- ✅ Código fácil de mantener y escalar.
- ✅ Uso de Paginación.

---

## 💡 Posibles extensiones futuras

- Exponer como REST API o app web con Spring MVC.
- Añadir exportación a CSV o PDF.
- Implementar autenticación con Spring Security.

---

## 🙋 Sobre mí

Este reto fue desarrollado por **24Kuant** como ejercicio para reforzar los conocimientos adquiridos en java. **Programa Alura ONE G8 2025**.  
Estoy abierto a feedback y nuevas oportunidades 🚀

---

## 📄 Licencia

MIT © [2025] - Uso libre para fines educativos y profesionales.
