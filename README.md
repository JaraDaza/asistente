# Asistente Pedagógico Perú V1.4.2 — Sin bases de datos

Corrección orientada al problema «sesión generada, pero controles desactivados».

- Se activa «Iniciar clase» después de generar correctamente una sesión.
- La etiqueta «Sesión lista» confirma el estado de la sesión.
- Hay una marca visible «Frontend V1.4.2 activo» para detectar archivos antiguos.
- Se evita la caché del navegador para HTML, CSS y JavaScript.
- El avatar Facecap, exportación Word y generación mantienen el funcionamiento previo.
- **No incluye ninguna base de datos ni conexión a EPAM.**

## Ejecutar

`python -m pip install -r requirements.txt`

`python app.py`

Abre `http://127.0.0.1:5000`. Comprueba que diga «Frontend V1.4.2 activo». Genera una sesión nueva (no se recuperan sesiones de la versión anterior al actualizar la página) y pulsa «Iniciar clase».

Si no aparece la versión V1.4.2, verifica que no haya un proceso Flask antiguo ocupando el puerto 5000 y que hayas abierto la carpeta correcta.
