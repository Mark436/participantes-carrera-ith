# Participantes · Carrera ITH

## ¿Qué es este proyecto?

Es un sitio web para consultar y buscar participantes de la Carrera ITH. Permite encontrar registros mediante un buscador con autocompletado y visualizar la información de cada participante en una tabla.

El proyecto está desarrollado en un solo archivo `index.html`, que contiene el HTML, CSS, JavaScript y los datos. No utiliza bases de datos externas ni dependencias.

## ¿Cómo se guardan los datos?

Todos los registros se almacenan directamente en el archivo `index.html`, dentro de un arreglo de JavaScript llamado `participantes`.

Cada participante se guarda como un objeto con la siguiente estructura:

```json
{
  "id": 1,
  "fecha": "2026-10-21T18:22:40",
  "nombre": "Nombre Apellido",
  "rama": "VARONIL",
  "talla": "XL",
  "categoria": "SUPER MASTER (60 Y MAS)",
  "nota": ""
}
```

Los datos no se guardan en una base de datos ni se actualizan automáticamente. Para conservar cualquier cambio, es necesario modificar el archivo y guardar los cambios en el repositorio.

## ¿Cómo agregar un participante nuevo?

1. Abre el archivo `index.html`.
2. Busca el arreglo `const participantes = [...]`.
3. Agrega un nuevo objeto al final de la lista, separado por una coma.
4. Asigna un `id` único y completa la información del participante.
5. Guarda los cambios y actualiza el repositorio.

### Campos disponibles

| Campo       | Descripción                                   |
| ----------- | --------------------------------------------- |
| `id`        | Identificador único del registro.             |
| `fecha`     | Fecha y hora del registro.                    |
| `nombre`    | Nombre completo del participante.             |
| `rama`      | `VARONIL` o `FEMENIL`.                        |
| `talla`     | `CH`, `M`, `L` o `XL`.                        |
| `categoria` | Categoría correspondiente.                    |
| `nota`      | Información adicional o comentarios.          |

Una vez actualizado el repositorio, Netlify realizará automáticamente un nuevo despliegue del sitio.
