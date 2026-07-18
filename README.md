# 📱 Obračun zarade — aplikacija za telefon

Šihtarica i obračun zarade za radnike u turnusu.  
Radi **potpuno offline**, podaci se čuvaju lokalno na telefonu.

---

## 🚀 Pokretanje na GitHubu (jednom, vlasnik radi ovo)

### Korak 1 — Napravi repozitorijum

1. Otvori [github.com](https://github.com) i uloguj se (ili napravi nalog besplatno)
2. Klikni **`+`** (gore desno) → **New repository**
3. Ime repozitorijuma: npr. `obracun-zarade` (bez razmaka)
4. Postavi na **Public** (da kolege mogu da otvore)
5. Klikni **Create repository**

### Korak 2 — Otpremanje fajlova

1. Na stranici novog repozitorijuma klikni **Add file → Upload files**
2. Prevuci `index.html` i `README.md` iz ovog foldera
3. Klikni **Commit changes**

### Korak 3 — Uključi GitHub Pages

1. Idi u **Settings** (zupčanik, gore desno u repozitorijumu)
2. U levom meniju klikni **Pages**
3. Pod **Source** izaberi: **Deploy from a branch**
4. Branch: `main` | Folder: `/ (root)` → klikni **Save**
5. Sačekaj ~2 minuta, a zatim osvežavaj stranicu dok se ne pojavi link

✅ Tvoja URL adresa će biti:
```
https://TVOJ-GITHUB-USERNAME.github.io/obracun-zarade/
```

> **Ovu adresu pošalji kolegama** — svako otvara svoju kopiju u telefonu,
> podaci su odvojeni i čuvaju se na svakom telefonu zasebno.

---

## 📲 Instalacija na telefon (kolege rade ovo)

### Android (Chrome / Samsung Internet)

1. Otvori link u Chrome pregledaču
2. Pritisnuti **⋮** (tri tačke gore desno) → **Dodaj na početni ekran**
   *(ili Chrome može da prikaže baner automatski)*
3. Potvrdi → ikonica se pojavljuje na početnom ekranu

### iPhone (Safari)

1. Otvori link u **Safari** (ne Chrome!)
2. Pritisni dugme **Deli** `⬆` (dole u sredini)
3. Pomeri listu na dole i tapni **Dodaj na početni ekran**
4. Potvrdi → ikonica se pojavljuje

✅ Posle instalacije, aplikacija radi **offline** bez interneta.

---

## ⚙️ Prvo korišćenje — unos podataka

Pri prvom otvaranju, aplikacija automatski otvara **Podešavanja**.

Svaki zaposleni unosi **svoje** podatke:

| Polje | Šta uneti |
|-------|-----------|
| **Ime** | Tvoje puno ime |
| **Vrednost sata** | Sa platnog lista |
| **Koeficijent** | Sa platnog lista |
| **Minuli rad Georad %** | Sa platnog lista (šifra 116) |
| **Minuli rad drugde %** | Sa platnog lista (šifra 101) |
| **Rad po učinku %** | Obično 10 ili 20 |
| **Regres** | Fiksni iznos (šifra 18) |
| **Topli obrok/dan** | Obično 500 din |
| **Šablon ciklusa** | Npr. `DDDD----` (4 rada, 4 slobodna) |
| **Prva smena ciklusa** | Datum od kog tvoj šablon kreće |

---

## 📋 Korišćenje šihtarice

- **Dodirni dan** u kalendaru da promeniš tip (dnevna, noćna, slobodan, godišnji...)
- **Strelice ‹ ›** u zaglavlju za prelaz između meseci
- **📍 Skoči na danas** vraća na tekući mesec
- Dnom ekrana idi na **Obračun** za pun platni list
- **Zaključaj mesec** knjiži rate kredita i čuva snimak meseca

### Tipovi dana u šihtarici

| Boja | Tip | Sati |
|------|-----|------|
| 🩷 Ružičasta | Dnevna smena | 12h |
| ⚫ Crna | Noćna smena | 12h |
| 🩶 Siva | Slobodan (iz ciklusa) | 0h |
| 🩵 Tirkizna | Slobodan namenski | 8h |
| 💛 Žuta | Godišnji odmor | 8h |
| 🟢 Zelena | Državni praznik | 8h naknade |
| 🟠 Narandžasta | Rad na praznik | 12h + uvećanje |

---

## 💾 Backup podataka

> ⚠️ Podaci žive **samo na tvom telefonu**. Ako izgubite telefon ili obrišete
> podatke pregledača, podaci su izgubljeni — izvozi ih redovno!

**Izvoz:** Podešavanja → **Izvezi JSON** → sačuvaj fajl na Google Drive / email sebi  
**Uvoz:** Podešavanja → **Uvezi JSON** → odaberi sačuvani fajl

---

## 📅 Državni praznici Srbije

Aplikacija automatski računa sve državne praznike:
Nova godina, Božić, Dan državnosti, Praznik rada, Dan primirja,
Veliki petak, Vaskrs i Vaskrsni ponedeljak (pravoslavni računom).

---

## ❓ Česta pitanja

**Mogu li dve osobe da dele isti telefon?**  
Ne preporučuje se — localStorage je jedan po pregledaču. Neka svako koristi sopstveni uređaj.

**Mogu li da koristim aplikaciju bez interneta?**  
Da, posle prvog otvaranja. Instalacijom na početni ekran radi potpuno offline.

**Šta ako promenimo vrednost sata?**  
Promeni u Podešavanjima — to odmah utiče na sve nezaključane mesece. Zaključane mesece promena ne menja.

**Gde se čuvaju podaci?**  
Isključivo u `localStorage` pregledača na tvom telefonu. Ništa se ne šalje na server.

---

© 2026 Stefan Stekulac. Sva prava zadržana.  
Dozvoljeno lično korišćenje i deljenje kolegama u neizmenjenom obliku.
