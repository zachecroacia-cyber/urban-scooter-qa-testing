
# KAN-1 — Courier Name Truncated in Order Tracking | Nombre del repartidor truncado en el seguimiento

## English

### Bug ID
KAN-1

### Title
Long courier name is truncated in the "Courier is on the way" status.

### Description
When a courier's name is too long to fit on one line, the application truncates it with an ellipsis instead of wrapping the text onto a second line.

### Severity
Minor (Menor)

### Test Environment
- Operating system: Windows 11
- Browsers: Google Chrome and Opera
- Application: Urban Scooter (web version)

### Steps to Reproduce
1. Create a valid order in Urban Scooter.
2. Create a courier with a long name, for example: Carlos Alejandro Sebastian Fernandez.
3. Assign the order to the created courier.
4. Open the web application and check the order status.
5. Locate the message "El repartidor o repartidora está en camino".
6. Observe how the courier's name is displayed.

### Expected Result
The courier's full name should be displayed without truncation, wrapping onto a second line when there is insufficient space on the first line.

### Actual Result
The courier's name is partially displayed with an ellipsis, for example "Ca...", instead of continuing onto a second line.

### Testing Type
- Manual functional testing
- User interface (UI) testing
- Text display validation

---

## Español

### ID del defecto
KAN-1

### Título
El nombre largo del repartidor se trunca en el estado "El repartidor o repartidora está en camino".

### Descripción
Cuando el nombre del repartidor es demasiado largo para mostrarse en una sola línea, el sistema lo trunca con puntos suspensivos en lugar de continuar el texto en una segunda línea.

### Severidad
Menor

### Configuración del sistema
- Sistema operativo: Windows 11
- Navegadores: Google Chrome y Opera
- Aplicación: Urban Scooter (versión web)

### Pasos a seguir
1. Crear un pedido válido en Urban Scooter.
2. Crear un repartidor con un nombre largo, por ejemplo: Carlos Alejandro Sebastian Fernandez.
3. Asignar el pedido al repartidor creado.
4. Abrir la aplicación web y consultar el estado del pedido.
5. Localizar el mensaje «El repartidor o repartidora está en camino».
6. Observar cómo se visualiza el nombre del repartidor.

### Resultado esperado
El nombre completo del repartidor debe mostrarse sin truncarse y continuar en una segunda línea cuando no haya espacio suficiente en la primera.

### Resultado actual
El nombre del repartidor se trunca y se muestra parcialmente con puntos suspensivos, por ejemplo: Ca..., en lugar de continuar en una segunda línea.

### Tipo de prueba
- Pruebas funcionales manuales
- Pruebas de interfaz de usuario (UI)
- Validación de visualización de texto
