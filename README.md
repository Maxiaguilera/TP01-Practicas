# Trabajo Práctico: Gestión de Ramas y Resolución de Conflictos en Git

## Objetivos

- Practicar el flujo de trabajo con ramas en Git
- Aprender a resolver conflictos de manera efectiva
- Comprender el proceso de merge y hotfix
- Trabajar colaborativamente en un proyecto

## Requisitos Previos

- Cuenta en GitHub
- Pertenecer a la organización CRUI-PP1
- Acceso al equipo asignado en la organización

## Estructura del Proyecto

El proyecto consistirá en un glosario de términos de las materias, donde cada integrante contribuirá con al menos 5 conceptos. La estructura será:

```
glosario/
├── conceptos.txt    # Archivo principal con los conceptos
└── ejemplos/        # Carpeta para archivos de ejemplo
```

## Flujo de Trabajo

### 1. Configuración Inicial

1. Clonar el repositorio
2. Crear una rama `dev` a partir de la rama principal
3. Cada integrante debe crear su propia rama a partir de `dev` con el formato: `feature/nombre-apellido`

### 2. Desarrollo Individual

Cada integrante debe:

1. Agregar al menos 5 conceptos al archivo `conceptos.txt`
2. Seguir el formato establecido:
   ```
   CONCEPTO
   Definición: [definición clara y concisa]
   Ejemplo: [ejemplo práctico]
   Notas: [información adicional relevante]
   ```

### 3. Ejercicios de Conflictos

#### Ejercicio 1: Conflictos de Edición Simultánea

1. Dos integrantes modificarán el mismo concepto en diferentes ramas
2. Ejemplo:
   - Integrante A modifica la definición de "Commit"
   - Integrante B modifica la misma definición
   - Resolver el conflicto manteniendo las mejoras de ambas versiones

#### Ejercicio 2: Conflictos de Orden y Estructura

1. Dos integrantes agregarán el mismo concepto en diferentes posiciones
2. Ejemplo:
   - Integrante A agrega "Branch" al principio del archivo
   - Integrante B agrega "Branch" al final
   - Decidir la posición correcta y resolver el conflicto

#### Ejercicio 3: Conflictos de Formato

1. Dos integrantes usarán diferentes formatos para el mismo concepto
2. Ejemplo:

   ```
   Versión A:
   COMMIT
   Definición: Guarda los cambios en el repositorio

   Versión B:
   Commit
   - Guarda los cambios
   - Crea un punto de control
   ```

   - Unificar el formato manteniendo la información relevante

#### Ejercicio 4: Hotfix

1. Identificar un error crítico en la rama main
2. Crear una rama `hotfix` desde main
3. Corregir el error
4. Mergear la corrección a main y dev

#### Ejercicio 5: Conflictos de Eliminación vs Modificación

1. Un integrante eliminará un concepto
2. Otro integrante modificará el mismo concepto
3. Resolver el conflicto decidiendo si:
   - Mantener el concepto con las modificaciones
   - Eliminarlo definitivamente
   - Moverlo a una sección diferente

### 4. Proceso de Integración

1. Mergear todas las ramas individuales a `dev`

   - Resolver los conflictos según los ejercicios anteriores
   - Documentar las decisiones tomadas en la resolución

2. Mergear `dev` a `test`

   - Verificar que no haya conflictos
   - Asegurar que el formato sea consistente

3. Mergear `test` a `main`
   - Realizar una revisión final
   - Asegurar que todos los conceptos estén correctamente formateados

## Criterios de Evaluación

1. **Completitud** (30%)

   - Al menos 5 conceptos por integrante
   - Todos los ejercicios de conflictos realizados
   - Proceso de integración completo

2. **Calidad del Contenido** (20%)

   - Definiciones claras y precisas
   - Ejemplos relevantes
   - Formato consistente

3. **Resolución de Conflictos** (30%)

   - Manejo adecuado de los conflictos
   - Documentación de las decisiones
   - Mantenimiento de la integridad del contenido

4. **Proceso Git** (20%)
   - Uso correcto de ramas
   - Commits descriptivos
   - Merge exitosos

## Entrega

1. Todos los cambios deben estar en la rama `main`
2. El repositorio debe contener:
   - Archivo `conceptos.txt` con todos los conceptos
   - Carpeta `ejemplos` con archivos de prueba
   - Documentación de los conflictos resueltos
3. Fecha límite: [fecha a definir]

## Notas Adicionales

- Mantener una comunicación clara entre los integrantes
- Documentar todos los conflictos resueltos
- Realizar commits frecuentes y descriptivos
- Seguir las convenciones de Git establecidas
