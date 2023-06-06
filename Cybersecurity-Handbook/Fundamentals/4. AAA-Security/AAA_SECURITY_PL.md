# Rozdział: Trójka A (AAA) Bezpieczeństwa

Trójka A, znana również jako AAA, odnosi się do trzech kluczowych elementów bezpieczeństwa: uwierzytelniania (Authentication), autoryzacji (Authorization) oraz kontroli dostępu (Accounting/Auditing). AAA jest ramą bezpieczeństwa kontrolującą dostęp do zasobów komputerowych, egzekwującą polityki i audytującą użycie.

## 1 Uwierzytelnianie (Authentication)

Uwierzytelnianie polega na dostarczeniu przez użytkownika informacji o swojej tożsamości. Użytkownicy przedstawiają dane logowania potwierdzające, że są tym, za kogo się podają. AAA porównuje dane uwierzytelniające użytkownika z bazą przechowywanych danych, sprawdzając czy nazwa użytkownika, hasło i inne narzędzia uwierzytelniające zgadzają się z danym użytkownikiem.

Trzy typy uwierzytelniania obejmują coś, co wiesz (np. hasło), coś, co masz (np. klucz USB) i coś, kim jesteś (np. odcisk palca lub inne biometryki).

## 2 Autoryzacja (Authorization)

Autoryzacja następuje po uwierzytelnianiu. W trakcie autoryzacji użytkownikowi można przyznać uprawnienia do dostępu do określonych obszarów sieci lub systemu. Autoryzacja różni się od uwierzytelniania tym, że uwierzytelnianie sprawdza jedynie tożsamość użytkownika, natomiast autoryzacja określa, co użytkownik może robić.

Na przykład członek zespołu IT może nie mieć potrzebnych uprawnień do zmiany haseł dostępu do sieci VPN całego przedsiębiorstwa. Jednak administrator sieci może zdecydować się nadać członkowi uprawnienia dostępu, umożliwiając mu zmianę haseł VPN poszczególnych użytkowników.

## 3 Kontrola Dostępu (Accounting/Auditing)

Kontrola dostępu śledzi aktywność użytkownika podczas logowania do sieci. Może być używana do analizy trendów, audytu aktywności użytkownika i precyzyjniejszego fakturowania.

## 4 Dlaczego AAA jest ważne w bezpieczeństwie sieciowym?

AAA jest kluczowym elementem bezpieczeństwa sieciowego, ponieważ ogranicza, kto ma dostęp do systemu i śledzi ich aktywność. Istnieją dwa główne typy AAA dla sieci: dostęp do sieci i administracja urządzeń.

### 4.1 Dostęp do sieci (Network Access)

Dostęp do sieci polega na blokowaniu, przyznawaniu lub ograniczaniu dostępu na podstawie poświadczeń użytkownika. AAA weryfikuje tożsamość urządzenia lub użytkownika, porównując podane informacje z bazą zatwierdzonych poświadczeń. Jeżeli informacje pasują, dostęp do sieci jest przyznawany.

### 4.2 Administracja urządzeniem (Device Administration)

Administracja urządzeniem obejmuje kontrolę dostępu do sesji, konsol urządzeń sieciowych, secure shell (SSH) i więcej. Ten rodzaj dostępu różni się od dostępu do sieci, ponieważ nie ogranicza, kto ma prawo wejść do sieci, ale raczej do jakich urządzeń mogą mieć dostęp.