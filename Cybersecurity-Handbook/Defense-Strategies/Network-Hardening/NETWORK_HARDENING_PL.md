# Rozdział 5: Utwierdzanie sieci (Network Hardening)

Utwierdzanie sieci, znane również jako "Network Hardening", to proces polegający na zwiększeniu bezpieczeństwa sieci poprzez wykrywanie i eliminację różnych luk bezpieczeństwa, które mogą zostać wykorzystane do zagrożenia integralności, dostępności czy poufności sieci. Proces ten obejmuje szereg strategii, technik i najlepszych praktyk, których celem jest zminimalizowanie podatności sieci na ataki, zarówno zewnętrzne, jak i wewnętrzne.

## 1. Proces utwardzania sieci

Proces utwardzania sieci zazwyczaj obejmuje następujące etapy:

1. **Ocena i analiza**: Pierwszym krokiem jest przeprowadzenie szczegółowej oceny bezpieczeństwa sieci, która obejmuje identyfikację wszystkich urządzeń, oprogramowania i protokołów, które są w niej wykorzystywane. Następnie analizowane są potencjalne słabości, które mogą być wykorzystane przez potencjalnych atakujących.
2. **Implementacja środków ochrony**: Po zidentyfikowaniu potencjalnych luk, kolejnym krokiem jest wdrożenie różnych środków ochrony. Mogą one obejmować aktualizację oprogramowania i systemów operacyjnych do najnowszych wersji, stosowanie silnych haseł, konfigurację zapór sieciowych oraz ograniczanie dostępu do określonych zasobów sieciowych tylko dla niezbędnych użytkowników.
3. **Monitorowanie i testowanie**: Po wdrożeniu środków ochrony, ważne jest ich regularne monitorowanie i testowanie, aby upewnić się, że są skuteczne. Może to obejmować regularne skanowanie sieci w poszukiwaniu potencjalnych luk, monitorowanie ruchu sieciowego w celu wykrycia nietypowej aktywności oraz przeprowadzanie testów penetracyjnych.

## 2. Utwierdzanie sieci a cyberbezpieczeństwo

W kontekście cyberbezpieczeństwa, utwardzanie sieci jest kluczowe dla zapewnienia ochrony przed różnymi zagrożeniami, takimi jak ataki typu DoS (Denial-of-Service), ataki typu "man-in-the-middle", oraz próby włamania. Bez odpowiedniego utwardzenia, sieć może stać się łatwym celem dla atakujących.

## 3. Jak utwardzić system?

Proces utwardzenia systemu polega na redukcji tzw. "powierzchni ataku", czyli zbioru wszystkich potencjalnych słabości i luk, które mogą być wykorzystane przez cyberprzestępców. Te podatności mogą wystąpić na wiele sposobów:

- **Domyślne hasła**: Cyberprzestępcy mogą wykorzystać programy do automatycznego łamania haseł, aby odgadnąć ustawienia domyślne. Ta luka może być szczególnie duże, jeżeli te same domyślne hasła są używane na wielu różnych urządzeniach czy kontach użytkowników.
- **Zaszyte w kodzie hasła i inne dane uwierzytelniające**: Jeżeli takie dane zostaną przypadkowo opublikowane lub zapomniane w kodzie, mogą one dostarczyć atakującym "tylne drzwi" do systemu.
- **Niezałatane luki w oprogramowaniu**: Niezałatane luki w oprogramowaniu i systemach są jednym z największych źródeł podatności na ataki. Chociaż łatanie takich luk zwykle niweluje problem, łatki nie zawsze są dostępne, a ich instalacja może być czasami skomplikowana lub kosztowna.
- **Brak kontroli dostępu dla kont o wysokich uprawnieniach**: Konta o wysokich uprawnieniach, takie jak konta administratorów, stanowią ogromne ryzyko, jeśli nie są odpowiednio chronione. Atakujący, którzy zdobędą dostęp do takiego konta, mogą mieć pełną kontrolę nad systemem.
- **Błędna konfiguracja sprzętu i oprogramowania**: Błędna konfiguracja systemów może prowadzić do poważnych luk bezpieczeństwa. Niewłaściwie skonfigurowane serwery, zapory sieciowe, routery czy porty mogą stanowić łatwe cele dla atakujących.
- **Niezabezpieczony ruch sieciowy**: Niezaszyfrowany ruch sieciowy lub dane przechowywane bez odpowiedniej ochrony mogą stanowić łatwy cel dla atakujących, którzy mogą podsłuchiwać komunikację i zdobyć cenne informacje, takie jak hasła czy dane osobowe użytkowników.

Dodatkowo, Centrum Bezpieczeństwa Internetu (Center for Internet Security, CIS) dostarcza aktualne wytyczne dotyczące najlepszych praktyk konfiguracji systemów dla konkretnych przypadków użycia. Standardy CIS obejmują ponad 100 wytycznych dla 25 rodzin produktów dostawców (Amazon Linux, Amazon AWS, Apple iOS, Apple macOS, Checkpoint Firewall, Cisco, Docker, Google Cloud, Microsoft Azure, itp.).