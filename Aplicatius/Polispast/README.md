
# Pràctica de Polispasts

## Descripció
Aquest projecte consisteix en una aplicació interactiva en HTML, CSS i JavaScript per practicar el càlcul de forces, avantatge mecànic i la identificació del nombre de politges mòbils en un polispast.

## Funcionalitats
- Generació aleatòria de problemes relacionats amb polispasts, amb tres variables: F (força), R (resistència) i n (nombre de politges mòbils).
- Opció de calcular el valor desconegut i l'avantatge mecànic.
- Feedback immediat amb un sistema de "correcte" o "error".
- Solucions detallades al fallar 3 intents.

## Requisits
- Navegador web modern amb suport per a JavaScript.

## Configuració
- **Variables clau:**

1. **DEBUG:** Controla si el solucionari és visible des del principi.

    - Valors possibles: `true` (solucionari visible), `false` (solucionari ocult).

    - Per defecte: `false`.

2. **TOLERANCE:** Controla el marge d'error permès per a les respostes.

    - Per defecte: `0.01` (1%).


## Estructura del projecte

```
/ (directori principal)

|-- polispast.html (fitxer principal)

|-- /img (carpeta d'imatges locals, si s'escau)
```

## Ús

1. Obre `index.html` en un navegador web.
2. Segueix les instruccions per resoldre els problemes generats de manera aleatòria.


## Personalització
- Si vols canviar el marge d'error permès, ajusta la variable `TOLERANCE` al fitxer principal:
```javascript
const TOLERANCE = 0.01;
```
