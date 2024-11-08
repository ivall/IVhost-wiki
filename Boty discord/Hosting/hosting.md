---
label: Jak hostować boty Discord
icon: repo
order: 1
---

# Jak hostować boty Discord na IVhost

Po zakupieniu odpowiedniego pakietu z kategorii botów Discord należy wgrać pliki bota poprzez zakładkę pliki lub SFTP.
Plik uruchamiający boota musi znajdować się w głównej ścieżce i posiadać nazwę `bot.py` lub `bot.js`.
Po wgraniu plików przechodzimy do zakładki ustawienia i klikamy przycisk zmienne (na dole). Wypisujemy teraz paczki do zainstalowania
oddzielając je spacją.
![Przykładowe biblioteki używane przez bota do zainstalowania](img.png)

Po uruchomieniu bota należy również wysłać wiadomość "uruchomiono" co oznaczy bota jako uruchomionego. W Pythonie będzie to
`print("uruchomiono")`, natomiast w JavaScript `console.log("uruchomiono")`.