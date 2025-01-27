# Pràctica de Pes i Palanques

## Descripció
Aquest projecte consisteix en una aplicació interactiva en HTML, CSS i JavaScript per practicar el càlcul de forces, avantatge mecànic i la identificació dels tipus de palanques.

## Funcionalitats
- Generació aleatòria de problemes relacionats amb palanques de primer, segon i tercer gènere.
- Opció de calcular forces, distàncies i avantatge mecànic.
- Suport per visualitzar imatges des de local o en línia segons la configuració.
- Feedback immediat amb un sistema de "correcte" o "error".
- Solucions detallades al fallar 3 intents.

## Requisits
- Navegador web modern amb suport per a JavaScript.
- Accés a internet si `MODE_IMATGE` està configurat a `ONLINE`.

## Configuració
### Variables clau:
1. **DEBUG**
   - Controla si el solucionari és visible des del principi.
   - Valors possibles: `true` (solucionari visible), `false` (solucionari ocult).
   - **Default**: `false`.

2. **MODE_IMATGE**
   - Determina si les imatges s'han de carregar localment o en línia.
   - Valors possibles: `"LOCAL"` (carregar des de `img/`), `"ONLINE"` (carregar des de GitHub).
   - **Default**: `"ONLINE"`.

### Com modificar:
Edita les variables al principi del fitxer `palanques.html`:
```javascript
const DEBUG = false;
const MODE_IMATGE = "ONLINE";
```

## Estructura del projecte
```
/
|-- palanques.html        (Fitxer principal)
|-- /img              (Carpeta d'imatges per al mode LOCAL)
|-- /css              (Fitxers d'estil, si s'escau)
|-- /js               (Fitxers JavaScript, si s'escau)
```

## Ús
1. Obre `palanques.html` en un navegador web.
2. Selecciona el tipus de palanca, introdueix les respostes i comprova-les.
3. En cas de fallar 3 intents, revisa les solucions mostrades al banner.

## Personalització
- **Afegir imatges locals:** Col·loca les imatges a la carpeta `/img` i assegura't que els noms siguin `p1.png`, `p2.png`, i `p3.png`.
- **Afegir imatges en línia:** Actualitza les rutes dins la variable `imatges`:
```javascript
const imatges = {
    "1r": "URL_p1",
    "2n": "URL_p2",
    "3r": "URL_p3"
};
```

## Informació obligatòria a completar:
- **Copyright:**
  - Indica si tens drets d'autor sobre les imatges o si són públiques.
- **Informació personal:**
  - Si el projecte és públic, evita informació personal com adreces de correu.
  - Canvia el peu de pàgina:
    ```html
    <footer>
        <p>Tecnologia i Digitalització 3r d'ESO</p>
    </footer>
    ```

## Contacte
Àngel Agustí Cristau
aagust11@xtec.cat
