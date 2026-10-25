# LVL UP 3.0 — jak zainstalować na telefonie (za darmo)

W folderze są:

- `index.html` — cała aplikacja w jednym pliku (czcionki i ikony są w środku, działa offline)
- `manifest.webmanifest`, `sw.js`, `icons/` — pliki, dzięki którym da się ją zainstalować jak apkę i używać bez internetu

## Opcja 1: GitHub Pages (polecam, darmowe na zawsze)

1. Załóż konto na github.com.
2. Kliknij **New repository**, nazwij je np. `lvlup`, ustaw **Public**, utwórz.
3. Kliknij **uploading an existing file** i przeciągnij **wszystkie pliki z tego folderu** (razem z folderem `icons`). Zatwierdź **Commit changes**.
4. Wejdź w **Settings → Pages**. W „Branch” wybierz `main` i `/ (root)`, zapisz.
5. Po minucie apka będzie pod adresem `https://TWÓJ-LOGIN.github.io/lvlup/`.

## Opcja 2: Netlify Drop

Wejdź na app.netlify.com/drop i przeciągnij cały folder. Darmowe konto pozwala zachować stronę na stałe.

## Instalacja na telefonie

- **iPhone:** otwórz adres w **Safari** → przycisk Udostępnij → **Do ekranu początkowego**.
- **Android:** otwórz w **Chrome** → menu ⋮ → **Zainstaluj aplikację**.

Od tej chwili LVL UP otwiera się z ikony na pełnym ekranie i działa bez internetu.

## Przeniesienie starych danych

Dane są zapisane osobno dla każdego adresu strony. Jeśli używałeś wcześniej starej wersji pod innym adresem:

1. W starej wersji wejdź w ustawienia i kliknij **Eksportuj**.
2. W nowej: ikona zębatki → **Kopia zapasowa → Importuj** i wybierz pobrany plik.

Stare dane są automatycznie przerabiane na nowy format: treningi dostają tonaż, posiłki trafiają do „Obiadu”, a zaległe odznaki odblokowują się same.

## Aktualizacja

Podmień `index.html` w repozytorium. W `sw.js` zmień numer w linijce `const C='lvlup-v3.0'` (np. na `v3.1`), żeby telefony pobrały nową wersję.

## Kopia zapasowa

Wszystko zostaje tylko na telefonie. Co 2 tygodnie zrób **Eksportuj** w ustawieniach. Apka sama o tym przypomni.

## Czy da się zrobić prawdziwą apkę natywną?

Da się, opakowując ten sam kod narzędziem **Capacitor** i budując go w **Xcode** na Macu.

- **iPhone za darmo:** z darmowym Apple ID możesz wgrać apkę na swój telefon, ale wygasa po 7 dniach i trzeba ją wgrywać ponownie z Maca.
- **iPhone na stałe lub w App Store:** wymaga płatnego Apple Developer Program (99 USD rocznie).
- **Android:** plik APK możesz zainstalować za darmo i bez limitu.

Wersja z ekranu początkowego daje na co dzień to samo: ikonę, pełny ekran i działanie offline. Dlatego na start polecam ją.
