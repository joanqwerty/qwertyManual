# Estructura y Gestión de Ramas en el Kernel de Linux

Breve resumen
- El kernel tiene varias ramas con roles claros: la rama principal (mainline) donde Linus integra los cambios, `linux-next` como integrador de parches de subsistemas, ramas de lanzamiento (rc), ramas `stable` para correcciones y ramas `longterm` (LTS) para soporte prolongado. Además hay ramas tópicas/por subsistema (topic/*, for-next/*) donde se preparan conjuntos de parches.

Flujo típico (resumen)
1. Desarrolladores envían parches a ramas topic/subsystem.
2. Los mantenedores consolidan y envían a `for-next` / `topic/*`.
3. `linux-next` integra ramas de subsistema para pruebas.
4. Linus mergea desde `linux-next` a `main` y crea release candidates (`vX.Y-rcN`).
5. Tras el lanzamiento, cambios críticos se aplican a `stable/vX.Y`.
6. Algunas versiones se marcan `longterm` para parches a largo plazo.

```mermaid
gitGraph
    commit id: "v6.5" tag: "v6.5"
    branch linux-next
    commit id: "merge-integration"
    branch for-next
    commit id: "subsys-merge"
    checkout linux-next
    merge for-next
    checkout main
    merge linux-next
    commit id: "v6.6-rc1" tag: "v6.6-rc1"
    branch stable/v6.x
    checkout stable/v6.x
    commit id: "stable-fix"
    checkout main
    branch longterm/v5.x
    commit id: "lts-fix"
    checkout longterm/v5.x
    commit id: "lts-backport"
    checkout main
    branch topic/driver-x
    commit id: "driver-x"
    checkout linux-next
    merge topic/driver-x
```