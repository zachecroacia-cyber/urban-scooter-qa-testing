# Urban Scooter — QA Testing Portfolio

**QA Engineer Final Project | TripleTen | November 2026**

**Author:** Carlos José Sánchez  
**Role:** QA Engineer Trainee  
**Project Status:** Approved  
**Project Type:** Software Quality Assurance — Web, Mobile, API and Database Testing

---

# English

## Project Overview

Urban Scooter is a scooter rental platform used as a practical software testing project during my QA Engineer training at TripleTen.

The project involved analyzing requirements, designing test cases, executing functional tests, validating REST API behavior, testing an Android mobile application, verifying database information, and documenting software defects.

The main objective was to evaluate the application's behavior against its functional requirements, identify deviations, and provide reproducible defect reports supported by testing evidence.

## Key Project Results

| Metric | Result |
|---|---:|
| Recorded test checks | **324** |
| Passed checks | **246** |
| Failed checks | **78** |
| Overall pass rate | **75.9%** |
| Overall failure rate | **24.1%** |
| Testing areas | Web, Data Validation, Mobile and API |

These figures represent recorded test outcomes, not necessarily unique test cases or independent software defects. A single defect may affect multiple checks.

### Test Execution Breakdown

| Testing Activity | Passed | Failed | Total |
|---|---:|---:|---:|
| Web functional testing | 54 | 18 | 72 |
| Input data validation | 28 | 5 | 33 |
| Android mobile testing | 31 | 15 | 46 |
| REST API testing | 133 | 40 | 173 |
| **Total** | **246** | **78** | **324** |

[View Detailed Test Results](test-results/)

## Tools and Technologies

| Category | Tools and Techniques |
|---|---|
| Test Management | Test cases, checklists, test execution |
| Defect Tracking | Jira |
| API Testing | Postman, REST APIs, HTTP, JSON |
| Database Testing | PostgreSQL, SQL |
| Mobile Testing | Android, Android Studio Emulator |
| UI Validation | Figma design comparison |
| Test Design | Equivalence Partitioning, Boundary Value Analysis |
| Documentation | Excel, Markdown, GitHub |
| Testing Approaches | Functional, Positive, Negative and Exploratory Testing |

## Testing Activities

### 1. Requirements Analysis

Reviewed functional requirements to understand the scooter rental workflow and expected application behavior.

Activities included:

- Analyzing the rental and order management processes.
- Identifying required and optional input fields.
- Reviewing validation rules and navigation behavior.
- Creating a functional requirements diagram.
- Identifying ambiguous requirements and areas requiring clarification.

[View Requirements Analysis and Diagram](requirements-analysis/)

### 2. Test Design

Designed test scenarios and documented verification procedures based on the application requirements.

Activities included:

- Creating functional checklists.
- Applying equivalence partitioning.
- Identifying boundary values.
- Designing positive and negative scenarios.
- Preparing expected results.
- Organizing test cases for web, mobile and API validation.

[View Test Design Documentation](test-design/)

[Open Test Design Workbook](test-design/Urban_Scooter_Test_Design.xlsx)

### 3. Web Application Testing

Performed functional verification of the Urban Scooter web application.

Testing included:

- Form field validation.
- Order creation.
- Rental date and period selection.
- Navigation between forms.
- Order status visualization.
- Order cancellation behavior.
- User interface verification.

Tests were performed using Google Chrome and Opera on Windows 11.

**Recorded results:**

- Passed: 54
- Failed: 18
- Total: 72

Input validation was also documented separately:

- Passed: 28
- Failed: 5
- Total: 33

### 4. Android Mobile Testing

Performed functional and user interface testing of the Urban Scooter Android application.

Testing included:

- Order list visualization.
- Order acceptance workflows.
- Interface layout verification.
- Notifications and application behavior.
- Positive and negative test scenarios.
- Comparison of interface elements against Figma designs.

**Test environment:**

- Android 13
- Samsung Galaxy S20 Ultra
- Android Studio Emulator

**Recorded results:**

- Passed: 31
- Failed: 15
- Total: 46

[View Mobile Testing Documentation](mobile-testing/)

### 5. REST API Testing

Used Postman to execute HTTP requests and verify API behavior against documented requirements.

Testing activities included:

- Sending HTTP requests.
- Validating JSON request and response data.
- Checking HTTP status codes.
- Testing order retrieval and cancellation workflows.
- Executing positive and negative scenarios.
- Comparing API responses with expected business rules.
- Verifying order information using PostgreSQL and SQL.

