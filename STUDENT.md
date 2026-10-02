# Moje wykonanie Lab00

- Login GitHub / pseudonim: Yochime
- System i terminal (np. Windows + WSL Ubuntu): MacOS + Terminal
- Edytor / IDE: Visual Studio Code
- Wersja Git: version 2.50.1 (Apple Git-155)
- Wersja kompilatora C++: Apple clang version 21.0.0 (clang-2100.1.1.101)
- Wersje java i javac: openjdk 27 2026-09-15 | javac 27
- Link do pierwszego PR (uzupełnij w zadaniu 5): https://github.com/Yochime/oop-lab00-167829/pull/1

## Uruchomienie lokalne

Wynik programu C++:

```
Hello from C++!
```

Wynik programu Java:

```
Hello from Java!
```

## Błąd i poprawka (zadanie 5)

- Krótki fragment komunikatu błędu i numer linii: cpp/main.cpp:5:59: error: expected ‘;’ before ‘return’ | 6
- Przyczyna oraz sposób naprawy: Dodanie brakującego średnika na końcu instrukcji std::cout
- Commit z błędem (SHA lub link): https://github.com/Yochime/oop-lab00-167829/actions/runs/37018453542/job/110875114976
- Czy Actions pokazały błąd, a po naprawie sukces? ...

## Krótkie odpowiedzi

1. Co różni commit od push?
   Commit zapisuje zmiany wyłącznie lokalnie na dysku Twojego komputera. Działa jak zrobienie zdjęcia (migawki) plików w danym momencie i dodanie go do lokalnej historii projektu.
   Push bierze Twoje lokalne commity i wysyła je na zewnętrzny serwer (np. GitHub). Dopiero po wykonaniu pusha Twoja praca jest zabezpieczona w chmurze i widoczna dla innych (np. dla prowadzącego).
2. Dlaczego po scaleniu PR wykonuję lokalnie pull?
   Kiedy klikasz "Merge pull request" na GitHubie, łączysz gałęzie i aktualizujesz kod na zdalnym serwerze w gałęzi main. Twoje lokalne repozytorium (na Twoim komputerze) o tym nie wie i wciąż posiada starą wersję main. Wykonanie git pull pobiera te nowości z serwera i aktualizuje pliki na Twoim dysku, aby oba miejsca (serwer i komputer) znów były idealnie zsynchronizowane.
3. Co potwierdza zielony wynik naszego CI, a czego nie potwierdza?
   Potwierdza: że kod nie ma błędów składniowych (kompiluje się) oraz że daje się uruchomić bez awarii w czystym, wyizolowanym środowisku na serwerach GitHuba.
   Nie potwierdza: poprawności logicznej działania programu (np. czy program wypisuje dokładnie ten tekst, o który prosił prowadzący w zadaniu) ani tego, czy środowisko programistyczne na Twoim własnym komputerze jest poprawnie skonfigurowane (ponieważ testy uruchamiają się na maszynie w chmurze, a nie u Ciebie).

## Ewentualne problemy środowiska

Brak / opis problemu i sposób rozwiązania: ...
