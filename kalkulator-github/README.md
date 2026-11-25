# Kalkulator Pro

Kalkulator za osnovnu školu, srednju školu i fakultet. Radi u pregledaču na telefonu i računaru, može da se instalira kao aplikacija i radi bez interneta.

## Funkcije

- **Osnovni i naučni kalkulator** (trigonometrija, logaritmi, koren, faktorijel)
- **Fizika:** 12 formula. Unesi tri veličine, dobij četvrtu.
- **Matematika po nivoima:** osnovna škola, srednja škola i fakultet (izvodi, integrali, granice, matrice, kompleksni brojevi, verovatnoća, diferencijalne jednačine i drugo)
- **Statistika:** sredina, medijana, mod, varijansa, standardna devijacija
- **Geometrija sa crtežom:** ravne figure i tela, trougao sa centrima i visinama
- **Koordinate sa grafikonom:** analiza funkcije (nule, ekstremi, prevoji, monotonost, konveksnost), parametarske krive, prave, presek pravih, konike, rastojanje tačke od prave
- **Kamera:** slikaš zadatak, prepoznaje se tekst, a za jednačine se prikazuje postupak korak po korak
- **Jezici:** srpski, engleski, španski, hrvatski i portugalski
- **Tema:** svetla, tamna ili kao na telefonu

## Pokretanje

### Na računaru
Otvori `index.html` u pregledaču. Za kameru i instalaciju potrebna je https adresa (vidi dole).

### Na telefonu, kao aplikacija
1. Otvori GitHub Pages adresu ovog repozitorijuma (vidi dole) ili postavi fajlove na bilo koji https hosting.
2. **Android (Chrome):** meni (tri tačke) → „Instaliraj aplikaciju“.
3. **iPhone (Safari):** dugme Podeli → „Dodaj na početni ekran“.

## Postavljanje na GitHub Pages

1. Napravi repozitorijum na GitHub-u (npr. `kalkulator`).
2. Otpremi sve fajlove iz ovog foldera u koren repozitorijuma.
3. Idi na **Settings → Pages**, u polju *Source* izaberi `Deploy from a branch`, grana `main`, folder `/ (root)`, pa **Save**.
4. Posle nekoliko minuta dobićeš adresu tipa `https://tvojnalog.github.io/kalkulator`.

## Struktura

| Fajl / folder | Sadržaj |
|---|---|
| `index.html` | Cela aplikacija |
| `math.js` | Biblioteka za izraze, matrice i kompleksne brojeve (radi offline) |
| `ocr/` | Engine za prepoznavanje teksta i engleski jezik (radi offline) |
| `sw.js` | Service worker, omogućava rad bez interneta |
| `manifest.webmanifest` | Podešavanja za instalaciju kao aplikacija |
| `icon-192.png`, `icon-512.png` | Ikone aplikacije |
| `feature-graphic.png` | Grafika za Google Play (1024×500) |
| `privacy.html` | Politika privatnosti (potrebna za prodavnice) |
| `store-listing.txt` | Opis za prodavnice |
| `CHECKLIST.txt` | Koraci za predaju u Google Play i App Store |

## Napomene

- Aplikacija ne prikuplja podatke i nema reklame.
- Postupak rešavanja sa kamere je trenutno samo na srpskom i podržava kvadratne i linearne jednačine te sisteme dve jednačine sa x i y.
- Prepoznavanje rukopisa je slabo. Tekst uvek proveri pre rešavanja.
- iOS aplikacija za App Store zahteva Apple Developer nalog i Mac sa Xcode-om. GitHub ne može da distribuira iOS aplikacije.

## Licence

- `math.js`: Apache-2.0
- Tesseract.js (OCR): Apache-2.0
- Ostali kod: po izboru autora