**Recorded results:**

- Passed: 133
- Failed: 40
- Total: 173

[View API Testing Documentation](api-testing/)

### 6. Database Verification

Used PostgreSQL and SQL to inspect order records and compare stored information with API responses.

Activities included:

- Querying order records.
- Verifying tracking numbers.
- Checking order status information.
- Inspecting cancellation and delivery fields.
- Comparing database values with observed application behavior.

Database verification helped support defect investigation and confirm whether application actions produced the expected changes.

### 7. Defect Reporting

Documented software defects using Jira.

Reports included:

- Defect identifier and descriptive title.
- Severity classification.
- Testing environment.
- Steps to reproduce.
- Expected result.
- Actual result.
- Supporting screenshots and technical evidence.

The objective was to provide clear, reproducible reports that could support investigation and correction.

[View Bug Reports](bug-reports/)

## Featured Defect Reports

### KAN-34 — Order Cancellation API Returns Unexpected HTTP 400

**Testing Area:** REST API and Database  
**Severity:** Major (Grave)

The order cancellation endpoint returned `400 Bad Request` with the message `Not enough data for search.` in scenarios where the API documentation specified different expected responses.

**Endpoint:** `PUT /api/v1/orders/cancel`

Expected responses included:

- `200 OK` for an eligible existing order.
- `404 Not Found` for a nonexistent tracking number.
- `409 Conflict` for an order already in processing.

Testing evidence included Postman responses and PostgreSQL verification.

[View KAN-34 Report and Evidence](bug-reports/KAN-34.md)

### KAN-18 — Accept Button Overlaps Metro Station Name

**Testing Area:** Android Mobile UI  
**Severity:** Minor (Menor)

In the All Orders screen, the Accept button overlapped long metro station names on collapsed order cards.

The issue prevented the full station name from being displayed and represented a deviation from the expected interface design.

The report includes reproduction steps, expected and actual behavior, and a supporting screenshot.

[View KAN-18 Report and Evidence](bug-reports/KAN-18.md)

## Repository Structure

| Folder | Description |
|---|---|
| [requirements-analysis/](requirements-analysis/) | Functional requirements analysis and diagrams |
| [test-design/](test-design/) | Test cases, checklists and test design workbook |
| [test-results/](test-results/) | Test execution results and traceability |
| [bug-reports/](bug-reports/) | Documented defects and supporting evidence |
| [api-testing/](api-testing/) | REST API testing and Postman evidence |
| [mobile-testing/](mobile-testing/) | Android functional and UI testing |

## Skills Demonstrated

This project provided practical experience in:

- Translating functional requirements into test scenarios.
- Designing and executing structured manual tests.
- Identifying defects and documenting reproducible issues.
- Validating REST API behavior with Postman.
- Using SQL to support defect investigation.
- Testing Android application functionality and interfaces.
- Comparing expected and actual results.
- Maintaining organized test documentation and evidence.

## Project Outcome

The Urban Scooter final QA project was approved as part of the TripleTen QA Engineer training program.

The project demonstrates practical experience across multiple testing areas and provides documented examples of test design, execution, defect reporting, API validation and database verification.

---

# Español

## Descripción del proyecto

Urban Scooter es una plataforma de alquiler de scooters utilizada como proyecto práctico durante mi formación como QA Engineer en TripleTen.

El proyecto incluyó análisis de requisitos, diseño de casos de prueba, ejecución de pruebas funcionales, validación de API REST, pruebas de una aplicación móvil Android, verificación de información en bases de datos y documentación de defectos.

El objetivo principal fue evaluar el comportamiento de la aplicación frente a sus requisitos funcionales, identificar desviaciones y elaborar informes de errores reproducibles respaldados por evidencias.

## Resultados principales

| Indicador | Resultado |
|---|---:|
| Comprobaciones registradas | **324** |
| Comprobaciones aprobadas | **246** |
| Comprobaciones no aprobadas | **78** |
| Porcentaje de aprobación | **75,9 %** |
| Porcentaje de no aprobación | **24,1 %** |
| Áreas evaluadas | Web, Validación de datos, Móvil y API |

Estas cifras representan resultados de comprobaciones registradas y no necesariamente casos de prueba únicos o defectos independientes. Un mismo defecto puede afectar varias comprobaciones.

### Resultados por actividad

