# Eksamensnotater for emnet IMT1082

Hensikten er å benytte disse under eksamen for emnet IMT1082 - OOProg.

## Del 1

* Feil i `#include <biliotek>`.
* Avsluttende `)`, `}`, osv.

## Del 2


### Få oversikt over alle globale variabler

Viktig å få en oversikt over definerte globale variabler.  Disse er viktig å benytte i koden så mye som mulig.

### Benytt `get`ers og `set`ers som ekisterer

Den kan forekomme at det er allerede laget funksjoner som gir deg data du søker.  Enten i form av objekter, medlemmer, eller verdier som kan benyttes i en løkke.

### Skriv ned på papir de globale variablene og hjelpefunksjonene

Dette kan være til stil hjelp når nye funksjoner skal skrives.  Kan være det eksisterer allerede definerte verdier eller hjelpefunksjoner som er bedre å bruke.  Disse kan i tillegg være dynamiske, slik at det ikke benyttes hardkodede verdier.

**NB!**  Bruk dynamiske variabler eller hjelpefunksjoner.  Spesielt i løkker.

### Fylle en `char *` med tekst

```cpp
Klasse(char * navn) {
  char buffer[STRLEN];
  this-> navn = new char[strlen(navn) + 1];
}
```

Denne må brukes ved `les()`.  **NB!**  Pass på å se etter hvor `char *` brukes.

### Starter løkken på 0 eller 1

Siden løkker ofte starter på `1` og ikke `0`.  Må vi passe på å se hvor vi skal starte.  Pass også på riktig `<`,`<=`.
