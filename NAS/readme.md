# Formulario NAS

Este proyecto es un formulario web diseñado para cargar y calcular materiales automáticamente según la tipificación de tareas técnicas en campo.

## 📋 Funcionalidades

- 🧭 **Paso 1: Activar Localización**
  - Solicita la ubicación del dispositivo (latitud y longitud). Permite escaneo y asociación QR.
  - Muestra alerta informativa si no se activa correctamente.

- 🛠 **Paso 2: Selección Técnica**
  - Selección de Caja CTO (modelo y capacidad).
  - Selección del cable a utilizar (FC, MPO).
  - Determina automáticamente los materiales a usar según la combinación elegida.

- 📦 **Paso 3: Visualización de Materiales**
  - Se muestran en tabla los materiales requeridos.
  - Incluye cálculo automático de alambre:  
    `alambre = longitud del cable × 0.014`  
    (leyenda visible junto al campo).
  



