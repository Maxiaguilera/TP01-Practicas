# TP01 - Gestión de Ramas y Resolución de Conflictos en Git

Fecha de entrega: 21/05/2025 23:00 hs

En caso de no entregar en termino, se deberan realizar reentregas con agregados.

## Estructura del Proyecto

```
TP01/
├── glosario/
│   ├── conceptos.txt    # Archivo principal con los conceptos
│   └── ejemplos/        # Carpeta para archivos de ejemplo
└── README.md            # Este archivo
```

## Instrucciones

1. Clonar este repositorio
2. Crear una rama `dev` a partir de la rama principal
3. Cada integrante debe crear su propia rama a partir de `dev` con el formato: `feature/nombre-apellido`
4. Cada integrante debe agregar 5 conceptos al archivo `glosario/conceptos.txt` siguiendo el formato establecido
   - Un grupo de 5 integrantes terminará con 25 conceptos en total
   - Cada concepto debe tener su propio commit con un mensaje descriptivo
   - Ejemplo: "feat: Agrega concepto de Git - Sistema de control de versiones"
5. Realizar los ejercicios de conflictos según las instrucciones
6. Seguir el proceso de integración especificado

## Formato de Conceptos

Cada concepto debe seguir el siguiente formato:

```
id:
seccion:
materias:
sigla|nombre:
descripcion:
link:
```

Donde:

- `id`: Número único secuencial para cada concepto (del 01 al 25 para un grupo de 5 integrantes)
- `seccion`: Área temática del concepto (ej: GIT, PROGRAMACION, etc.)
- `materias`: Materias relacionadas (separadas por comas)
- `sigla|nombre`: Nombre o sigla del concepto
- `descripcion`: Explicación detallada del concepto
- `link`: Enlace a documentación oficial o referencia relevante

## Ejercicios de Conflictos

### 1. Conflictos de Edición Simultánea

- Dos integrantes modificarán el mismo concepto en diferentes ramas
- Resolver manteniendo las mejoras de ambas versiones
- **Buena documentación**:
  - Captura del conflicto mostrando los marcadores de Git
  - Captura del archivo resuelto
  - Explicación de las decisiones tomadas

### 2. Conflictos de Orden y Estructura

- Dos integrantes agregarán el mismo concepto con diferentes IDs
- Decidir el ID correcto y resolver el conflicto
- **Buena documentación**:
  - Captura de los IDs en conflicto
  - Explicación del criterio usado para decidir el ID final

### 3. Conflictos de Formato

- Dos integrantes usarán diferentes formatos para el mismo concepto
- Unificar el formato manteniendo la información relevante
- **Buena documentación**:
  - Captura de los diferentes formatos
  - Explicación del formato elegido y por qué

### 4. Hotfix

- Identificar un error crítico en la rama main (ej: ID duplicado)
- Crear una rama `hotfix` desde main
- Corregir el error
- Mergear la corrección a main y dev
- **Buena documentación**:
  - Captura del error identificado
  - Captura del proceso de hotfix
  - Explicación del impacto del hotfix

### 5. Conflictos de Eliminación vs Modificación

- Un integrante eliminará un concepto
- Otro integrante modificará el mismo concepto
- Resolver decidiendo si mantener, eliminar o mover el concepto
- **Buena documentación**:
  - Captura del conflicto
  - Explicación de la decisión tomada

## Proceso de Integración

1. Mergear todas las ramas individuales a `dev`
   - **Evidencia en Git**: Historial de commits y merges
2. Mergear `dev` a `test`
   - **Evidencia en Git**: Historial de commits y merges
3. Mergear `test` a `main`
   - **Evidencia en Git**: Historial de commits y merges

## Guía de Documentación

### Estructura de Documentación

```
glosario/ejemplos/
├── conflictos/
│   ├── ejercicio-1/
│   │   ├── conflicto.png
│   │   ├── resolucion.png
│   │   └── explicacion.md
│   ├── ejercicio-2/
│   │   └── ...
│   └── ...
└── hotfix/
    ├── error.png
    ├── proceso.png
    └── explicacion.md
```

### Contenido de la Documentación

1. **Capturas de Pantalla**:

   - Usar nombres descriptivos
   - Incluir contexto relevante
   - Resaltar los puntos importantes

2. **Explicaciones**:

   - Describir el problema encontrado
   - Explicar el proceso de resolución
   - Justificar las decisiones tomadas
   - Incluir lecciones aprendidas

3. **Formato de los Archivos**:
   - Incluir encabezados claros
   - Usar listas para organizar la información
   - Incluir referencias cuando sea necesario

## Notas Importantes

- Mantener una comunicación clara entre los integrantes
- Documentar todos los conflictos resueltos
- Realizar commits frecuentes y descriptivos
- Asegurar que los IDs sean únicos y secuenciales (01-25 para grupo de 5)
- Verificar que todos los campos requeridos estén completos
- Seguir la estructura de documentación propuesta
- Usar mensajes de commit descriptivos y consistentes
- Cada integrante debe contribuir con 5 conceptos únicos
- Coordinar entre integrantes para evitar duplicación de conceptos
- Mantener un registro de qué integrante agregó cada concepto
