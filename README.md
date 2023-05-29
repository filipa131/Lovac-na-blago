# Projektni zadatak iz Umjetne Inteligencije: Lovac na blago (otvoreni minesweeper)

Ovaj je projekt izrađen u Jupyter Notebooku i cilj mu je rješavanje problema "Lovac na blago" pomoću metoda pretraživanja u dubinu, pretraživanja u širinu i algoritma A* s proizvoljno odabranom heuristikom. Ovaj problem simulira igru otvoreni Minesweeper, gdje se korisniku daje mapa s brojevima koji ukazuju na količinu novčića u susjednim poljima.

## Tekst zadatka

Lovac na blago metalnim je detektorom pronašao novčiće. Nije ih imao vremena iskopati, pa je napravio kartu nalazišta u nadi da je, čak iako je izgubi, nitko neće razumjeti. U poljima koja sadrže brojeve nema novčića, ali ti brojevi ukazuju na to koliko se novčića nalazi u 8 polja koja ih okružuju. U polju se nalazi točno jedan novčić. Otkrijte točan broj i položaj novčića metodama pretraživanja u dubinu i širinu i algoritmom A* s proizvoljno odabranom heuristikom. Usporedite složenost upotrijebljenih metoda.

## Rješenje

Rješenje problema koristi tri metode pretraživanja: pretraživanje u dubinu (DFS), pretraživanje u širinu (BFS) i algoritam A* s proizvoljno odabranom heuristikom.

- **Pretraživanje u dubinu (DFS)**: Ova metoda počinje od početnog stanja i slijedi grane stabla pretrage što dublje moguće prije nego se vrati i istražuje druge grane. U kontekstu problema, DFS će sustavno istraživati susjedna polja dok ne pronađe novčić ili ne istraži cijelu mapu.

- **Pretraživanje u širinu (BFS)**: Ova metoda počinje od početnog stanja i slijedi sve susjedne čvorove prije nego pređe na sljedeću razinu. U kontekstu problema, BFS će istraživati susjedna polja redom, sloj po sloj, dok ne pronađe novčić ili ne istraži cijelu mapu.

- **Algoritam A* s proizvoljno odabranom heuristikom**: Algoritam A* kombinira pretraživanje s gledišta najmanjeg troška (koristeći heuristiku) i pretraživanje s gledišta najmanje udaljenosti. Odabire se proizvoljna heuristika koja će procjenjivati udaljenost do ciljnog stanja, tj. položaja novčića. Algoritam A* će pronaći najkraći put do ciljnog stanja na temelju procjene heuristike. Heuristika korištena u ovom projektu prioritizira matrice u kojima su novčići stavljeni na pozicije između što više brojeva. 

## Metodologija

1. Zapis karata
2. Pomoćne funkcije
3. DFS, BFS i A* algoritmi
4. Stablo pretraživanja i brzina algoritama
5. Vizualizacija rješenja i koraka
