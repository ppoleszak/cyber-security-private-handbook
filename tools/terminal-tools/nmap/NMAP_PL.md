# Rozdział: Skanowanie sieci z użyciem narzędzia Nmap

## 1. Definicja i funkcjonalność Nmap

Nmap, skrót od "Network Mapper", to otwarte narzędzie służące do odkrywania sieci i audytu bezpieczeństwa. Opracowany przez Gordona Lyona (znanego jako Fyodor Vaskovich), Nmap oferuje bogaty zestaw funkcji, co czyni go potężnym narzędziem dla administratorów systemów i profesjonalistów z zakresu cyberbezpieczeństwa.

Nmap wykonuje wiele zadań, w tym odkrywanie hostów, wykrywanie usług, wykrywanie wersji, identyfikację systemu operacyjnego i analizę podatności. Może skanować duże sieci lub pojedyncze hosty i dostarcza obszerne dane na temat badanych systemów. Te informacje mogą być cenne zarówno w rutynowej konserwacji sieci, jak i proaktywnych działaniach związanych z bezpieczeństwem, takich jak identyfikacja potencjalnych słabych punktów w obronie sieci.

## 2. Kiedy używać Nmap

Ze względu na swoją wszechstronność, Nmap może być przydatny w kilku scenariuszach. Oto kilka sytuacji, kiedy jego użycie jest odpowiednie:

- **Inwentaryzacja sieci i zarządzanie**: Administratorzy systemów mogą używać Nmap do sporządzania inwentaryzacji wszystkich urządzeń w ich sieci, weryfikacji topologii sieci i śledzenia czasu działania usług.
- **Audyt bezpieczeństwa**: Profesjonaliści ds. bezpieczeństwa mogą używać Nmap do identyfikacji słabych punktów, wykrywania nieautoryzowanych urządzeń w sieci lub skanowania otwartych portów, które mogłyby być wykorzystane przez złośliwych aktorów.
- **Rozwiązywanie problemów i analiza sieci**: Nmap może pomóc w diagnozowaniu problemów sieciowych, mierzeniu czasu odpowiedzi sieci i śledzeniu usług powodujących problemy.

## 3. Top 10 najczęściej używanych poleceń Nmap

1. **Skanowanie ping (Odkrywanie hostów)**: `nmap -sn <cel>`
    - To polecenie jest używane do odkrywania hostów bez skanowania portów. Często używa się go do znalezienia aktywnych hostów w sieci.

2. **Skanowanie określonego portu**: `nmap -p <port> <cel>`
    - To polecenie służy do skanowania określonego portu na hoście docelowym.

3. **Skanowanie wielu portów**: `nmap -p <port1,port2,etc> <cel>`
    - To polecenie skanuje wiele określonych portów na hoście docelowym.

4. **Skanowanie wszystkich portów**: `nmap -p- <cel>`
    - To polecenie skanuje wszystkie 65535 portów na hoście docelowym.

5. **Wykrywanie wersji**: `nmap -sV <cel>`
    - To polecenie pomaga określić wersję usług działających na otwartych portach.

6. **Wykrywanie systemu operacyjnego**: `nmap -O <cel>`
    - To polecenie próbuje określić system operacyjny hosta docelowego.

7. **Agresywne skanowanie**: `nmap -A <cel>`
    - To polecenie wykonuje agresywne skanowanie, które obejmuje wykrywanie systemu operacyjnego, wykrywanie wersji, skanowanie skryptów i traceroute.

8. **Szybkie skanowanie**: `nmap -F <cel>`
    - To polecenie wykonuje szybkie skanowanie, skanując mniej portów niż domyślne skanowanie.

9. **Skanowanie TCP SYN**: `nmap -sS <cel>`
    - To polecenie wykonuje skanowanie TCP SYN, często nazywane skanowaniem "półotwartym".

10. **Skanowanie połączenia TCP**: `nmap -sT <cel>`
    - To polecenie wykonuje pełne skanowanie połączenia TCP.

Pamiętaj, aby korzystać z Nmap odpowiedzialnie. Choć jest to potężne narzędzie do utrzymania i zabezpieczania własnych sieci, nieautoryzowane skanowanie systemów innych osób może być postrzegane jako agresywne lub złośliwe działanie. Zawsze staraj się uzyskać pozwolenie przed skanowaniem sieci, które nie są twoją własnością lub do których nie masz wyraźnego upoważnienia do skanowania.
