# Cartas Yu-Gi-Oh! TCG – Catálogo

Catálogo web estático (GitHub Pages) de mis cartas Yu-Gi-Oh! con tasación, filtros, búsqueda y compra por WhatsApp.

## Estructura
- `index.html` – la página (no requiere compilación).
- `data/cards.json` – lista de cartas (un objeto por carta).
- `img/<id>.jpg` – foto de cada carta.

## Agregar cartas nuevas
1. Guardar la foto como `img/<id>.jpg` (id único, ej. `dark-magician-es`, copias: `-2`, `-3`).
2. Agregar un objeto al final de `data/cards.json`:

```json
{"id":"dark-magician-es","name_es":"Mago Oscuro","name_en":"Dark Magician","set_code":"LOB-SP005",
 "set_name":"Leyenda del Dragón Blanco de Ojos Azules","year":2002,"language":"Español",
 "edition":"Ilimitada","rarity":"Ultra Rare","type":"Monstruo Normal","condition":"NM",
 "price_clp":5000,"price_usd":5.0,"price_source":"...","price_url":"https://...","notes":"",
 "image":"img/dark-magician-es.jpg"}
```
Opcional: `"sold": true` oculta la carta del catálogo.

## Precios
Referenciales en CLP: primero mercado chileno; si no hay, internacional (TCGplayer/Cardmarket vía PriceCharting) convertido con el dólar observado del día. El estado se estima por foto.

## Contacto
WhatsApp: +56 9 5659 2453
