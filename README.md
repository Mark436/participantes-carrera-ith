# Participantes · Carrera ITH

Buscador de participantes con autocompletado, ficha del registro y tabla completa.
Todo vive en un solo `index.html` (HTML + CSS + JS + datos), sin dependencias ni build.

## Uso local

Abre `index.html` en el navegador. No necesita servidor.

## Despliegue en Netlify

1. En Netlify: **Add new site → Import an existing project → GitHub** y elige este repo.
2. Deja los valores que toma de `netlify.toml`: sin comando de build, directorio de publicación `.`.
3. **Deploy**. Cada push a `main` vuelve a desplegar solo.

## Actualizar los registros

Los datos están en `index.html`, en la línea `const participantes = [...]`.
Cada registro tiene esta forma:

```json
{"id":1,"fecha":"2026-10-21T18:22:40","nombre":"Nombre Apellido","rama":"VARONIL","talla":"XL","categoria":"SUPER MASTER (60 Y MAS)","nota":""}
```

- `rama`: `VARONIL` o `FEMENIL`
- `talla`: `CH`, `M`, `L` o `XL`
- `nota`: texto libre del formulario (comentarios, teléfono, etc.)

## Privacidad

La lista incluye nombres y algunos teléfonos. El sitio manda `X-Robots-Tag: noindex` y
`robots.txt` bloquea a los buscadores, pero cualquiera con el enlace puede verlo.
Si quieres restringirlo, activa **Password protection** en Netlify
(Site configuration → Access & security) o mantén el repo privado.
