# Rotten Tomatoes Scraper (Async)

Scraper asíncrono en Python para obtener información básica de películas/series desde [Rotten Tomatoes](https://www.rottentomatoes.com/), incluyendo:

- Link a la página de la película/serie desde los resultados de búsqueda.
- Porcentajes de aprobación de críticos y audiencia.
- Cantidad de reviews y enlaces a las páginas de reviews.

## Características

- **Asíncrono**: usa `aiohttp` y `asyncio` para hacer peticiones HTTP no bloqueantes.
- **Robusto**: manejo de errores de red, timeouts y respuestas HTTP no exitosas.
- **Logging estructurado**: en lugar de `print`, usa el módulo `logging` para facilitar debugging y monitoreo.
- **Fácil de extender**: la estructura por funciones separadas (`search_movie`, `find_scorecard`, `init_scorecard_search`) permite agregar más campos o endpoints sin reescribir todo.

## Requisitos

- Python 3.10+ (recomendado por la sintaxis de `async with` múltiple y tipado).
- Dependencias:
  - `aiohttp`
  - `beautifulsoup4`

## Instalación

```bash
pip install aiohttp beautifulsoup4
```

## Uso básico

Ejecutar directamente como script:

```bash
python tu_archivo.py
```