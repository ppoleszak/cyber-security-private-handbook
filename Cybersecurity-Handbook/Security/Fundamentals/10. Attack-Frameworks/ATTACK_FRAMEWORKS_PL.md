# Rozdział: Frameworki Ataku w Cyberbezpieczeństwie

## 1 Kill Chain

Kill Chain to framework opracowany przez Lockheed Martin, który opisuje etapy, poprzez które napastnik (ang. threat actor) postępuje podczas inwazji sieciowej. Framework ten składa się z następujących etapów:

### 1.1 Rozpoznanie (Reconnaissance)

Na tym etapie, napastnik określa, które metody wykorzysta do wykonania ataku. Rozpoznanie polega na gromadzeniu informacji o celu, które mogą obejmować działania takie jak skanowanie portów, identyfikacja systemu operacyjnego, określanie wersji oprogramowania i identyfikacja potencjalnych słabych punktów. Narzędzia często wykorzystywane do tego etapu to np. Nmap, Nessus, czy Wireshark.

### 1.2 Uzbrojenie (Weaponization)

Tutaj, napastnik łączy kod ładunku, który umożliwi dostęp, z kodem exploit, który wykorzysta podatność do wykonania na systemie docelowym. Proces ten może obejmować tworzenie lub modyfikowanie malware, ukrywanie malware przed systemami wykrywania lub utworzenie phishingowego emaila lub strony internetowej. Narzędzia takie jak Metasploit, Veil-Evasion czy SET (Social-Engineer Toolkit) mogą być tutaj wykorzystane.

### 1.3 Dostarczenie (Delivery)

W tym etapie, napastnik identyfikuje wektor, poprzez który przekaże uzbrojony kod do środowiska docelowego. Wektory dostarczenia mogą obejmować e-maile, strony internetowe, nośniki USB, sieciowe skanowanie portów lub ataki typu man-in-the-middle. Przykładowo, narzędzia do spear phishingu, takie jak GoPhish, mogą być używane do dostarczania ładunków.

### 1.4 Wykorzystanie (Exploitation)

Tutaj, uzbrojony kod jest wykonywany na systemie docelowym. Może to obejmować wykorzystanie podatności, zmuszenie użytkownika do wykonania czynności (na przykład kliknięcie na link w e-mailu phishingowym) lub inny mechanizm, który umożliwi kodowi dostęp do systemu. Znane narzędzia takie jak Metasploit, Exploit DB mogą być użyte do wykorzystania podatności.

### 1.5 Instalacja (Installation)

Ten mechanizm umożliwia uzbrojonemu kodowi uruchomienie narzędzia do zdalnego dostępu i osiągnięcie trwałości na systemie docelowym. Może to obejmować działania takie jak zmiana ustawień systemowych, dodawanie wpisów do rejestru lub tworzenie nowych usług, które uruchamiają się przy starcie systemu. Narzędzia RAT (Remote Access Trojan) takie jak njRAT, DarkComet, albo Mimikatz służą do utrzymania dostępu.

### 1.6 Command & Control (C2)

W tym etapie, uzbrojony kod ustanawia kanał wyjściowy do zdalnego serwera, który może następnie być wykorzystany do kontrolowania narzędzia do zdalnego dostępu i ewentualnie pobierania dodatkowych narzędzi do przeprowadzenia ataku. Serwery C2 mogą być bezpośrednio kontrolowane przez napastnika, lub mogą być częścią sieci botnet. Narzędzia takie jak Empire, Cobalt Strike, czy Powershell są często wykorzystywane na tym etapie.

### 1.7 Działania na celach (Actions on Objectives)

Na tym etapie, napastnik zazwyczaj wykorzystuje uzyskany dostęp do cichego gromadzenia informacji z systemów docelowych i przekazuje je do zdalnego systemu (egzfiltracja danych) lub realizuje inne cele i motywy. To może obejmować kradzież danych, sabotowanie operacji, szpiegostwo, tworzenie backdoors, lub dowolne inne działania, które napastnik może chcieć podjąć.

Analiza Kill Chain może być używana do identyfikacji defensywnej macierzy działań w celu przeciwdziałania postępom ataku na każdym etapie.

## 2 MITRE ATT&CK Framework

MITRE ATT&CK (Adversarial Tactics, Techniques & Common Knowledge) to baza wiedzy utrzymana przez MITRE Corporation, zawierająca listę i wyjaśnienia specyficznych taktyk, technik i procedur stosowanych przez przeciwników. Ten framework jest dostępny na stronie [attack.mitre.org](https://attack.mitre.org).

MITRE ATT&CK obejmuje szeroki zakres taktyk i technik stosowanych przez przeciwników na różnych etapach ataku. Dla każdej taktyki, techniki są opisane szczegółowo, z informacjami na temat tego, jak są używane, jak mogą być wykrywane i jak można im przeciwdziałać. Framework pre-ATT&CK odnosi się do taktyk związanych z etapami rozpoznania i uzbrojenia Kill Chain.

## 3 Diamond Model of Intrusion Analysis

Diamond Model to framework do analizy incydentów związanych z cyberbezpieczeństwem i wtargnięciami, badający relacje pomiędzy czterema kluczowymi aspektami: przeciwnikiem (adversary), zdolnością (capability), infrastrukturą (infrastructure) i ofiarą (victim).

Przeciwnik to podmiot, który przeprowadza atak. Może to być pojedynczy haker, grupa hakerów, organizacja przestępcza, czy nawet państwo. Zdolność to zestaw umiejętności, wiedzy, narzędzi i innych zasobów, które przeciwnik ma do swojej dyspozycji. Infrastruktura to środki, które przeciwnik wykorzystuje do przeprowadzenia ataku, takie jak serwery, sieci botnet, czy strony phishingowe. Ofiara to podmiot, który jest celem ataku.

Analiza zgodna z modelem Diamond pozwala na lepsze zrozumienie i charakterystykę incydentu poprzez zrozumienie, jak te cztery aspekty są ze sobą powiązane i jak każdy z nich wpływa na przebieg incydentu.