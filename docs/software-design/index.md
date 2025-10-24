# Diseño de software

Bienvenido a la guía completa de principios de diseño en desarrollo de software. Aquí encontrarás el índice de los principales principios que te ayudarán a escribir código más limpio, mantenible y eficiente.

## Principios Fundamentales

### [KISS (Keep It Simple, Stupid)](/principios/kiss.md)

Mantener la simplicidad como objetivo clave en el diseño de software.

### [DRY (Don't Repeat Yourself)](/principios/dry.md)

Evitar la duplicación de código y conocimiento en el sistema.

### [YAGNI (You Aren't Gonna Need It)](/principios/yagni.md)

No implementar funcionalidad hasta que sea realmente necesaria.

## Principios SOLID

### [S - Single Responsibility Principle](/principios/solid/srp.md)

Una clase debe tener una sola razón para cambiar.

### [O - Open/Closed Principle](/principios/solid/ocp.md)

Las entidades deben estar abiertas para extensión pero cerradas para modificación.

### [L - Liskov Substitution Principle](/principios/solid/lsp.md)

Los objetos de una superclase deben ser reemplazables por objetos de sus subclases.

### [I - Interface Segregation Principle](/principios/solid/isp.md)

Los clientes no deben depender de interfaces que no utilizan.

### [D - Dependency Inversion Principle](/principios/solid/dip.md)

Depender de abstracciones, no de concreciones.

## Principios GRASP

### [Information Expert](/principios/grasp/information-expert.md)

Asignar responsabilidad a la clase que tiene la información necesaria.

### [Creator](/principios/grasp/creator.md)

Determinar quién debe ser responsable de crear objetos.

### [Controller](/principios/grasp/controller.md)

Manejar eventos del sistema de manera coordinada.

### [Low Coupling](/principios/grasp/low-coupling.md)

Minimizar las dependencias entre clases.

### [High Cohesion](/principios/grasp/high-cohesion.md)

Mantener elementos relacionados juntos.

### [Polymorphism](/principios/grasp/polymorphism.md)

Usar polimorfismo para manejar alternativas basadas en tipos.

### [Pure Fabrication](/principios/grasp/pure-fabrication.md)

Crear clases artificiales para mantener bajo acoplamiento.

### [Indirection](/principios/grasp/indirection.md)

Asignar responsabilidad a un objeto intermedio.

### [Protected Variations](/principios/grasp/protected-variations.md)

Proteger elementos de variaciones en otros elementos.

## Otros Principios Importantes

### [Composition over Inheritance](/principios/composition-over-inheritance.md)

Favorecer la composición sobre la herencia para reutilizar código.

### [Law of Demeter](/principios/law-of-demeter.md)

Un objeto debe conocer solo sus colaboradores inmediatos.

### [Separation of Concerns](/principios/separation-of-concerns.md)

Separar diferentes aspectos del programa en secciones distintas.

### [Inversion of Control](/principios/inversion-of-control.md)

Invertir el control del flujo de ejecución del programa.

## Beneficios de Aplicar Principios de Diseño

- **Mantenibilidad** - Código más fácil de modificar y extender
- **Legibilidad** - Código más claro y comprensible
- **Reutilización** - Componentes más reutilizables
- **Testabilidad** - Código más fácil de probar
- **Escalabilidad** - Sistemas que crecen de manera ordenada
- **Flexibilidad** - Adaptación más sencilla a cambios de requisitos

---

_Recuerda: Los principios de diseño son guías fundamentales para crear software de calidad. Aplícalos de manera consistente para lograr código más robusto y mantenible._
