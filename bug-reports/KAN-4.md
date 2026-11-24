
# KAN-4 — Order Remains Accessible After Cancellation | El pedido continúa disponible después de su cancelación

## English

### Bug ID
KAN-4

### Title
Order remains accessible after confirming cancellation through the web interface.

### Severity
Grave (Major)

### Test Environment
- Operating system: Windows 11
- Browsers: Google Chrome and Opera
- Application: Urban Scooter (web version)

### Steps to Reproduce
1. Open the Urban Scooter web application.
2. Create a new order.
3. Check the order status.
4. Click "Cancelar el pedido" (Cancel order).
5. Confirm the cancellation.
6. Click "Okay" or "Bien" in the confirmation message.
7. Search for the order again using its tracking number.
8. Verify the order cancellation status through the API.

### Expected Result
After confirming cancellation, the order should no longer be accessible using its tracking number, according to the specified requirement.

### Actual Result
After confirming cancellation, the order remains accessible using its tracking number. Additionally, the API indicates that the order has not been cancelled (`"cancelled": false`).

### Testing Techniques
- Functional testing
- Web interface validation
- API response verification

---

## Español

### ID del defecto
KAN-4

### Título
El pedido continúa disponible después de confirmar su cancelación desde la interfaz web.

### Severidad
Grave

### Configuración del sistema
- Sistema operativo: Windows 11
- Navegadores: Google Chrome y Opera
- Aplicación: Urban Scooter (versión web)

### Pasos a seguir
1. Abrir la aplicación web Urban Scooter.
2. Crear un pedido nuevo.
3. Consultar el estado del pedido.
4. Pulsar «Cancelar el pedido».
5. Confirmar la cancelación.
6. Pulsar «Okay» o «Bien» en el mensaje de confirmación.
7. Consultar nuevamente el pedido utilizando su número de seguimiento.
8. Verificar el estado de cancelación del pedido mediante la API.

### Resultado esperado
Después de confirmar la cancelación, el pedido no debe poder consultarse nuevamente mediante su número de seguimiento, de acuerdo con el requisito establecido.

### Resultado actual
Después de confirmar la cancelación, el pedido continúa disponible para su consulta mediante el número de seguimiento. Además, la API indica que el pedido no está cancelado (`"cancelled": false`).

### Técnicas de prueba
- Pruebas funcionales
- Validación de interfaz web
- Verificación de respuestas de API
