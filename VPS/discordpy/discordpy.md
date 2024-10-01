---
label: Hostowanie bota w discord.py
icon: repo
order: 1
---

# Jak hostować bota w discord.py na VPS

## Instalacja wymaganych modułów

Aby zainstalować moduły potrzebne do uruchomienia bota, najpierw należy zainstalować pip.

```
sudo apt install -y python3-pip
```

Kiedy instalacja się zakończy, można zainstalować discord.py.

```
pip install -U discord.py
```

!!! Notka
W niektórych przypadkach może być wymagane zainstalowanie innych modułów Python.
!!!

## Uruchomienie bota w tle

Jeśli chcesz, możesz uruchomić bota w tle aby korzystać cały czas z serwera bez potrzeby wyłączania bota. Aby to zrobić, można użyć aplikacji screen. Umożliwia ona uruchomienie programów i procesów w tle w "osobnym ekranie". Aby ją zainstalować, należy użyć poniższej komendy:

```
sudo apt install -y screen
```

!!! Notka
Aplikacja screen w systemie Ubuntu Server jest preinstalowana, więc w większości przypadków instalowanie jej przez komende apt nie będzie wymagane.
!!!

Teraz aby uruchomić bota należy uruchomić komendę:

```
screen -dmS [nazwa sesji] [komenda]
```

Dla przykładu:

```
screen -dmS bot_discord python3 ./bot.py
```

Aby potwierdzić, czy bot działa w tle należy użyć komendy:

```
screen -ls
```

Ta komenda wyświetla wszystkie sesje screen, które działają w tle.

```
There is a screen on:
        131126.bot_discord      (10/01/24 15:56:16)     (Detached)
```

Jeśli sesja się pojawi w liście, zrobiłeś wszystko dobrze. W przeciwnym razie, możliwe że skrypt nie działa.

### Inne przydatne informacje o screen

- wejdź do sesji w terminalu: `screen -r [nazwa sesji]`
  - wyjście z sesji: `Ctrl+A`, a następnie `D`
  - wyłączenie bota z sesji: `Ctrl+C`
- wyłączenie bota bez wchodzenia do sesji: `screen -X -S [numer sesji, w tym przypadku 131126] quit`