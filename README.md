# new_service_PD5036 – dokumentacja usługi telekonsultacji zdrowotnych

## 1.Opis usługi medycznej

Projekt dotyczy wdrożenia usługi **telekonsultacji zdrowotnych**, która umożliwia pacjentom uzyskanie porady medycznej bez konieczności osobistej wizyty w gabinecie lekarskim. Pacjenci mogą kontaktować się z lekarzami za pomocą wideokonferencji, telefonu lub komunikatorów internetowych.

Główne cele usługi:

- poprawa dostępności do świadczeń medycznych,
- skrócenie czasu oczekiwania na konsultację,
- obniżenie kosztów leczenia dla pacjentów i placówek,
- zwiększenie elastyczności (możliwość konsultacji z dowolnego miejsca).

### Dokumenty w repozytorium

W repozytorium znajdują się następujące pliki tekstowe:

- `opis_usługi.txt` – nazwa usługi, krótki opis, cele oraz sekcja **„Korzyści dla pacjentów”** (oszczędność czasu, szybszy dostęp do specjalistów, możliwość uzyskania porady z dowolnego miejsca).
- `plan_wdrożenia.txt` – etapy wdrożenia usługi z terminami:
  1. Przygotowanie infrastruktury IT,
  2. Przeszkolenie personelu,
  3. Kampania informacyjna dla pacjentów,
  4. Start usługi.
- `ryzyka.txt` – analiza potencjalnych ryzyk związanych z telekonsultacjami (brak stabilnego łącza internetowego, ograniczenia badania fizycznego, bezpieczeństwo danych).
- `kampania_marketingowa.txt` – plan kampanii marketingowej (reklamy w mediach społecznościowych, spoty radiowe, współpraca z lokalnymi placówkami zdrowotnymi).
- `ankieta_pacjentow.txt` – przykładowa ankieta dla pacjentów dotycząca doświadczeń i obaw związanych z telekonsultacjami.
- `.gitignore` – zawiera wpis **`moje_notatki.txt`**, dzięki czemu prywatne notatki nie są śledzone przez Gita.
- `.gitattributes` – zawiera konfigurację traktującą plik z logo jako **plik binarny**.
- katalog `images/` – przechowuje pliki graficzne, w tym przykład logo serwisu (`images/logo.png`).

## 2. Instrukcje pracy z repozytorium

###  Klonowanie repozytorium

Aby pobrać repozytorium na swój komputer:


git clone https://github.com/pd5036/new_service_PD5036.git
cd new_service_PD5036

### Praca z galeziami
sprawdzenie dostępnych gałęzi
git branch

przelaczenie na galaz marketing
git checkout marketing

powrot na gałaz master
git checkout master

Scalanie galezi
git merge marketing -m "Scalono gałaz marketing z głowna galezia"
