## Rozdział: Co to jest router?

Router, nazywany także ruterem, to urządzenie pełniące rolę "dyrygenta" w sieci komputerowej. Łączy ono ze sobą dwie lub więcej sieci typu pakietowego, czyli sieci, które przesyłają dane w pakietach, umożliwiając przesyłanie tych pakietów do ich docelowych adresów IP. W ten sposób router zarządza ruchem pomiędzy sieciami. Dodatkowo, pozwala wielu urządzeniom na korzystanie z tego samego połączenia internetowego.

Routery mogą przyjmować różne formy i służyć różnym celom, ale najczęściej spotykane są routery, które przekazują dane między sieciami lokalnymi (LAN) a sieciami rozległymi (WAN). Sieć lokalna (LAN) to grupa urządzeń połączonych w jednym, określonym geograficznie obszarze, która zazwyczaj wymaga tylko jednego routera.

Sieć rozległa (WAN) natomiast, to sieć o dużym zasięgu, rozprzestrzeniająca się na dużym obszarze geograficznym. Duże organizacje i firmy działające w wielu lokalizacjach na terenie kraju, na przykład, będą potrzebować oddzielnych sieci LAN dla każdej lokalizacji, które następnie łączą się z innymi sieciami LAN, tworząc sieć WAN. Z racji swojej dużej skali, sieć WAN często wymaga zastosowania wielu routerów i przełączników sieciowych.

Przełącznik sieciowy przesyła pakiety danych między grupami urządzeń w tej samej sieci, podczas gdy router przekazuje dane między różnymi sieciami.

### 1 Jak działa router?

Można myśleć o routerze jako o kontrolerze ruchu lotniczego, a pakietach danych jako samolotach zmierzających do różnych lotnisk (czyli sieci). Tak jak każdy samolot ma unikalne miejsce docelowe i podąża wyznaczoną trasą, każdy pakiet danych musi być skierowany do swojego miejsca docelowego jak najefektywniej. Tak samo jak kontroler ruchu lotniczego zapewnia, że samoloty docierają do swojego celu bez zbłądzenia czy napotkania poważnych zakłóceń w drodze, router pomaga kierować pakiety danych do ich docelowych adresów IP.

Aby skutecznie kierować pakiety, router korzysta z wewnętrznej tablicy routingu - listy ścieżek do różnych destynacji sieciowych. Router odczytuje nagłówek pakietu, aby dowiedzieć się, dokąd jest kierowany, następnie konsultuje tablicę routingu, aby znaleźć najbardziej efektywną drogę do tego celu. Następnie przekazuje pakiet do kolejnej sieci na trasie.

### 2 Co różni router od modemu?

Chociaż niektóre dostawcy usług internetowych (ISP) mogą łączyć router i modem w jednym urządzeniu, nie są one tym samym. Każde z nich pełni inną, ale równie ważną rolę w łączeniu sieci ze sobą i z Internetem.

Router tworzy sieci i zarządza przepływem danych w obrębie tych sieci i pomiędzy nimi, podczas gdy modem łączy te sieci z Internetem. Modemy tworzą połączenie z Internetem, przekształcając sygnały od ISP na sygnał cyfrowy, który może być odczytany przez każde podłączoną urządzenie. Pojedyncze urządzenie może być podłączone do modemu, aby połączyć się z Internetem; z drugiej strony, router może pomóc dystrybuować ten sygnał do wielu urządzeń w ramach ustanowionej sieci, umożliwiając wszystkim połączenie z Internetem jednocześnie.

Możemy to sobie wyobrazić tak: Jeśli Bob ma router, ale nie ma modemu, będzie mógł utworzyć sieć LAN i wysyłać dane między urządzeniami w tej sieci. Jednak nie będzie mógł podłączyć tej sieci do Internetu. Alice, z drugiej strony, ma modem, ale nie ma routera. Będzie mogła podłączyć pojedyncze urządzenie do Internetu (na przykład swój laptop służbowy), ale nie będzie mogła dystrybuować tego połączenia internetowego do wielu urządzeń (na przykład do swojego laptopa i smartfona). Natomiast Carol ma zarówno router, jak i modem. Korzystając z obu urządzeń, może utworzyć sieć LAN z jej komputerem stacjonarnym, tabletem i smartfonem i podłączyć je wszystkie do Internetu jednocześnie.

