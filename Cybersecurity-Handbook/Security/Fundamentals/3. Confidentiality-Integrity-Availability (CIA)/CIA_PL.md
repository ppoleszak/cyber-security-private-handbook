# Rozdział: Poufność, Integralność, Dostępność (CIA)

## Wstęp

Model CIA to podstawowe zasady bezpieczeństwa informacji, stanowiące wytyczne do oceny, a także tworzenia polityk, procedur i mechanizmów kontrolnych zorientowanych na ochronę informacji.

## Poufność

Poufność odnosi się do upewnienia się, że dostęp do informacji mają jedynie osoby uprawnione. Technologia szyfrowania to podstawowe narzędzie zabezpieczające poufność, ale równie istotne jest zarządzanie prawami dostępu oraz uwierzytelnianie użytkowników. Naruszenie poufności może prowadzić do nieautoryzowanego ujawnienia danych, co może mieć poważne konsekwencje, takie jak naruszenie prywatności, utrata własności intelektualnej czy niewłaściwe użycie informacji.

Poufność zawiera dwa kluczowe elementy:

* Autentykacja, która obejmuje procesy umożliwiające systemom weryfikację tożsamości użytkowników. Zaliczają się do nich hasła, techniki biometryczne, tokeny bezpieczeństwa, klucze kryptograficzne itd.
* Autoryzacja, która definiuje, kto i do jakich informacji ma dostęp. Ważne jest, aby zrozumieć, że identyfikacja użytkownika nie oznacza automatycznego dostępu do wszystkich danych. Mechanizmy autoryzacji to jeden z głównych sposobów zabezpieczania poufności.

## Integralność

Integralność gwarantuje, że informacje nie zostaną zmienione lub usunięte w sposób nieupoważniony. Kontrola integralności może obejmować takie mechanizmy jak kontrola wersji, sumy kontrolne, funkcje skrótu kryptograficznego i cyfrowe podpisy. Naruszenie integralności może prowadzić do wprowadzenia fałszywych informacji, które mogą wpływać na decyzje biznesowe, bezpieczeństwo czy zgodność z prawem.

## Dostępność

Dostępność gwarantuje, że informacje i zasoby są dostępne dla uprawnionych użytkowników wtedy, kiedy są potrzebne. Kontrola dostępności może obejmować redundancję, odporność na awarie, równoważenie obciążenia, backupy i plany odzyskiwania po awarii. Naruszenie dostępności może prowadzić do przestojów, które mogą wpływać na funkcjonowanie organizacji.

## Model CIA w praktyce

Model CIA powinien być wytyczną dla Twojej organizacji podczas tworzenia i implementacji ogólnych polityk i strategii bezpieczeństwa. Implementacja modelu CIA to nie tylko zakup konkretnych narzędzi, ale przede wszystkim sposób myślenia, planowania i ustalania priorytetów.

## Rozszerzenia modelu CIA

Chociaż model CIA jest fundamentalny, istnieją dodatkowe zasady i modele, które poszerzają ten podstawowy trybunał. Na przykład, w 1998 roku Donn Parker zaproponował sześciostronny model, zwany Parkerian Hexad, obejmujący zasady:

* Poufność
* Posiadanie lub kontrola
* Integralność
* Autentyczność
* Dostępność
* Przydatność

Warto zaznaczyć, że dodatkowe trzy punkty tego modelu są kontrowersyjne i mogą być grupowane pod dostępnością.

Jeszcze jedną zasada bezpieczeństwa, nieobjętą przez model CIA, jest niezaprzeczalność. Jest to gwarancja, że dana osoba nie może fałszywie zaprzeczyć, że stworzyła, zmieniła, zaobserwowała czy przesłała określoną informację.