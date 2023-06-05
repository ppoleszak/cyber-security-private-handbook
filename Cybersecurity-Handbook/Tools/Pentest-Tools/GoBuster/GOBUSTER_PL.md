# Rozdział: Wyszukiwanie katalogów i plików z GoBuster

## Sekcja 1: GoBuster - Definicja i cel

GoBuster to wydajne narzędzie open-source napisane w języku Go. Jego główne zastosowanie znajduje się w cyberbezpieczeństwie, szczególnie przy brutalnym forsowaniu Uniform Resource Identifiers (URI), w tym katalogów i plików na stronach internetowych, poddomen DNS oraz nazw wirtualnych hostów na serwerach docelowych. Opracowany z myślą o testerach penetracji, GoBuster pomaga w procesie wyliczania, odkrywając "ukryte" katalogi i pliki na serwerze, które mogą nie być połączone z publicznie dostępną częścią aplikacji.

## Sekcja 2: Kiedy i dlaczego używać GoBuster

GoBuster jest zazwyczaj wykorzystywany podczas fazy rozpoznania w operacji etycznego hakowania czy testowania penetracji. Poniższe scenariusze oferują wgląd w sytuacje, kiedy korzystanie z GoBuster może być szczególnie korzystne:

1. **Odkrywanie ukrytych katalogów i plików**: GoBuster może identyfikować katalogi i pliki, które nie są połączone z główną stroną internetową lub są w inny sposób niewidoczne dla standardowych użytkowników.

2. **Wyliczanie DNS**: GoBuster może wyliczać poddomeny docelowego domeny, potencjalnie odkrywając dodatkowe wektory ataku.

3. **Odkrywanie wirtualnych hostów**: W przypadku serwerów obsługujących wiele stron internetowych, GoBuster może identyfikować te wirtualne hosty, każdy z nich potencjalnie ma unikalne podatności.

Dzięki wykorzystaniu GoBuster staje się możliwe identyfikowanie dodatkowych wektorów ataku, które mogą nie być natychmiastowo widoczne podczas regularnej interakcji z aplikacją za pomocą przeglądarki internetowej. To czyni GoBuster niezastąpionym narzędziem w arsenale każdego etycznego hakera.

## Sekcja 3: 10 Najpopularniejszych poleceń GoBuster

Uwaga: Zamień "[target]" na faktyczny cel.

1. **Bruteforcing katalogów/plików**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt
   ```
   To polecenie próbuje brutalnie forsować katalogi i pliki na stronie internetowej za pomocą predefiniowanej listy słów.

2. **Wyliczanie poddomen DNS**:
   ```
   gobuster dns -d [target] -w /usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt
   ```
   To polecenie służy do wyliczania poddomen DNS przy użyciu podanej listy słów.

3. **Wyliczanie wirtualnych hostów**:
   ```
   gobuster vhost -u http://[target] -w /usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt
   ```
   To polecenie jest użyteczne do wyliczania wirtualnych hostów przy użyciu określonej listy słów.

4. **Używanie specyficznych metod HTTP**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -m POST
   ```
   To polecenie pozwala na wykonanie żądań POST do celu podczas ataku brutalnym forsowaniem.

5. **Ustawianie nagłówków HTTP**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -H "Authorization: Bearer [Token]"
   ```
   To polecenie umożliwia dodanie konkretnego nagłówka HTTP do żądań.

6. **Dodawanie nazwy użytkownika i hasła**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -U admin -P password
   ```
   To polecenie dodaje dane uwierzytelniające Basic HTTP Authentication do żądań.

7. **Dodawanie ciasteczek**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -c "sessionid=[cookie]"
   ```
   To polecenie dodaje konkretne ciasteczko do żądań.

8. **Ustawianie User-Agent**:
   ```
   gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -a "Mozilla/5.0"
   ```
   To polecenie modyfikuje User-Agent w nagłówkach żądań HTTP.

9. **Ignorowanie certyfikatu SSL**:
   ```
   gobuster dir -k -u https://[target] -w /usr/share/wordlists/dirb/common.txt
   ```
   To polecenie mówi GoBuster, aby ignorował weryfikację certyfikatu SSL.

10. **Ustawianie limitu czasowego**:
    ```
    gobuster dir -u http://[target] -w /usr/share/wordlists/dirb/common.txt -t 100
    ```
    To polecenie ustawia limit czasowy dla żądań HTTP.

Ważne jest, aby pamiętać o odpowiedzialnym korzystaniu z narzędzi takich jak GoBuster i używaniu ich tylko wtedy, gdy masz odpowiednie uprawnienia do przeprowadzania działań związanych z testowaniem penetracji.