### 3 Typy routerów

- **Router bezprzewodowy**: Ten rodzaj routera korzysta z kabla Ethernet do połączenia z modemem. Dane dystrybuowane są poprzez konwersję pakietów z kodu binarnego na sygnały radiowe, które następnie są bezprzewodowo transmitowane za pomocą anten. Routery bezprzewodowe nie tworzą sieci LAN, ale WLAN (bezprzewodowe sieci lokalne), które łączą wiele urządzeń za pomocą komunikacji bezprzewodowej.

- **Router przewodowy**: Podobnie jak router bezprzewodowy, router przewodowy również korzysta z kabla Ethernet do połączenia z modemem. Następnie używa osobnych kabli do połączenia z jednym lub większą ilością urządzeń w sieci, tworząc sieć LAN i łącząc urządzenia w tej sieci z Internetem.

Ponadto, obok routerów bezprzewodowych i przewodowych dla małych sieci LAN, istnieje wiele specjalistycznych typów routerów służących konkretnym celom:

- **Router rdzeniowy (core router)**: W przeciwieństwie do routerów używanych w domu lub małej firmie, router rdzeniowy jest używany przez duże korporacje i firmy, które transmitują dużą ilość pakietów danych w swojej sieci. Routery rdzeniowe działają w "rdzeniu" sieci i nie komunikują się z sieciami zewnętrznymi.

- **Router brzegowy (edge router)**: Podczas gdy router rdzeniowy zarządza wyłącznie ruchem danych w sieci na dużą skalę, router brzegowy komunikuje się zarówno z routerami rdzeniowymi, jak i z sieciami zewnętrznymi. Routery brzegowe znajdują się na "krawędzi" sieci i korzystają z protokołu BGP (Border Gateway Protocol) do wysyłania i odbierania danych z innych sieci LAN i WAN.

- **Router wirtualny**: Router wirtualny to aplikacja oprogramowania, która pełni te same funkcje co standardowy router sprzętowy. Może on używać protokołu VRRP (Virtual Router Redundancy Protocol) do ustanowienia podstawowych i zapasowych routerów wirtualnych, na wypadek awarii jednego z nich.

SSID, czyli "service set identifier", to techniczne określenie nazwy sieci, którą transmitują routery WLAN. SSID umożliwia użytkownikom znalezienie i połączenie się z siecią bezprzewodową transmitowaną przez router (odpowiednio zabezpieczony router powinien wymagać wprowadzenia hasła). Routery dla sieci WiFi zazwyczaj mają swoje domyślne SSID wydrukowane na boku lub na dole urządzenia.

Z routerami związane są pewne wyzwania związane z bezpieczeństwem. Każdy sprzętowy router jest wyposażony w preinstalowane oprogramowanie zwane firmware, które pomaga routerowi w wykonywaniu jego funkcji. Jak każdy inny rodzaj oprogramowania, firmware routera często zawiera luki, które mogą być wykorzystywane przez cyberprzestępców. Dostawcy routerów regularnie wydają aktualizacje mające na celu załatanie tych luk, dlatego firmware routera powinno być regularnie aktualizowane. Nieaktualizowane routery mogą zostać skompromitowane przez napastników, co umożliwia im monitorowanie ruchu sieciowego lub wykorzystanie routera jako części botnetu.

Małe i duże organizacje często są celem ataków DDoS (distributed denial-of-service), skierowanych na ich infrastrukturę sieciową. Ataki DDoS na warstwę sieciową, które nie są skutecznie mitigowane, mogą przeciążyć routery lub spowodować ich awarię, co skutkuje przerwą w działaniu sieci. Istnieją różne rozwiązania, jak Cloudflare Magic Transit, które służą do ochrony routerów i sieci przed tego typu atakami.

Wszystkie routery są wyposażone w zestaw danych logowania administratora, które umożliwiają wykonywanie funkcji administracyjnych. Te dane są ustawione na domyślne wartości, takie jak "admin" jako nazwa użytkownika i "admin" jako hasło. Nazwa użytkownika i hasło powinny być jak najszybciej zmienione na bardziej bezpieczne, ponieważ atakujący są świadomi tych domyślnych wartości i mogą je wykorzystać do zdalnego przejęcia kontroli nad routerem, jeśli nie zostaną one zmienione.