| Actividad | Aprobado | No aprobado | Total |
|---|---:|---:|---:|
| Pruebas funcionales web | 54 | 18 | 72 |
| Validación de datos | 28 | 5 | 33 |
| Pruebas móviles Android | 31 | 15 | 46 |
| Pruebas de API REST | 133 | 40 | 173 |
| **Total** | **246** | **78** | **324** |

[Consultar resultados detallados](test-results/)

## Herramientas y tecnologías

| Categoría | Herramientas y técnicas |
|---|---|
| Gestión de pruebas | Casos de prueba, listas de comprobación y ejecución |
| Gestión de defectos | Jira |
| Pruebas de API | Postman, API REST, HTTP, JSON |
| Bases de datos | PostgreSQL, SQL |
| Pruebas móviles | Android, Android Studio Emulator |
| Validación de interfaz | Comparación con diseños de Figma |
| Diseño de pruebas | Clases de equivalencia y valores límite |
| Documentación | Excel, Markdown, GitHub |
| Enfoques de prueba | Funcionales, positivos, negativos y exploratorios |

## Actividades realizadas

### 1. Análisis de requisitos

Analicé los requisitos funcionales para comprender el proceso de alquiler de scooters y el comportamiento esperado de la aplicación.

Las actividades incluyeron:

- Análisis del proceso de alquiler y gestión de pedidos.
- Identificación de campos obligatorios y opcionales.
- Revisión de reglas de validación y navegación.
- Elaboración de un diagrama de requisitos funcionales.
- Identificación de requisitos ambiguos y zonas grises.

[Consultar análisis de requisitos y diagrama](requirements-analysis/)

### 2. Diseño de pruebas

Diseñé escenarios de prueba y documenté procedimientos de verificación basados en los requisitos de la aplicación.

Las actividades incluyeron:

- Elaboración de listas de comprobación.
- Aplicación de clases de equivalencia.
- Identificación de valores límite.
- Diseño de escenarios positivos y negativos.
- Documentación de resultados esperados.
- Organización de casos de prueba web, móviles y de API.

[Consultar documentación de diseño de pruebas](test-design/)

[Consultar archivo Excel de pruebas](test-design/Urban_Scooter_Test_Design.xlsx)

### 3. Pruebas de aplicación web

Realicé verificaciones funcionales de la aplicación web Urban Scooter.

Las pruebas incluyeron:

- Validación de campos de formularios.
- Creación de pedidos.
- Selección de fechas y períodos de alquiler.
- Navegación entre formularios.
- Visualización de estados de pedidos.
- Comportamiento de cancelación de pedidos.
- Verificación de elementos de interfaz.

Las pruebas se realizaron con Google Chrome y Opera en Windows 11.

**Resultados registrados:**

- Aprobadas: 54
- No aprobadas: 18
- Total: 72

Adicionalmente, se documentaron comprobaciones de validación de datos:

- Aprobadas: 28
- No aprobadas: 5
- Total: 33

### 4. Pruebas móviles Android

Realicé pruebas funcionales y de interfaz de la aplicación Android Urban Scooter.

Las actividades incluyeron:

- Visualización de listas de pedidos.
- Flujos de aceptación de pedidos.
- Verificación de distribución de elementos visuales.
- Notificaciones y comportamiento de la aplicación.
- Escenarios positivos y negativos.
- Comparación de elementos de interfaz con diseños de Figma.

**Entorno de pruebas:**

- Android 13
- Samsung Galaxy S20 Ultra
- Android Studio Emulator

**Resultados registrados:**

- Aprobadas: 31
- No aprobadas: 15
- Total: 46

[Consultar pruebas móviles](mobile-testing/)

### 5. Pruebas de API REST

Utilicé Postman para ejecutar solicitudes HTTP y verificar el comportamiento de la API frente a los requisitos documentados.

Las actividades incluyeron:

- Envío de solicitudes HTTP.
- Validación de solicitudes y respuestas JSON.
- Verificación de códigos de estado HTTP.
- Pruebas de consulta y cancelación de pedidos.
- Ejecución de escenarios positivos y negativos.
- Comparación de respuestas con reglas de negocio.
- Verificación de información mediante PostgreSQL y SQL.

**Resultados registrados:**

- Aprobadas: 133
- No aprobadas: 40
- Total: 173

[Consultar documentación de API](api-testing/)

### 6. Verificación de bases de datos

Utilicé PostgreSQL y SQL para consultar registros de pedidos y comparar la información almacenada con las respuestas de la API.

