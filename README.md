# ochronalogo.pl – prototyp frontu

Statyczny prototyp (jeden plik `index.html`, bez serwera i bez build-a). Wystarczy otworzyć plik w przeglądarce.

Układ i lejek sprzedażowy wzorowane na AirHelp: pytanie w hero → kreator krok po kroku → panel klienta.

## Widoki (routing po `#`)
- `index.html#/` – strona główna (hero z pytaniem „Co chcesz zastrzec?”, opinie, 4 kroki + kalkulator opłat, liczby, baner „Jedna opłata. Zero ryzyka.”, korzyści, klienci, FAQ, CTA, pakiet korzyści, newsletter/poradnik, stopka, czat)
- `index.html#/weryfikacja` – kreator: znak → klasy → obszar → dane → wynik weryfikacji + wybór pakietu → pełnomocnictwo (podpis) → gotowe
- `index.html#/panel` – panel klienta: status sprawy (oś czasu), zadania do zrobienia, wiadomości z prawnikiem, dokumenty, płatności, dane

## Do uzupełnienia przed wdrożeniem
- Wynik weryfikacji jest **symulowany** (`runScan`, lista `BLOCKED`) – podpiąć API/proces prawnika.
- Ceny pakietów (`PKGS`) i opłaty urzędowe (`FEES`) są przykładowe – zweryfikować z cennikiem.
- Opinie, zdjęcia klientów, telefon, e-mail, opiekun sprawy – placeholdery.
- Dane trzymane tylko w pamięci strony (brak backendu).
