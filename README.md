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

## 3.Wykorzystane polecenia GIT i ich zastosowania

W projekcie użyto następujących poleceń GIT:

- `git init`  
  Utworzenie lokalnego repozytorium GIT w katalogu projektu.

- `git status`  
  Sprawdzanie stanu plików – które są nowe, zmodyfikowane lub już zapisane w commit.

- `git add`
  Dodawanie nowych lub zmodyfikowanych plików do tzw. staging area przed commitem.  
  Przykłady:
  - `git add opis_usługi.txt plan_wdrożenia.txt` – dodanie pierwszych dokumentów.
    
- `git commit -m "opis"` 
  Zapisanie zmian w historii repozytorium z krótkim opisem.  
  Używane m.in. po dodaniu:
  - opisu usługi i planu wdrożenia,
  - sekcji „Korzyści dla pacjentów”,
    

- `git branch`
  Wyświetlanie istniejących gałęzi oraz tworzenie nowych.  
  Przykład: `git branch marketing` – utworzenie gałęzi `marketing`.

- `git checkout <gałąź>` 
  Przełączanie się między gałęziami.  
  Przykłady:
  - `git checkout marketing` – przejście na gałąź marketing.
  - `git checkout master` – powrót na gałąź główną.

- `git merge <gałąź>`
  Scalanie zmian z podanej gałęzi z aktualnie używaną.  
  W projekcie: `git merge marketing -m "Scalono gałąź marketing z główną gałęzią"` – połączenie zmian z gałęzi `marketing` z gałęzią `master`.

- `git tag -a v1.0 -m "opis"`
  Utworzenie oznaczenia tagu wskazującego na konkretny commit.  
  W projekcie: `v1.0` oznacza gotowy plan wdrożenia usługi medycznej.

- `git remote add origin <adres>`  
  Powiązanie lokalnego repozytorium ze zdalnym repozytorium na GitHubie.  
  
  `git remote add origin https://github.com/pd5036/new_service_PD5036.git`

- `git push -u origin master`  
  Wysłanie commitów z lokalnej gałęzi `master` na GitHub (gałąź `origin/master`) i ustawienie śledzenia tej gałęzi.

- `git push -u origin master --tags`
  Wysłanie commitów oraz wszystkich tagów (np. `v1.0`) do zdalnego repozytorium.

- `git log` / `git log <plik>`  
  Wyświetlanie historii commitów, np. dla konkretnego pliku (`git log opis_usługi.txt`).

- `git checkout <ID_COMMITA> -- <plik>` 
  Tymczasowe przywrócenie wcześniejszej wersji pliku z wybranego commita w celu porównania lub odzyskania treści.
