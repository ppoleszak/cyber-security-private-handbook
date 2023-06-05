# Hashcat - Narzędzie do łamania haseł

## 1. Definicja i funkcjonalność Hashcat

Hashcat to narzędzie do łamania haseł, które znajduje szerokie zastosowanie w świecie bezpieczeństwa cyfrowego. Jest wykorzystywane przez testerów penetracyjnych, administratorów systemów oraz, niestety, również przez cyberprzestępców.

Hashcat służy do łamania skomplikowanych haseł, przechowywanych w formie tzw. hashy, czyli zaszyfrowanej postaci hasła. Dzięki swoim zaawansowanym algorytmom, jest w stanie "odwrócić" proces szyfrowania i odzyskać oryginalne hasło z hashu, co jest kluczowe w wielu aspektach bezpieczeństwa sieciowego.

## 2. Kiedy używać Hashcat

Hashcat może być używane w różnych sytuacjach, m.in.:

- **Sprawdzanie bezpieczeństwa haseł**: Administratorzy systemów mogą używać Hashcat do testowania siły haseł użytkowników. Jeśli Hashcat może łatwo złamać hasło, to samo może zrobić potencjalny napastnik.

- **Testy penetracyjne**: Hashcat jest często używany podczas testów penetracyjnych do łamania haseł i uzyskiwania dostępu do chronionych systemów.

Pamiętaj, że narzędzie to powinno być używane odpowiedzialnie i zawsze zgodnie z prawem.

## 3. Najczęściej używane komendy Hashcat

1. **Atak słownikowy**: `hashcat -m 0 -a 0 hash.txt wordlist.txt`
    - Ten przykład pokazuje prosty atak słownikowy.

2. **Atak kombinacyjny**: `hashcat -m 0 -a 1 hash.txt wordlist1.txt wordlist2.txt`
    - Przykład pokazuje atak kombinacyjny, który łączy słowa z dwóch różnych list słów.

3. **Atak maskowy**: `hashcat -m 0 -a 3 hash.txt ?l?l?l?l?l?l?l?l?l`
    - Ten przykład pokazuje atak maskowy, który jest bardzo skuteczny, jeśli znamy strukturę hasła.

4. **Atak oparty na regułach**: `hashcat -m 0 -a 0 -r rules/best64.rule hash.txt wordlist.txt`
    - Ten przykład pokazuje atak oparty na regułach, który jest jednym z najbardziej skomplikowanych trybów ataku.

5. **Atak siłowy**: `hashcat -m 0 -a 3 hash.txt ?a?a?a?a?a?a?a?a`
    - Ten przykład pokazuje atak siłowy, który próbuje wszystkie możliwe kombinacje.

6. **Atak na hasła WPA/WPA2**: `hashcat -m 2500 -a 0 capture.hccapx wordlist.txt`
    - Ten przykład pokazuje, jak można atakować hasła WPA/WPA2 z użyciem hashcat.

7. **Atak ze słowami składowymi**: `hashcat -m 0 -a 6 hash.txt wordlist.txt ?d?d?d?d`
    - Przykład pokazuje, jak wykonać atak ze słowami składowymi, co pozwala na szybsze odzyskiwanie haseł.

8. **Atak kombinacji**: `hashcat -m 0 -a 1 hash.txt wordlist.txt`
    - Ten przykład pokazuje, jak można połączyć różne metody ataku w celu zwiększenia skuteczności.

9. **Atak hybrydowy**: `hashcat -m 0 -a 6 hash.txt wordlist.txt ?d?d?d?d`
    - Przykład pokazuje, jak wykonać atak hybrydowy, który łączy atak słownikowy z atakiem maskowym.

10. **Odwrócenie hasha**: `hashcat -m 1000 -a 0 -o cracked.txt hash.txt wordlist.txt`
    - Ten przykład pokazuje, jak odwrócić hasha, czyli zaszyfrowane hasło, do jego oryginalnej formy.
