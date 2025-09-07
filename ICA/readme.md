# 📌 DF Intervención de Caja Activa - Brownfield  

Este documento describe el flujo de trabajo para la **intervención de una caja activa en un escenario Brownfield**, desde la detección hasta el cierre de tareas.  

---

## 🔄 Flujo del Proceso  

1. **Inicio**  
   - El proceso comienza cuando el **supervisor de obra detecta una caja activa**.  

2. **Notificación**  
   - El supervisor notifica a **despacho** para que cree la tarea interna correspondiente.  

3. **Creación de Tareas**  
   - Se crea la **tarea interna ICA** para ejecutar la **Tarea de Campo (TC)**.  
   - Se genera una **tarea de monitoreo para NOC** con el fin de corroborar el estado de la caja activa al finalizar la TC.  
 
4. **Ejecución de la Tarea de Campo**  
   - Se programa la TC para que la **EC (empresa contratista)** ejecute la intervención.  

5. **Validación de Ejecución**  
   - Se evalúa si la **Tarea de Campo fue ejecutada correctamente**:  
     - ✅ **Sí**:  
       1. Se realiza el **cierre de tarea interna MCA**.    
       2. La **cuadrilla de empalme** contacta al supervisor de campo para informar la finalización del trabajo.  
       3. Se ejecuta el **cierre de tarea interna ICA**.  
     - ❌ **No**:  
       - El **NOC detecta una caída de servicio**.  
       - Se toman acciones correctivas (pendiente de definir en el flujo).  

---

## 📋 Actores Involucrados  
- **Supervisor de obra**: Detecta la caja activa y da aviso inicial.  
- **Despacho**: Crea las tareas internas.  
- **NOC**: Monitorea y detecta caídas de servicio.  
- **Cuadrilla de empalme**: Confirma finalización de trabajos y ejecuta la tarea de campo. .  

---

## ✅ Resultado Esperado  
- Cierre exitoso de las tareas internas (**MCA** e **ICA**).  
- Confirmación de estado de la caja activa.  
- Prevención de caídas de servicio.

---
