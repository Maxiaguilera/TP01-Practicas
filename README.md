# TP01 - Gestión de Ramas y Resolución de Conflictos en Git

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
4. Agregar al menos 5 conceptos al archivo `glosario/conceptos.txt` siguiendo el formato establecido
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

- `id`: Número único secuencial para cada concepto
- `seccion`: Área temática del concepto (ej: GIT, PROGRAMACION, etc.)
- `materias`: Materias relacionadas (separadas por comas)
- `sigla|nombre`: Nombre o sigla del concepto
- `descripcion`: Explicación detallada del concepto
- `link`: Enlace a documentación oficial o referencia relevante

## Ejercicios de Conflictos

### 1. Conflictos de Edición Simultánea

- Dos integrantes modificarán el mismo concepto en diferentes ramas
- Resolver manteniendo las mejoras de ambas versiones
- **Evidencia requerida**: Captura de pantalla del conflicto y su resolución

### 2. Conflictos de Orden y Estructura

- Dos integrantes agregarán el mismo concepto con diferentes IDs
- Decidir el ID correcto y resolver el conflicto
- **Evidencia requerida**: Captura de pantalla del conflicto y su resolución

### 3. Conflictos de Formato

- Dos integrantes usarán diferentes formatos para el mismo concepto
- Unificar el formato manteniendo la información relevante
- **Evidencia requerida**: Captura de pantalla del conflicto y su resolución

### 4. Hotfix

- Identificar un error crítico en la rama main (ej: ID duplicado)
- Crear una rama `hotfix` desde main
- Corregir el error
- Mergear la corrección a main y dev
- **Evidencia requerida**:
  - Captura de pantalla del error identificado
  - Captura de pantalla del proceso de hotfix
  - Historial de Git que muestre la rama hotfix y su merge

### 5. Conflictos de Eliminación vs Modificación

- Un integrante eliminará un concepto
- Otro integrante modificará el mismo concepto
- Resolver decidiendo si mantener, eliminar o mover el concepto
- **Evidencia requerida**: Captura de pantalla del conflicto y su resolución

## Proceso de Integración

1. Mergear todas las ramas individuales a `dev`
   - **Evidencia en Git**: Historial de commits y merges
2. Mergear `dev` a `test`
   - **Evidencia en Git**: Historial de commits y merges
3. Mergear `test` a `main`
   - **Evidencia en Git**: Historial de commits y merges

## Evidencias Requeridas

### Capturas de Pantalla

- Cada conflicto y su resolución
- Proceso de hotfix
- Estado final del archivo de conceptos

### Historial Git

- Creación y uso de ramas
- Commits descriptivos
- Proceso de merge
- Resolución de conflictos
- Hotfix implementado

## Notas Importantes

- Mantener una comunicación clara entre los integrantes
- Documentar todos los conflictos resueltos
- Realizar commits frecuentes y descriptivos
- Asegurar que los IDs sean únicos y secuenciales
- Verificar que todos los campos requeridos estén completos
- Guardar todas las capturas de pantalla en la carpeta `glosario/ejemplos/`
