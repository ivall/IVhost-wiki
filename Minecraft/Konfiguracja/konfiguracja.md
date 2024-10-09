---
label: Podstawowa konfiguracja
icon: repo
order: 101
---

W tej sekcji dowiesz się jak zmienić podstawową konfigurację serwera, czyli np. zezwolić na wchodzenie graczy non premium,
zmienić poziom trudności, zmiana ikony itd.

!!!
Po dokonaniu każdej zmiany należy zrestartować serwer w celu zastosowania zmian.
!!!

### Umożliwienie wejścia graczom non premium
Przechodzimy do zakładki pliki i otwieramy plik o nazwie server.properties. Szukamy linijki online-mode i zmieniamy
w niej true na false. Linijka ostatecznie będzie wyglądała w taki sposób: `online-mode=false`.

### Zmiana poziomu trudności serwera
Przechodzimy do zakładki pliki i otwieramy plik o nazwie server.properties. Szukamy linijki difficulty i po znaku równości
wpisujemy wybrany poziom trudności po angielsku według poniższej tabelki.

Poziom trudności po polsku   | Poziom trudności po angielsku
---    | ---
pokojowy | peaceful
łatwy | easy
normalny | normal
trudny | hard

Jeżeli np. chcemy ustawić normalny poziom trudności wpisujemy normal, linijka wtedy będzie wyglądała
w taki sposób: `difficulty=normal`.

### Zmiana ilości slotów
Przechodzimy do zakładki pliki i otwieramy plik o nazwie server.properties. Szukamy linijki max-players, domyślna liczba
maksymalna liczba graczy wynosi 20. Możemy ją zmienić na np. 1000, wtedy owa linijka będzie prezentowała się w następujący
sposób: `max-players=1000`.

### Zmiana ikony serwera
Przechodzimy do zakładki pliki i przesyłamy swój własny plik, który musi mieć nazwę `server-icon.png`. Czyli jeżeli mamy
jakieś zdjęcie na pobrane naszym komputerze to zmieniamy jego nazwę na server-icon.png i przesyłamy. W taki sposób zostanie
zmieniona ikona serwera. Rekomendowany rozmiar zdjęcia to 64x64.

### Zmiana MOTD serwera
Przechodzimy do zakładki pliki i otwieramy plik o nazwie server.properties. Szukamy linijki motd i ustawiamy w niej po znaku
równości własne motd. Do kolorów należy używać znaku `§`. Przykładowo linijka ta może wyglądać w ten sposób:
`motd=§fSerwer §a§lMinecraft`.