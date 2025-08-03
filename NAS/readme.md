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

## 🧱 MATERIALES

Esta parte del documento detalla los materiales requeridos para la instalación de cajas NAS, organizados por categorías.

---

### 1. Puesta a tierra

| Artículo | Descripción | Cantidad |
| --- | --- | --- |
| 031044 | Jabalina para puesta a tierra de 1/2" | 1 |
| 031092 | Alambre de cobre para PAT por Kg. | 1 |
| 032037 | Tomacable bronceado para jabalina de 1/2" | 1 |
| 032047 | Cubrejabalina | 1 |
| 031011 | Clavo U para jabalina | 12 |
| 031019 | Prensacable de acero de 1/4 para jabalina/linga | 2 |
| 033042 | Hebilla de acero inoxidable AISI 304 para fleje 033041 | 3 |
| 033041 | Fleje de acero inoxidable AISI 304 | 3 |

---

### 2. Cajas CDO / CTO

Permite seleccionar entre alguna de estas dos opciones (HUB o SUB)

| Artículo | Descripción | Cantidad |
| --- | --- | --- |
| 034129 | Caja Distribución Óptica CDO - SP 1x8 - 1 Ent MPO Female 6FO 12 Sal SC/APC 1FO | 1 |
| 034130 | Caja de empalme HUAWEI FTTH SUB 1+8 14260682 | 1 |

---

### 3. Cables de interconexión entre cajas

Dependiendo de la selección de la caja (HUB o SUB), se presentarán los cables disponibles.

**3.a. Caja HUB**

| Artículo | Descripción | Cantidad |
| --- | --- | --- |
| 030058 | Cable distribucion 6FO 50 m. Un extremo preconectorizado MPO. (14136997) | 1 |
| 030055 | Cable distribucion 6FO 100 m. Un extremo preconectorizado MPO. (14136997-004) | 1 |
| 030056 | Cable distribucion 6FO 150 m. Un extremo preconectorizado MPO. (14136997-005) | 1 |
| 030057 | Cable distribucion 6FO 200 m. Un extremo preconectorizado MPO. (14136997-006) | 1 |

**3.b. Caja SUB**

| Artículo | Descripción | Cantidad |
| --- | --- | --- |
| 030067 | Cable interconexion ADSS 1FO 50 m/5 mm. Fastconnect SC/APC. (14137733-001) | 1 |
| 030068 | Cable interconexion ADSS 1FO 100 m/5 mm. Fastconnect SC/APC. (14137733-003) | 1 |
| 030069 | Cable interconexion ADSS 1FO 150 m/5 mm. Fastconnect SC/APC. (14137733-004) | 1 |
| 030070 | Cable interconexion ADSS 1FO 200 m/5 mm. Fastconnect SC/APC. (14137733-009) | 1 |