Las actividades incluyeron:

- Consulta de registros de pedidos.
- Verificación de números de seguimiento.
- Revisión de estados de pedidos.
- Consulta de campos relacionados con cancelación y entrega.
- Comparación de valores de la base de datos con el comportamiento observado.

Estas verificaciones permitieron respaldar la investigación de defectos y comprobar si las acciones de la aplicación producían los cambios esperados.

### 7. Documentación de defectos

Documenté defectos de software mediante Jira.

Los informes incluyeron:

- Identificador y título descriptivo.
- Clasificación de severidad.
- Configuración del entorno.
- Pasos para reproducir.
- Resultado esperado.
- Resultado actual.
- Capturas y evidencias técnicas.

El objetivo fue elaborar informes claros y reproducibles para facilitar la investigación y corrección de defectos.

[Consultar informes de errores](bug-reports/)

## Defectos destacados

### KAN-34 — La API de cancelación devuelve HTTP 400 inesperadamente

**Área:** API REST y base de datos  
**Severidad:** Grave

El endpoint de cancelación devolvió `400 Bad Request` con el mensaje `Not enough data for search.` en escenarios donde la documentación establecía otras respuestas esperadas.

**Endpoint:** `PUT /api/v1/orders/cancel`

Las respuestas esperadas incluían:

- `200 OK` para un pedido existente apto para cancelación.
- `404 Not Found` para un número de seguimiento inexistente.
- `409 Conflict` para un pedido en procesamiento.

Las evidencias incluyeron respuestas de Postman y verificaciones en PostgreSQL.

[Consultar informe KAN-34 y evidencias](bug-reports/KAN-34.md)

### KAN-18 — El botón Aceptar se superpone al nombre de la estación

**Área:** Interfaz móvil Android  
**Severidad:** Menor

En la pantalla «Todos los pedidos», el botón Aceptar se superponía a nombres largos de estaciones de metro cuando las tarjetas estaban contraídas.

El defecto impedía visualizar completamente el nombre de la estación y representaba una diferencia respecto al diseño esperado.

El informe incluye pasos de reproducción, resultados esperados y actuales, y una captura de evidencia.

[Consultar informe KAN-18 y evidencias](bug-reports/KAN-18.md)

## Estructura del repositorio

| Carpeta | Contenido |
|---|---|
| [requirements-analysis/](requirements-analysis/) | Análisis de requisitos y diagramas funcionales |
| [test-design/](test-design/) | Casos de prueba, listas de comprobación y Excel |
| [test-results/](test-results/) | Resultados de ejecución y trazabilidad |
| [bug-reports/](bug-reports/) | Informes de defectos y evidencias |
| [api-testing/](api-testing/) | Pruebas de API REST y evidencias de Postman |
| [mobile-testing/](mobile-testing/) | Pruebas funcionales y de interfaz Android |

## Competencias demostradas

Este proyecto permitió desarrollar experiencia práctica en:

- Transformar requisitos funcionales en escenarios de prueba.
- Diseñar y ejecutar pruebas manuales estructuradas.
- Identificar defectos y documentar problemas reproducibles.
- Validar el comportamiento de API REST con Postman.
- Utilizar SQL para investigar defectos.
- Probar funcionalidades e interfaces Android.
- Comparar resultados esperados y reales.
- Organizar documentación y evidencias de pruebas.

## Resultado del proyecto

El proyecto final de QA Urban Scooter fue aprobado como parte del programa de formación QA Engineer de TripleTen.

El repositorio demuestra experiencia práctica en diferentes áreas de pruebas de software y presenta ejemplos documentados de diseño, ejecución, reporte de defectos, validación de API y verificación de bases de datos.

---

## Education and Certification | Formación y certificación

**QA Engineer — TripleTen**  
Final project approved: November 2026

**Software Engineering Student — Politécnico Grancolombiano**

## Contact | Contacto

**GitHub:** [zachecroacia-cyber](https://github.com/zachecroacia-cyber)

**LinkedIn:** [Carlos Sánchez](https://www.linkedin.com/in/carlos-sanchez-161461172/)

---

*Portfolio project developed for educational and professional demonstration purposes. The repository documents testing activities and evidence from the TripleTen QA training project.*

*Proyecto de portafolio desarrollado con fines educativos y de demostración profesional. El repositorio documenta actividades y evidencias de pruebas realizadas durante la formación QA en TripleTen.*
