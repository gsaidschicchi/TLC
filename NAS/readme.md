# Formulario NAS

Este proyecto es un formulario web diseñado para permitir completar tareas de campo,cargar, y calcular materiales automáticamente según la tipificación de tareas técnicas.
Permite la supervisión de obras remota y da trazabilidad a la construcción de obras por parte de las EC.
## 📋 Funcionalidades

---

- 🧭 **Paso 1: Activar Localización**
  - Solicita la ubicación del dispositivo (latitud y longitud). Permite escaneo y asociación QR.
  - Muestra alerta informativa si no se activa correctamente.

---

- 🛠 **Paso 2: Selección Técnica**
  - Selección de Caja CTO (modelo y capacidad).
  - Selección del cable a utilizar (FC, MPO).
  - Determina automáticamente los materiales a usar según la combinación elegida.

---

- 📦 **Paso 3: Visualización de Materiales**
  - Se muestran en tabla los materiales requeridos.
  - Incluye cálculo automático de alambre:  
    `alambre = longitud del cable × 0.014`

---





