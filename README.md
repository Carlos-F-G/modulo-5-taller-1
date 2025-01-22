# Proyecto: Hospital Nueva Vida - Consumo de API

## Consumo de API con Axios

### ¿Por qué se usó Axios en lugar de Fetch API?
En este proyecto se eligió Axios en lugar de `fetch` para consumir la API debido a las siguientes ventajas:

1. Manejo Automático de JSON: Axios convierte automáticamente las respuestas en JSON, mientras que con Fetch es necesario llamar `response.json()`.
2. Manejo Simplificado de Errores: Con Fetch, hay que verificar manualmente si la respuesta fue exitosa (`response.ok`), mientras que Axios lanza un error automáticamente si hay fallos.
3. Soporte para Cancelación de Peticiones: Axios permite cancelar peticiones fácilmente usando `CancelToken`.
4. Mayor Compatibilidad con Antiguos Navegadores: Fetch no es compatible con todos los navegadores sin polyfills.

En este proyecto, Axios se utilizó en `DoctorList.jsx` para obtener la lista de doctores desde la API y manejar correctamente los errores en caso de fallos en la conexión.

---

## Requisitos de la Evaluación
Este proyecto cumple con todos los requisitos de la evaluación:

### Implementación de Peticiones con useEffect y useState
- Se utilizó `useEffect` y `useState` para manejar el estado y la carga de datos en `DoctorList.jsx`.
- Los datos se muestran correctamente en la interfaz.

### Uso de Fetch API o Axios para el Consumo de la API
- Se implementó `Axios` para el consumo de la API.
- Se documentó la elección de `Axios` en este `README.md`.
- Se manejaron los errores de manera adecuada en la interfaz.

### Peticiones Basadas en Eventos del Usuario
- Se implementó un botón `Recargar Datos` para permitir al usuario actualizar la información manualmente.

### Manejo de Errores en Peticiones Asíncronas
- Se muestra un mensaje de error cuando la API falla.
- Se agregó un botón `Reintentar` para intentar nuevamente la petición.

### Optimización del Rendimiento al Omitir Efectos en useEffect
- Se optimizó `useEffect` en `DoctorList.jsx` para evitar peticiones innecesarias.
- Se utilizó `useCallback` para mejorar el rendimiento.



## Estructura del Proyecto

src/
 ├── components/
 │   ├── DoctorList.jsx
 │   ├── DoctorCard.jsx
 │   ├── AppointmentForm.jsx
 │   ├── AppointmentList.jsx
 │   ├── Header.jsx
 │   ├── Footer.jsx
 │   ├── ServiceList.jsx
 ├── views/
 │   ├── Home.jsx
 │   ├── Appointments.jsx
 ├── context/
 ├── data/
 ├── App.jsx
 ├── main.jsx


### Carlos Farias Galdames
