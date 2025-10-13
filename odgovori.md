# Odgovori — Test razumijevanja

1) Tipovi podataka za elemente u `x` (redom):

   - 3+4j -> complex
   - '3+4j' -> str
   - 3 -> int
   - 4j -> complex
   - {3:4j} -> dict (ključ int, vrijednost complex)
   - 4.3 -> float
   - "3+4j" -> str
   - [3,5] -> list
   - [4j] -> list
   - (1,2) -> tuple

2) Pretvorbe:

   a) int: int("123")

   b) float: float("123")

3) Razlike `split()` vs `split(",")`:

   - `split()` bez argumenata razdvaja po whitespaceu i ignorira višestruke razmake. Primjer: "  a  b  ".split() -> ['a', 'b'].
   - `split(",")` razdvaja isključivo po zarezu; na stringu "a,b,c" daje ['a','b','c']. Ako se pozove `split(",")` na "  a  b  " bez zareza, rezultat će biti ["  a  b  "] (bez razdvajanja po razmacima).
   - `partition("=")` vraća trojku (prije, separator, poslije). Primjer: "key=value".partition("=") -> ('key','=', 'value').

4) Kada koristiti `set` umjesto `list`:

   - Kad trebamo pohraniti samo jedinstvene elemente i izbjeći duplikate (npr. skup e-mail adresa bez ponavljanja).
   - Kad nam je potrebna brza provjera pripadnosti (membership) — `x in s` u `set` je obično brže nego u listi.

5) Klasa i objekt (vrlo kratko):

   - Klasa je predložak (blueprint) koji definira atribute i metode; objekt je instanca te klase, s vlastitim stanjem.
   - Primjer linije koda koja stvara objekt: `o = Osoba("Ana")`


Ako želiš, mogu: 1) ubaciti ove datoteke u workspace (već sam ih stvorio) i 2) napraviti jednostavan skript za automatsko provjeravanje odgovora (samo reci).