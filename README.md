# Middleware
# Práctica: comportamiento transversal en FastAPI

Práctica de 2.º DAW. He añadido a la API tres cosas que afectan a todas las rutas: CORS, un middleware de tiempo y un manejador global de errores.

## Qué incluye

- **CORS**: permite peticiones desde el frontend en `http://localhost:5173`.
- **Middleware `X-Process-Time`**: añade a cada respuesta el tiempo de proceso en milisegundos.
- **Exception handler global**: captura cualquier error no controlado y devuelve `{"error": "Error interno del servidor"}` con código 500, sin mostrar el stacktrace.

## Requisitos

- Python 3.10 o superior
- fastapi y uvicorn

```bash
pip install fastapi uvicorn
```

## Cómo ejecutarlo

```bash
cd routers
uvicorn main:app --reload --port 8000
```

La API queda en `http://127.0.0.1:8000`.

## Rutas de prueba

| Ruta | Resultado |
|------|-----------|
| `GET /` | 200 `{"mensaje": "Todo correcto"}` |
| `GET /error` | 500 `{"error": "Error interno del servidor"}` |

## Capturas

# Práctica: comportamiento transversal en FastAPI

Práctica de 2.º DAW. He añadido a la API tres cosas que afectan a todas las rutas: CORS, un middleware de tiempo y un manejador global de errores.

## Qué incluye

- **CORS**: permite peticiones desde el frontend en `http://localhost:5173`.
- **Middleware `X-Process-Time`**: añade a cada respuesta el tiempo de proceso en milisegundos.
- **Exception handler global**: captura cualquier error no controlado y devuelve `{"error": "Error interno del servidor"}` con código 500, sin mostrar el stacktrace.

## Requisitos

- Python 3.10 o superior
- fastapi y uvicorn

```bash
pip install fastapi uvicorn
```

## Cómo ejecutarlo

```bash
cd routers
uvicorn main:app --reload --port 8000
```

La API queda en `http://127.0.0.1:8000`.

## Rutas de prueba

| Ruta | Resultado |
|------|-----------|
| `GET /` | 200 `{"mensaje": "Todo correcto"}` |
| `GET /error` | 500 `{"error": "Error interno del servidor"}` |

## Capturas

![Imagen](<Captura de pantalla 2026-10-27 180920.png>)
