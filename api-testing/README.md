# API Testing | Pruebas de API

## English

### Project Overview
REST API testing performed as part of the Urban Scooter QA training project at TripleTen.

### Testing Scope
- HTTP requests using Postman.
- JSON request and response validation.
- Verification of HTTP status codes.
- Order creation, retrieval, and cancellation workflows.
- Positive and negative test scenarios.
- Database verification using PostgreSQL.

### Tools and Technologies
- Postman
- REST APIs
- HTTP and JSON
- PostgreSQL
- SQL

### Documented Defect: KAN-34
**Endpoint:** `PUT /api/v1/orders/cancel`

During testing, the API returned `400 Bad Request` with the message `Not enough data for search.` when cancellation requests were submitted for different order scenarios.

The observed behavior did not match the documented expected responses:
- Existing eligible order: 200 OK.
- Nonexistent tracking number: 404 Not Found.
- Order already in processing: 409 Conflict.

The defect was documented in Jira and reviewed as part of the approved TripleTen project.

### Evidence
Screenshots of Postman responses and database verification will be added to this folder.

---

## Español

### Descripción del proyecto
Pruebas de API REST realizadas como parte del proyecto de formación QA Urban Scooter en TripleTen.

### Alcance de las pruebas
- Solicitudes HTTP mediante Postman.
- Validación de solicitudes y respuestas JSON.
- Verificación de códigos de estado HTTP.
- Flujos de creación, consulta y cancelación de pedidos.
- Escenarios de prueba positivos y negativos.
- Verificación de datos mediante PostgreSQL.

### Herramientas y tecnologías
- Postman
- API REST
- HTTP y JSON
- PostgreSQL
- SQL

### Defecto documentado: KAN-34
**Endpoint:** `PUT /api/v1/orders/cancel`

Durante las pruebas, la API devolvió `400 Bad Request` con el mensaje `Not enough data for search.` al intentar cancelar pedidos en diferentes escenarios.

Este comportamiento no coincidió con las respuestas esperadas según la documentación:
- Pedido existente y apto para cancelación: 200 OK.
- Número de seguimiento inexistente: 404 Not Found.
- Pedido en procesamiento: 409 Conflict.

El defecto fue documentado en Jira y revisado como parte del proyecto aprobado por TripleTen.

### Evidence | Evidencias

**English**

Defect KAN-34 was documented during API testing of the endpoint `PUT /api/v1/orders/cancel`.

[View KAN-34 defect report and supporting evidence](https://github.com/zachecroacia-cyber/urban-scooter-qa-testing/blob/main/bug-reports/KAN-34.md)

**Español**

El defecto KAN-34 fue documentado durante las pruebas de API del endpoint `PUT /api/v1/orders/cancel`.

[Consultar reporte KAN-34 y evidencias asociadas](https://github.com/zachecroacia-cyber/urban-scooter-qa-testing/blob/main/bug-reports/KAN-34.md)

