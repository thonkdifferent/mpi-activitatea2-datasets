# Seturi de date și rezultate pentru activitatea 2 la Metode și Practici în Informatică

În acest repo se pot găsit datele complete de test pentru lucrarea la activitatea 2 de la `Metode și Practici în Informatică` și rezultatele complete per baterie de teste, per algoritm

### Mod de utilizare pentru reproducerea rezultatelor.

1. Se clonează / descarcă repo-ul acesta într-o locație ușor accesibilă din linia de comandă (Terminal / Command Prompt / Power Shell / ...)
2. Se clonează / descarcă [repo-ul cu algoritmi](https://github.com/EloquentDevTeam/SAT-Algorithms/) într-o locație ușor accesibilă din linia de comandă (Terminal / Command Prompt / Power Shell / ...)
3. Se execută instrucțiunile de pe repo-ul cu algoritmi
4. Se rulează scriptul python de benchmark cu ținta pe `<this_repo_path>/seturi-de-date/batch_<nr>`, unde `<nr>` poate să ia valori în intervalul **[1,4]**
5. După rulare, în interiorul folderului de teste se va genera un folder cu rezultate numit `<algoritm>_results`. Dacă toți algoritmii s-au executat cu succes (verificați linia de comandă să spună `Done` și să nu existe avertismente (warnings)) se va genera un fișier `benchmark_results.csv` și câte un fișier `.result.txt` cu rezultatele per test)


### Tipurile de date incluse
Fiecare baterie de teste conține 1000 de teste cu un anumit specific:

- Bateria 1: Literali (relativ) puțini (403), clauze (relativ) multe (10.000)
- Bateria 2: Literali (relativ) mulți (403), clauze (relativ) puține (10)
- Bateria 3: Literali și clauze echilibrate (43, 50)
- Bateria 4: Set de date cu mimim 3 clauze cu 43 literali și 50 clauze

### Interpretarea rezultatelor
În fiecare folder de rezultate ar trebui să existe 1001 fișiere (câte 1 per test, 1 fișier CSV).

În cazul în care programele sunt oprite prematur, NU se va genera un csv de test. Testele care au fost rezolvate vor avea un conținut similar cu

```
S-a citit tests/batch_1/test1.cnf
Start SAT. Resultat: UNSAT
Clauze totale: 9573
Număr maxim de clauze 9573
Timp de execuție: 135343μs
Memorie consumată: 19083264B.
Memorie consumată: 18636KB.
Memorie consumată: 18MB.
Memorie consumată: 0GB.
```

Cele care nu au fost rezolvate vor avea un conținut similar cu

```
Start SAT. Result: 
```


