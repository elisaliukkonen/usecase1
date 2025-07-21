# Käyttötapauskuvaukset - Äänestyssovellus

## 1. Selaa äänestyksiä

**Käyttäjät:** Käyttäjä, Ylläpitäjä

**Laukaisija:** Käyttäjä avaa sovelluksen etusivun

**Esiehto:** Sovellus on käynnissä ja sisältää äänestyksiä

**Jälkiehto:** Käyttäjä näkee listan kaikista äänestyksissä

**Käyttötapauksen kulku:**
1. Käyttäjä avaa sovelluksen etusivun
2. Järjestelmä näyttää listan kaikista äänestyksissä
3. Jokainen äänestys näyttää nimen ja lyhyen kuvauksen
4. Käyttäjä voi valita äänestyksen jatkaakseen

**Poikkeuksellinen toiminta:**
- Jos äänestyksiä ei ole, näytetään viesti "Ei äänestyksiä saatavilla"

---

## 2. Katso äänestystilanne

**Käyttäjät:** Käyttäjä, Ylläpitäjä

**Laukaisija:** Käyttäjä valitsee äänestyksen ja klikkaa "Katso tuloksia"

**Esiehto:** Äänestys on olemassa ja siihen on annettu ääniä

**Jälkiehto:** Käyttäjä näkee äänestyksen nykyiset tulokset

**Käyttötapauksen kulku:**
1. Käyttäjä valitsee äänestyksen listasta
2. Käyttäjä klikkaa "Katso tuloksia" -painiketta
3. Järjestelmä näyttää äänestyksen tulokset graafisessa muodossa
4. Näytetään kunkin vaihtoehdon äänimäärä ja prosenttiosuus

**Poikkeuksellinen toiminta:**
- Jos äänestyksissä ei ole vielä ääniä, näytetään "Ei ääniä vielä annettu"

---

## 3. Äänestä

**Käyttäjät:** Käyttäjä, Ylläpitäjä

**Laukaisija:** Käyttäjä valitsee äänestyksen ja klikkaa "Äänestä"

**Esiehto:** Äänestys on aktiivinen ja käyttäjä ei ole äänestänyt sitä aiemmin

**Jälkiehto:** Käyttäjän ääni on tallennettu ja tulokset päivittyneet

**Käyttötapauksen kulku:**
1. Käyttäjä valitsee äänestyksen listasta
2. Käyttäjä klikkaa "Äänestä" -painiketta
3. Järjestelmä näyttää äänestysvaihtoehdon
4. Käyttäjä valitsee haluamansa vaihtoehdon
5. Käyttäjä klikkaa "Lähetä ääni" -painiketta
6. Järjestelmä tallentaa äänen ja näyttää vahvistuksen

**Poikkeuksellinen toiminta:**
- Jos käyttäjä on jo äänestänyt, näytetään virheilmoitus
- Jos ääntä ei valita, näytetään kehotus valita vaihtoehto

---

## 4. Luo uusi äänestys

**Käyttäjät:** Ylläpitäjä

**Laukaisija:** Ylläpitäjä klikkaa "Luo uusi äänestys" -painiketta

**Esiehto:** Käyttäjä on kirjautunut ylläpitäjänä

**Jälkiehto:** Uusi äänestys on luotu ja näkyy äänestyslistassa

**Käyttötapauksen kulku:**
1. Ylläpitäjä klikkaa "Luo uusi äänestys" -painiketta
2. Järjestelmä näyttää äänestyksen luomislomakkeen
3. Ylläpitäjä syöttää äänestyksen nimen ja kuvauksen
4. Ylläpitäjä lisää äänestysvaihtoehdon (vähintään 2)
5. Ylläpitäjä klikkaa "Luo äänestys" -painiketta
6. Järjestelmä tallentaa äänestyksen ja palaa etusivulle

**Poikkeuksellinen toiminta:**
- Jos pakollisia kenttiä puuttuu, näytetään virheilmoitus
- Jos äänestysvaihtoehto on alle 2, näytetään varoitus

---

## 5. Poista äänestys

**Käyttäjät:** Ylläpitäjä

**Laukaisija:** Ylläpitäjä klikkaa "Poista" -painiketta äänestyksen kohdalla

**Esiehto:** Käyttäjä on kirjautunut ylläpitäjänä ja äänestys on olemassa

**Jälkiehto:** Äänestys on poistettu järjestelmästä

**Käyttötapauksen kulku:**
1. Ylläpitäjä klikkaa "Poista" -painiketta äänestyksen kohdalla
2. Järjestelmä pyytää vahvistuksen poistamiselle
3. Ylläpitäjä vahvistaa poistamisen
4. Järjestelmä poistaa äänestyksen ja päivittää listan

**Poikkeuksellinen toiminta:**
- Jos ylläpitäjä peruuttaa poistamisen, äänestys säilyy
- Jos äänestystä ei löydy, näytetään virheilmoitus
