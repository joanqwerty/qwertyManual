# Rational Unified Process (RUP) y el Modelo 4+1 de Vistas

**Rational Unified Process (RUP)** organiza el desarrollo de software en fases iterativas, mientras que el **Modelo 4+1 de Vistas** ofrece una forma de documentar y visualizar la arquitectura del sistema desde cinco perspectivas:

- **Vista Lógica** (Logical)
- **Vista de Procesos** (Process)
- **Vista de Desarrollo** (Development)
- **Vista Física** (Physical)
- **Vista de Casos de Uso** (Use Case)

A continuación se muestra cómo se relacionan las etapas de RUP con los diagramas típicos de cada vista.

---

## 1. Inicio (Inception)

En esta fase se define el alcance y los requisitos del sistema.

**Diagramas usados:**

- **Vista de Casos de Uso:** Diagramas de casos de uso para identificar actores y funcionalidades clave.
- **Vista Lógica (preliminar):** Diagramas de clases de alto nivel para mostrar conceptos principales.
- **Vista de Procesos (opcional):** Diagrama de flujo de trabajo de alto nivel para identificar procesos críticos.

**Objetivo:** Validar la viabilidad y definir los límites del sistema.

---

## 2. Elaboración (Elaboration)

Se refinan los requisitos y se establece la arquitectura.

**Diagramas usados:**

- **Vista Lógica:** Diagramas de clases detallados y diagramas de secuencia para modelar interacciones clave.
- **Vista de Procesos:** Diagramas de actividad y colaboración para mostrar concurrencia y sincronización.
- **Vista de Desarrollo:** Diagramas de componentes para planificar la estructura de módulos.
- **Vista de Casos de Uso:** Refinamiento de casos de uso y escenarios principales.

**Objetivo:** Construir una arquitectura sólida y minimizar riesgos técnicos.

---

## 3. Construcción (Construction)

Se implementa y prueba el sistema.

**Diagramas usados:**

- **Vista de Desarrollo:** Diagramas de componentes y paquetes para guiar la implementación.
- **Vista Lógica:** Diagramas de clases y secuencias para validar diseño detallado.
- **Vista de Procesos:** Diagramas de comunicación y actividad para controlar ejecución concurrente.

**Objetivo:** Producir un sistema funcional listo para pruebas de integración.

---

## 4. Pruebas / Transición (Transition)

Se valida el sistema antes de su despliegue.

**Diagramas usados:**

- **Vista de Casos de Uso:** Diagramas de casos de uso para pruebas de aceptación y validación por el usuario.
- **Vista Física:** Diagramas de despliegue para planificar la infraestructura de producción.
- **Vista de Procesos:** Diagramas de actividad para verificar flujos críticos durante la operación.

**Objetivo:** Garantizar calidad, desempeño y satisfacción del usuario.

---

## 5. Mantenimiento (Maintenance)

Proceso continuo posterior al despliegue.

**Diagramas usados:**

- **Vista de Desarrollo:** Diagramas de componentes para planificar mejoras o refactorizaciones.
- **Vista de Casos de Uso:** Diagramas de casos de uso para nuevas funcionalidades.
- **Vista Física:** Diagramas de despliegue para cambios en infraestructura.

**Objetivo:** Mantener y evolucionar el sistema de manera controlada.

---

## Resumen visual

| Fase          | Casos de Uso | Lógica | Procesos | Desarrollo | Física |
| ------------- | ------------ | ------ | -------- | ---------- | ------ |
| Inicio        | ✅           | ⚪     | ⚪       | ⚪         | ⚪     |
| Elaboración   | ✅           | ✅     | ✅       | ✅         | ⚪     |
| Construcción  | ⚪           | ✅     | ✅       | ✅         | ⚪     |
| Pruebas       | ✅           | ⚪     | ✅       | ⚪         | ✅     |
| Mantenimiento | ✅           | ⚪     | ⚪       | ✅         | ✅     |

> ✅ = Principalmente utilizado
> ⚪ = Opcional / menor relevancia
