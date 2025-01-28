# Pràctica de Torn

## Descripció
Aquest projecte és una aplicació interactiva en HTML, CSS i JavaScript que permet practicar càlculs relacionats amb el torn. Els conceptes treballats inclouen:
- Longitud de la maneta (l).
- Radi del torn (r).
- Força aplicada (F).
- Resistència (R).

## Funcionalitats
- Generació aleatòria de problemes amb un valor desconegut entre l, r, F o R.
- Càlcul automàtic de l'avantatge mecànic:
  - Si falta `l` o `r`: `AM = R / F`.
  - Si falta `F` o `R`: `AM = l / r`.
- Feedback immediat per comprovar les respostes.
- Visualització del solucionari si `DEBUG` està activat.
- Mostra de solucions després de 3 intents incorrectes.

## Requisits
- Navegador web modern amb suport per a JavaScript.
- Accés a internet si es necessiten recursos externs.

## Configuració
### Variables clau
1. **DEBUG**
   - Mostra el solucionari automàticament si està activat.
   - Valors possibles: `true` o `false`.
2. **TOLERANCE**
   - Permet ajustar el marge d'error permès per a les respostes.
   - Per defecte: `0.01` (1%).

### Modificació de la configuració
Edita el fitxer HTML i modifica les constants a la part superior del codi JavaScript:
```javascript
const DEBUG = false;
const TOLERANCE = 0.01;
```

## Ús
1. Obre el fitxer `index.html` en un navegador web.
2. Llegeix l'enunciat generat automàticament.
3. Introdueix les respostes per al valor desconegut i l'avantatge mecànic.
4. Comprova les respostes i visualitza el feedback.

## Estructura del projecte
```
/
|-- torn.html        (Fitxer principal)
|-- /img              (Carpeta d'imatges, si s'escau)
```

## Personalització
- Per ajustar la dificultat o afegir noves funcionalitats, modifica el codi JavaScript:
  - Generació de valors per `l`, `r`, `F` i `R`.
  - Mètodes de càlcul per a l'avantatge mecànic.

## Exemple de problema
| F (N) | l (m) | R (N) | r (m) |
|-------|-------|-------|-------|
| ?     | 2.50  | 50.00 | 0.75  |

- Valor desconegut: F.
- Avantatge mecànic calculat: `l / r`.

## Contacte
Afegeix la teva informació de contacte o crèdits aquí si és necessari.

