# Aplicatius de Rampa

Aquest projecte inclou dues aplicacions educatives interactives per a treballar conceptes relacionats amb les rampes:
- **`rampa_l.html`**: Es basa en la longitud de la rampa `l` com a dada principal.
- **`rampa_x.html`**: Es basa en la base de la rampa `x` i calcula la longitud de la rampa `l` a partir del teorema de Pitàgores.

## Descripció de les aplicacions
### `rampa_l.html`
- Aquesta aplicació utilitza les dades: `F` (força), `R` (resistència), `l` (longitud de la rampa) i `h` (alçada de la rampa).
- L'avantatge mecànic es calcula segons:
  - Si falta `F` o `R`: `AM = l / h`.
  - Si falta `l` o `h`: `AM = R / F`.

### `rampa_x.html`
- Aquesta aplicació utilitza les dades: `F` (força), `R` (resistència), `x` (base de la rampa) i `h` (alçada de la rampa).
- La longitud de la rampa `l` es calcula amb el teorema de Pitàgores: \( l^2 = x^2 + h^2 \).
- L'avantatge mecànic es calcula igual que a `rampa_l.html`.

## Funcionalitats compartides
- Generació automàtica de problemes amb valors aleatoris.
- Selecció d'una variable desconeguda (`F` o `R`) que l'usuari ha de calcular.
- Verificació de respostes:
  - Valor desconegut.
  - Avantatge mecànic.
- Feedback immediat amb missatges de correcte/incorrecte.
- Mostra de les solucions després de tres intents fallits.

## Diferències clau
| Característica          | `rampa_l.html`         | `rampa_x.html`         |
|-------------------------|------------------------|------------------------|
| Dada de la rampa       | Longitud `l`          | Base `x`               |
| Càlcul de `l`          | Proporcionada directament | Calculada amb Pitàgores |

## Instruccions d'ús
1. Obre el fitxer HTML desitjat (`rampa_l.html` o `rampa_x.html`) en un navegador.
2. Segueix les instruccions per resoldre el problema generat.
3. Introdueix les respostes als camps corresponents:
   - Valor desconegut.
   - Avantatge mecànic.
4. Comprova les respostes i llegeix el feedback proporcionat.

## Configuració
- **`DEBUG`**:
  - Si està activat, mostra el solucionari automàticament.
  - Valors possibles: `true` o `false`.
- **`TOLERANCE`**:
  - Controla el marge d'error permès en les respostes.
  - Valor per defecte: `0.01` (1%).

## Exemple de problemes generats
### Exemple 1: `rampa_l.html`
| F (N) | R (N) | l (m) | h (m) |
|-------|-------|-------|-------|
| ?     | 200   | 5.00  | 3.00  |
- Avantatge mecànic: \( AM = l / h = 5 / 3 = 1.67 \).

### Exemple 2: `rampa_x.html`
| F (N) | R (N) | x (m) | h (m) |
|-------|-------|-------|-------|
| 100   | ?     | 4.00  | 3.00  |
- Longitud de la rampa: \( l = \sqrt{x^2 + h^2} = \sqrt{4^2 + 3^2} = 5 \).
- Avantatge mecànic: \( AM = l / h = 5 / 3 = 1.67 \).

## Contacte
- Correu electrònic: aagust11@xtec.cat
- Correu electrònic: angelac@insmollet.cat

