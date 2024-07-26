# Carreras

## Listado de Entidades

### carreras **(ED)**

- id_carrera **(PK)** INT AUTO **UNIQUE**
- nombre VARCHAR(50)
- tipo_carrera **(FK)** INT
- fecha DATE
- tiempo VARCHAR(10)
- mejor_tiempo BOOLEAN
- altitud INT
- lugar VARCHAR(50)
- pais **(FK)** INT
- foto VARCHAR(255)

### tipos_carreras **(EC)**

- id_tipo_carrera **(PK)** INT AUTO **UNIQUE**
- descripcion TEXT
- distancia **(UQ)** FLOAT 

### países **(EC)**

- id_pais **(PK)** INT AUTO **UNIQUE**
- nombre VARCHAR(50)


## Relaciones entre entidades

1. Una **carrera** _pertenece_ a un **tipo de carrera**. (_1 a 1_)
1. Una **carrera** se _corre_ a un **país**. (_1 a 1_)


## Diagramas

### Modelo Entidad - Relación

![Modelo Entidad - Relación](./CarrerasModeloE-R.png)

### Modelo Entidad - Relación

![Modelo Relacional de la Base de Datos](./ModeloRelacionalBBDD.png)

## Reglas de Negocio

### carreras

1. Crear el registro de una carrera
1. Leer el registro de una(s) carrera(s) dada una condición en particular.
1. Leer todos los registros de la entidad carreras.
1. Actualizar los datos de una carrera dada una condición en particular.
1. Eliminar los datos de una carrera dada una condición en particular.

### tipos_carreras

1. Todos los valores del atributo distancia, deberán estar expresados en km y no se podrán repetir.
1. Crear el registro de un tipo de carrera
1. Leer el registro de un(os) tipo(s) de carrera(s) dada una condición en particular.
1. Leer todos los registros de la entidad tipos carreras.
1. Actualizar los datos de un tipo de carrera dada una condición en particular.
1. Eliminar los datos de una tipo de carrera dada una condición en particular.

### paises

1. Crear el registro de un país
1. Leer el registro de un(os) pais(es) dada una condición en particular.
1. Leer todos los registros de la entidad paises.
1. Actualizar los datos de un país dada una condición en particular.
1. Eliminar los datos de un páis dada una condición en particular.