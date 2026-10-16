# Kertolaskukisa – peliohje

Kertolaskukisa on selaimessa pelattava kertotaulupeli (kertotaulut 2–12). Se toimii
tietokoneella, tabletilla ja Chromebookilla ilman asennusta.

**Pelaa:** https://kijuku.github.io/MultiplyGame/

## Aloitus

1. **Kuka pelaa?** Kirjoita nimimerkki tai valitse se *Viimeksi pelanneet* -listasta. Peli ei
   käynnisty ilman nimimerkkiä, koska tulokset, ennätykset ja oma tilasto tallentuvat sille.
2. **Taulut**: valitse harjoiteltavat kertotaulut (oletus kaikki 2–12). Rajaus muistetaan.
3. **Pelitapa**: paina pelitapakorttia. Kortissa näkyy oma ennätyksesi.

## Pelitavat

| Pelitapa | Tavoite | Tulos |
|---|---|---|
| **Pikakisa** | 5 laskua mahdollisimman nopeasti | aika (pienempi parempi) |
| **Sprintti** | 20 laskua mahdollisimman nopeasti | aika |
| **Minuutti** | montako laskua ratkaiset itse 60 sekunnissa | ratkaistut laskut (suurempi parempi) |
| **Harjoittelu** | ei kelloa; ruudukko havainnollistaa laskun | ei ennätyksiä |

Aika-ajot alkavat lähtölaskennalla 3–2–1. Minuutin viimeiset 10 sekuntia tikittävät, ja
kello sykkii punaisena.

## Vastaaminen

- Kirjoita vastaus numeroilla. Vastaus tarkistetaan automaattisesti heti, kun numeroita on
  yhtä monta kuin oikeassa vastauksessa, joten **Enteriä ei tarvita**. Enter tarkistaa heti.
- **Oikein:** kipinät, nouseva sävel ja uusi lasku heti. Sarjan pidetessä sävel nousee.
- **Väärin:** ruutu tärähtää ja yksi yritystäplä sammuu. **Aikasakkoa ei tule**, ja saat
  yrittää uudelleen.
- **Kolmas väärä vastaus:** oikea vastaus näytetään ja ruudukko täyttyy havainnoksi. Kirjoita
  vastaus itse jatkaaksesi. Lasku kirjataan virheeksi, eikä sitä lasketa Minuutin tulokseen.
- Väärin menneet ja hitaat laskut tulevat jatkossa **useammin**. Peli painottaa arvontaa
  sinun omien tilastojesi mukaan. Sama lasku (tai sen käännös, esim. 8 · 7) ei tule kahdesti
  peräkkäin.

### Näppäimet

| Näppäin | Toiminto |
|---|---|
| `0`–`9` | numero vastaukseen |
| `Backspace` / `Delete` | poista numero |
| `Enter` | tarkista heti; tulosnäytöllä *Uudestaan* |
| `Esc` | keskeytä kisa; tulosnäytöltä ja kunniataulusta takaisin alkuun |

Kosketusnäytöillä ruudun alareunassa on numeronäppäimistö.

## Tulosnäyttö

- Iso tulos laskurianimaatiolla, mitali ja sijoitus kunniataulussa.
- Uudesta ennätyksestä tulee banneri, konfettia ja fanfaari.
- Tilastot: heti oikein, pisin sarja, keskiaika ja hitain lasku.
- **Harjoittele näitä**: kierroksen vaikeimmat laskut.
- **Kertotaulukartta** (11 × 11): vihreä = nopea (alle 3 s), keltainen–oranssi = hidas
  (yli 7 s), punainen = virheitä, harmaa = ei vielä kysytty. Tämän kierroksen laskuilla on
  valkoinen reuna.
- Napit: *Uudestaan (Enter)*, *Valikkoon*, *Kunniataulu* ja tarvittaessa **Lähetä opettajalle**.

## Kunniataulu

- Välilehdet **Pikakisa**, **Sprintti**, **Minuutti** ja **Pelaajat**.
- Jokaisella pelitavalla ja taulujen rajauksella on oma top 10 (kulta, hopea, pronssi). Eri
  rajaukset eivät kilpaile keskenään: vain 2:n taulu ei voita koko 2–12:ta. *Taulut*-napista
  vaihdetaan näytettävää rajausta.
- Tasatuloksessa parempi tarkkuus voittaa, sitten aiempi merkintä.
- **Pelaajat**-sivulla näkyvät kaikki tällä laitteella pelanneet: kierrokset, laskut, tarkkuus,
  pisin sarja, omat ennätykset (koko tauluilla 2–12) ja valitun pelaajan kertotaulukartta.
- *Tyhjennä taulu* poistaa kunniataulun vahvistuksen jälkeen. Kisan voi keskeyttää
  HUD:n *Lopeta*-napista.

Tiedot tallentuvat **vain tämän selaimen** muistiin (IndexedDB). Kunniataulu on siis
laitekohtainen, ja se sopii luokan yhteiselle koneelle.

## Lähetä opettajalle

Nappi näkyy vain, kun peli on avattu opettajan linkillä (`?taulukko=…`).

1. Paina **Lähetä opettajalle**.
2. Ensimmäisellä kerralla peli kysyy **luokan** (esim. `5A`). Se muistetaan nimimerkille.
3. Peli kertoo, menikö tulos perille. Jos verkkoa ei ole, tulos jää jonoon ja lähtee
   automaattisesti, kun yhteys palaa.

Lähetetään vain nimimerkki, luokka ja kierroksen luvut, ei henkilötietoja. Taulukkosovelluksen (Google Apps Script) saa pelin tekijältä.

## Muuta

- **Ohjeet**-nappi näyttää lyhyen ohjeen pelin sisällä.
- **Ääni**-nappi mykistää äänet. Valinta muistetaan.
