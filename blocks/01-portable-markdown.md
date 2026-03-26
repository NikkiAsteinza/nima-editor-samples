# Portable Markdown And Callouts

Este archivo esta pensado para validar que la base del editor sigue siendo Markdown normal aunque se edite en modo enriquecido.

## Formato inline

Puedes seleccionar este parrafo para probar **bold**, *italic*, ~~strikethrough~~, `inline code` y <u>underline</u>.

Tambien puedes insertar un [enlace relativo](./02-technical-blocks.md) y comprobar que sigue siendo portable fuera del editor.

## Callouts

> [!NOTE]
> Los callouts forman parte de la base documental y deberian verse bien en preview y export.

> [!WARNING]
> Edita el texto dentro de este callout y guarda para confirmar que no se rompe la sintaxis.

> [!IMPORTANT]
> Esta pagina sirve para validar toolbar de formato, seleccion, serializacion y lectura final.

## Listas

- Crear un item nuevo
- Mover un item a otra posicion
- Convertir una linea en lista numerada

1. Abrir el archivo
2. Editar una frase
3. Revisar el resultado

## Checklist

- [x] Markdown legible
- [x] Callouts visibles
- [ ] Probar el cambio entre modo texto y modo enriquecido
- [ ] Agregar un item nuevo

## Cita

> Nima anade tooling al Markdown. No reemplaza el formato base.

## Tabla pequena

| Elemento | Validacion |
| --- | --- |
| Heading | jerarquia visual |
| Lista | roundtrip limpio |
| Callout | render y export |
| Link | navegacion interna |
