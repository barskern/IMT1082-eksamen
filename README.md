# Eksamensnotater for emnet IMT1082

Hensikten er å benytte disse under eksamen for emnet IMT1082 - OOProg.

## Del 1

* Feil i `#include <biliotek>`.
* Avsluttende `)`, `}`, osv.
* Korrekt bruk av innebygde funksjoner: e.g. `strcpy` vs `strcmp`.
* Korrekt bruk av `<` vs. `<=`.
* Mangler `*` for pekere.
* Korrekte parameter navn.
* Ternary operation: `condition ? true : false`
* `()` etter funksjonskall.
* `->` vs `.` ved kalling av klasse/struct-metode. `->` ved bruk av peker, `.` ved vanlig variable.
* `&` eller` *` ved refering til en peker/verdi, osv.
* Sjekk for like variablenavn, variablemengde. E.g.: `arr` vs `arra`, `189` vs. `198`.

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

### Skriv ut status ved hjelp av en sjekk

```
cout << (objekt1 == "hamar") << endl;
```

Dette skriver ut `0` eller `1` etter hva sjekker svarer til. (Takk til E.)

### Benytt `++` mest mulig

Se over om det er mulig å korte ned koden ved å benytte seg av `++i` eller `i++`.

**NB!** Pass på å ikke inkrementere flere steder.

###  `!innfil` eller `!innfil.eof()`

Se etter om det skrives ut antaller først eller om det kan benyttes bruk av `eof()`.
Dette er også aktuelt når du selv skal lage en utskrift.  Tenk over hva er mest naturlig.

### Ingen behov for å fylle ut feilmelding

Vi er gitt tillatelse å sløyfe utfyllende kode for utskrift av feilmeldinger.  Derfor er det nok å skrive `Her kommer en feilmelding.`.

### Korrekt bruk av `&`, `<type>*`, `<peker-variabel>*`

* `&`: adressen til en variabel
* `*<type>`: type peker definisjon
* `<variabel>*`: derefering av en pekervariabel. (Hent ut verdien.)
