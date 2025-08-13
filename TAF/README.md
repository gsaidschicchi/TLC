# Modificación de Tipificación TAF

En lugar de trabajar con los elementos **cable** y generar múltiples tareas (una por cada caja H y S del proyecto), se trabajará con una **única TAF** que generará un contenedor con los cables del proyecto.  

Para evitar replicar las fotos solicitadas por los elementos *apoyo* que pueden compartir múltiples cables —lo que incrementa la carga operativa para la EC—, en la tarea se presentará **la totalidad de los apoyos** por los que pasan cables **FC** y **MPO**.

El técnico seleccionará el apoyo en el que se encuentra y completará la información correspondiente en el formulario TAF.

---

## Premisa

> *"No son necesarios todos los secuenciales de los cables preconectorizados a no ser que sobrepase la longitud de cable indicada en diseño"*

---

## Comportamiento propuesto 1 (pendiente de consensuar)

El formulario NAS presenta el cable indicado por diseño como **preseleccionado** para la tarea a completar.  

**Ejemplo:** instalación de caja `N01-H01` → cable **MPO** de 100 metros.  

Si el técnico identifica que la longitud de cable propuesta **no es suficiente** (por ejemplo, coloca un cable de 150 metros), lo registrará en el formulario.  
En este caso, el sistema solicitará también completar el **secuencial de inicio y fin**.

Inconveniente: El técnico que completa esta información no es el mismo que tendió el cable. El administrativo de la contratista debe enviar la información al técnico de medición previo a completar el form.

---

## Comportamiento propuesto 2 (pendiente de consensuar)

Se presentará la totalidad de los cables dentro del formulario TAF. El técnico deberá indicar cual/es sufrieron modificaciones e incluir los secuenciales de inicio y fin para solo esos casos.  

Inconveniente: La info la completa el técnico de forma manual en la calle. Se presentan la totalidad de cables del proyecto y tiene que identificar desde el celular cuales sufrieron modificaciones. Puede haber errores.

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
$$
50 \ \text{m} \times 0.014 \ \frac{\text{kg}}{\text{m}} = 0.7 \ \text{kg}
$$

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

