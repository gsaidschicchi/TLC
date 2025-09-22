# Casos de Uso del Formulario - Escenarios de Campo

A continuación se describen los casos de uso disponibles en el formulario, con énfasis en **cuándo corresponde utilizar cada uno**:

---

## 📌 Escenario 1: Informar elemento en calle - no encontrado en tarea

**🟩 Cuándo se usa:**  
Cuando se detecta en campo un elemento existente que **no está incluido en la tarea original**.

**🟢 ¿Por qué se reporta?:**  
Aunque no requiere mano de obra adicional, **sí genera consumo de materiales**, por lo tanto debe informarse.

---

## 📌 Escenario 2: Informar instalación de nuevo elemento - detectado desde calle

**🟩 Cuándo se usa:**  
Cuando en campo se identifica la necesidad de **instalar un nuevo elemento**, **sin que exista una tarea previa** creada para ello.

**🟢 ¿Por qué se reporta?:**  
Porque la instalación **no fue planificada** y debe **ser registrada directamente desde el terreno**.

# 📌 Caso de Uso: Reporte de Novedades

## 📝 Descripción
Este caso de uso permite a la **cuadrilla de la empresa contratista** reportar un elemento detectado en calle que **no se encuentra en el plano**.  
El objetivo es **registrar, validar y actualizar** esta novedad en el sistema, de manera que:
- Se evidencie el trabajo realizado.
- Se registre el consumo de materiales.
- Se habilite el pago de la tarea (si corresponde).
- El **GIS** se mantenga actualizado.

---

## 👥 Actores
- **Cuadrilla** → Actor principal, reporta la novedad.  
- **Supervisor de campo** → Valida la ejecución de la tarea.  
- **Administrador GIS** → Incorpora el nuevo elemento en el plano.  
- **Moica Público** → Sistema móvil para cargar el formulario en campo.  
- **GIS** → Sistema cartográfico donde se consolida la información.  

---

## 🎯 Objetivos del Actor
- Declarar un elemento que no está en el plano.  
- Registrar la tarea para poder consumir materiales y, si corresponde, habilitar el pago.  
- Proporcionar evidencia (foto, ubicación, observaciones).  

---

## 🔄 Flujo Principal
1. La cuadrilla detecta un elemento en calle no reflejado en el plano.  
2. Ingresa a **Moica Público** y selecciona “Reporte de Novedad”.  
3. El sistema solicita **clasificar el elemento**:  
   - **Pagable** (consume materiales y habilita pago).  
   - **No Pagable** (consume materiales).  
4. La cuadrilla completa el **formulario** con datos, fotos y materiales.  
5. La información se envía al sistema central.  
6. El **supervisor de campo** valida la novedad.  
7. El **administrador GIS** actualiza el plano en el sistema GIS.  
8. El proceso finaliza con la novedad registrada y GIS actualizado.  

---

## ⚠️ Flujos Alternativos / Excepciones
- **[A1] Sin conexión en campo:** la novedad se guarda localmente y se envía más tarde.  
- **[A2] Novedad rechazada:** el supervisor no valida la novedad y devuelve para corrección.  
- **[A3] Error GIS:** si la integración falla, se genera una alerta al administrador GIS.  

---

## ✅ Post-condiciones
- El elemento queda registrado en el sistema.  
- El consumo de materiales se almacena.  
- La tarea queda habilitada para pago (si corresponde).  
- El GIS refleja la novedad.  

---

## 📊 Diagrama de Caso de Uso

```plantuml
@startuml
left to right direction

actor "Cuadrilla" as Cuadrilla
actor "Supervisor de campo" as Supervisor
actor "Administrador GIS" as AdminGIS
actor "Moica Público (Sistema)" as Moica
actor "GIS" as GIS

usecase "Reporte de Novedad" as UC1
usecase "Clasificar Elemento" as UC2
usecase "Elemento Pagable\n(consumo materiales)" as UC2a
usecase "Elemento No Pagable\n(consumo materiales)" as UC2b
usecase "Registrar Novedad\n(Formulario)" as UC3
usecase "Validar Novedad" as UC4
usecase "Actualizar GIS" as UC5

Cuadrilla --> UC1
Moica --> UC3
Supervisor --> UC4
AdminGIS --> UC5
GIS --> UC5

UC1 --> UC2 : <<include>>
UC1 --> UC3 : <<include>>
UC1 --> UC4 : <<include>>
UC1 --> UC5 : <<include>>

UC2 --> UC2a : <<extend>>
UC2 --> UC2b : <<extend>>

@enduml


---

## 📌 Escenario 3: Informar re-instalación por ausencia de elemento

**🟩 Cuándo se usa:**  
Cuando se constata en campo que un elemento que **debía estar instalado está ausente**.

**🟢 ¿Por qué se reporta?:**  
Se debe **reejecutar la tarea**, ya que el material se perdió o no fue correctamente instalado.

---

## 📌 Escenario 4: Informar reemplazo por falla de elemento

**🟩 Cuándo se usa:**  
Cuando un elemento instalado **no funciona correctamente y necesita ser reemplazado**.

**🟢 ¿Por qué se reporta?:**  
Puede implicar un **descuento de materiales por mala ejecución**, afectando la responsabilidad de la empresa contratista.

---

## 📌 Escenario 5: Informar elemento dañado por terceros

**🟩 Cuándo se usa:**  
Cuando se observa en calle un **daño provocado por terceros** que impide el correcto funcionamiento de la red.

**🟢 ¿Por qué se reporta?:**  
Aunque no sea responsabilidad del contratista, **se debe volver a ejecutar la tarea** para restablecer el servicio.

---
