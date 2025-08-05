---
label: Jak podpiąć domenę
icon: repo
order: 99
---
## Darmowa subdomena
IVhost oferuje darmową subdomenę ivhs.pl (np. serwer.ivhs.pl). W celu ustawienia subdomeny należy udać się do ustawień
serwera i w polu Subdomena wpisać nazwę serwera. Jeżeli wpiszemy np. dirt to połączymy się z serwerem używając adresu
dirt.ivhs.pl.
## Domena z Cloudflare
Przejdź do panelu Cloudflare i wybierz swoją domenę, a następnie przejdź do zakładki DNS. Kliknij add record, w polu type
wybierz SRV, a w polu name wpisz `_minecraft._tcp`. Priority i weight ustaw na 1, w polu port wpisz główny port, który znajdziesz
w ustawieniach serwera w panelu IVhost. W target wpisz adres połączeniowy (z panelu IVhost) serwera bez portu, a następnie kliknij save.
![Podpinanie domeny na Cloudflare do serwera Minecraft](img_4.png)