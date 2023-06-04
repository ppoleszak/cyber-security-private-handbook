# Rozdział: Ransomware - Wielowymiarowe Zagrożenie Cyberbezpieczeństwa

Ransomware to rodzaj złośliwego oprogramowania, znany także jako malware, który uniemożliwia dostęp do plików, systemów lub sieci komputerowych, wymagając zapłaty okupu za ich zwrot.

## 1. Podstawowe informacje o ransomware

Ransomware jest formą malware (złośliwego oprogramowania) który blokuje dane ofiary lub urządzenie i grozi, że pozostanie zablokowany - lub co gorsza - jeśli ofiara nie zapłaci okupu napastnikowi. Według raportu IBM Security X-Force Threat Intelligence Index 2023, ataki typu ransomware stanowiły 17 procent wszystkich ataków cybernetycznych w 2022 roku.

Najwcześniejsze ataki ransomware po prostu żądały okupu w zamian za klucz szyfrujący potrzebny do odzyskania dostępu do dotkniętych danych lub do użycia zainfekowanego urządzenia. Poprzez regularne tworzenie kopii zapasowych danych, organizacja mogła ograniczyć koszty wynikające z tego typu ataków ransomware i często unikać płacenia żądanej sumy okupu.

## 2 Czym jest ransomware?

Ransomware, znane również jako oprogramowanie szantażujące, to złośliwe oprogramowanie (malware), które ma na celu uniemożliwić dostęp do danych lub systemów użytkownika, a następnie żądać od niego "okupu" za ich zwrot.

### 2.1 Jak działa ransomware?

Proces infekcji ransomware jest zazwyczaj dość prosty, ale skuteczny. Oto, jak to działa:

1. Użytkownik nieświadomie pobiera i instaluje ransomware na swoim komputerze. Może to nastąpić poprzez kliknięcie na załącznik w e-mailu, odwiedzenie zainfekowanej strony internetowej, a nawet poprzez pobranie i instalację oprogramowania, które wydawało się bezpieczne.

2. Po zainstalowaniu, ransomware zaczyna szyfrować pliki użytkownika. W tym momencie, użytkownik nadal może nie wiedzieć, że jest zainfekowany.

3. Gdy proces szyfrowania jest zakończony, ransomware pokazuje komunikat, informując użytkownika o infekcji i żądając okupu (zwykle w formie kryptowaluty, takiej jak Bitcoin) za odszyfrowanie plików.

Niestety, płacenie okupu nie gwarantuje, że użytkownik odzyska dostęp do swoich danych. W niektórych przypadkach, cyberprzestępcy nie wysyłają klucza deszyfrującego nawet po otrzymaniu okupu. W innych, proces deszyfrowania może nie działać poprawnie i pliki mogą pozostać zaszyfrowane.

### 2.2 Skąd wiem, że jestem zainfekowany?

Zwykle, najłatwiej rozpoznać infekcję ransomware po komunikacie o okupie, który się wyświetla. Jednak istnieją także inne oznaki, które mogą wskazywać na infekcję ransomware:

- Nie możesz otworzyć plików, które wcześniej były dostępne.
- Pliki na twoim komputerze mają dziwne rozszerzenia, których wcześniej tam nie było.
- Twój komputer działa wolniej niż zwykle.
- Otrzymujesz komunikaty o błędach podczas próby otwarcia plików.
- Zauważasz nieznane procesy działające w Menedżerze zadań.

### 2.3 Jak mogę się chronić?

Najlepszym sposobem ochrony przed ransomware jest zapobieganie. Oto kilka wskazówek, które pomogą Ci uchronić się przed infekcją


## 3 Typy ransomware

### 3.1 Szyfrujący ransomware (crypto-ransomware)

Najczęstszy typ, nazywany ransomware szyfrującym lub krypto-ransomware, bierze dane ofiary jako zakładników, szyfrując je. Następnie napastnik żąda okupu w zamian za dostarczenie klucza deszyfrującego potrzebnego do odszyfrowania danych.

### 3.2 Ransomware blokujący (screen-locking ransomware)

Rzadsza forma ransomware, nazywana ransomware nie szyfrującym lub blokującym ekran, blokuje całe urządzenie ofiary, zazwyczaj uniemożliwiając dostęp do systemu operacyjnego. Zamiast normalnego uruchamiania, urządzenie wyświetla ekran z żądaniem okupu.

### 3.3 Podkategorie ransomware

1. **Leakware/Doxware** to ransomware, który kradnie, lub eksfiltruje, wrażliwe dane i grozi ich opublikowaniem. Podczas gdy wcześniejsze formy leakware lub doxware często kradły dane bez ich szyfrowania, dzisiejsze warianty często robią obie te rzeczy.

2. **Mobile ransomware** obejmuje wszystkie rodzaje ransomware, które wpływają na urządzenia mobilne. Dostarczany przez złośliwe aplikacje lub przez pobieranie za pośrednictwem sieci, mobile ransomware jest zazwyczaj typem ransomware nie szyfrującym, ponieważ automatyczne kopie zapasowe danych w chmurze, standardowe na wielu urządzeniach mobilnych, ułatwiają odwrócenie ataków szyfrujących.

3. **Wipers/destructive ransomware** grozi zniszczeniem danych, jeśli okup nie zostanie zapłacony - z wyjątkiem przypadków, gdy ransomware niszczy dane nawet jeśli okup jest płatny. Ten ostatni rodzaj wiperów często podejrzewa się, że jest używany przez państwa-nacje lub hakerów, a nie zwykłych cyberprzestępców.

4. **Scareware** to rodzaj ransomware, który próbuje przestraszyć użytkowników, aby zapłacili okup. Scareware może udawać wiadomość od agencji ścigania, oskarżając ofiarę o przestępstwo i żądając grzywny; może naśladować prawdziwe ostrzeżenie o infekcji wirusem, zachęcając ofiarę do zakupu oprogramowania antywirusowego lub antymalware. Czasami scareware jest ransomware, szyfrując dane lub blokując urządzenie; w innych przypadkach, jest wektorem ransomware, nie szyfruje nic, ale zmusza ofiarę do pobrania ransomware.

## 4 Ewolucja ataków ransomware

W ostatnich latach ataki ransomware ewoluowały, obejmując ataki typu podwójne i potrójne, które znacznie podnosiły stawkę - nawet dla ofiar, które utrzymują regularne kopie zapasowe danych lub płacą początkową żądanie okupu. Ataki podwójnej eksploatacji dodają groźbę kradzieży danych ofiary i wycieku ich online; na to wszystko ataki potrójnej eksploatacji grożą wykorzystaniem skradzionych danych do ataku na klientów lub partnerów biznesowych ofiary.

## 5 Koszt ataków ransomware

Ofiary i negocjatorzy ransomware niechętnie ujawniają kwoty okupu. Jednak według Definitive Guide to Ransomware, żądania okupu wzrosły do siedmio- i ośmiocyfrowych kwot. A płatności okupów stanowią tylko część całkowitego kosztu infekcji ransomware. Według raportu IBM Cost of a Data Breach 2022, średni koszt naruszenia danych spowodowanego atakiem ransomware - nie uwzględniając płatności okupu - wyniósł 4,54 miliona dolarów. Oczekuje się, że ataki ransomware będą kosztować ofiary szacunkowo 30 miliardów dolarów w 2023 roku.
