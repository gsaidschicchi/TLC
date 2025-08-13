# Modificación de Tipificación TAF

En lugar de trabajar con los elementos **cable** y generar múltiples tareas (una por cada caja H y S del proyecto), se trabajará con una **única TAF** que generará un contenedor con los cables del proyecto.  

Para evitar replicar las fotos solicitadas por los elementos *apoyo* que pueden compartir múltiples cables —lo que incrementa la carga operativa para la EC—, en la tarea se presentará **la totalidad de los apoyos** por los que pasan cables **FC** y **MPO**.

El técnico seleccionará el apoyo en el que se encuentra y completará la información correspondiente en el formulario TAF.

---

## Manejo de secuenciales de FO de distribución

Para no perjudicar la operatividad de la cuadrilla al completar el form, se incorporará la planilla de secuenciales durante la etapa de supervisión de obras de la tarea TAF del proyecto.  
En caso de que no se agregue en esta instancia, se podrá agregar posteriormente editando la tarea en Viena.

---

## Consumo de materiales

En función de si un cable es **pasante** o **terminal** en un apoyo, se presentará el consumo de materiales correspondiente:

- 1 morseto de 1 bulón → cable pasante  
- 2 morsetos de 1 bulón → cable terminal  

El **alambre de devanar** se calculará en función de la longitud parcial entre apoyos que compartan uno o más cables.

**Ejemplo:**
Vano A-B = **50 metros**  
Pasan **4 cables**  

Consumo:  
50m * 0.014kg/m = 0.7kg

*Nota:* ver **precintos** y **separadores de linga**.

---

## Pregunta clave

> **¿Qué sucede si el técnico no puede completar la totalidad de apoyos del formulario al finalizar la jornada laboral?**

---

## Posibles alternativas

### 1. Guardado parcial
Permitir que el técnico guarde el formulario con los apoyos ya completados y lo retome más tarde.

### 2. División automática
Si quedan apoyos pendientes, generar automáticamente una nueva tarea con los restantes.

### 3. Bloqueo de cierre
No permitir cerrar la tarea hasta que todos los apoyos estén cargados.

### 4. SubProceso para suspensión de tareas desde el área de despacho o técnico de calle

