---
label: Plugin DynMap
icon: repo
order: 100
---

W tym poradniku dowiesz się jak skonfigurować plugin DynMap czyli najpopularniejszy plugin na mapę serwera wyświetlaną
na stronie internetowej.

## Pobieranie pluginu
Pierwszym krokiem jest pobranie pluginu np. z <a href="https://www.spigotmc.org/resources/dynmap%C2%AE.274/" rel="nofollow">spigotmc</a>.
Pobrany plik jar wrzucamy do folderu plugins naszego serwera, po czym restartujemy serwer. Ważne jest, aby w pełni zrestartować
serwer, a nie jedynie użyć komendy reload.

## Konfiguracja DynMap
Przechodzimy w panelu IVhost do swojego serwera, a następnie do zakładki ustawienia. Klikamy teraz obok portów na zębatkę,
po przeniesieniu na podstronę z portami klikamy nowy port, jako rodzaj portu wybieramy DynMap. 

Przechodzimy teraz w plikach do plugins -> dynmap -> configuration.txt. Szukamy linijki webserver-port i zmieniamy domyślny 
port (8123) na port, ktory wcześniej dodaliśmy w panelu IVhost w ustawieniach. Warto upewnić się również, że pole webserver-bindaddress 
jest zakomentowane (# z przodu) lub ustawione na 0.0.0.0, w przeciwnym razie mapa nie będzie działała. 

Zapisujemy teraz plik i restartujemy serwer, jeżeli wszystko zrobiliśmy poprawnie to powinniśmy znaleźć mapę serwera wchodząc
w przeglądarce na adres ip_serwera:port_dynmap.