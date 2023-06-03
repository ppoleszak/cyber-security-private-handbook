# Rozdział: Eliminowanie ryzyka wielodostępu (multitenancy) w chmurze obliczeniowej

## 1 Definicja Wielodostępu

Wielodostęp, znany też jako *multitenancy*, to fundamentalny aspekt architektury chmury obliczeniowej, który pozwala na dzielenie zasobów i usług pomiędzy wieloma klientami. W tym kontekście, "najemcami" są różne podmioty - firmy, organizacje, jednostki - które korzystają z tych samych zasobów fizycznych (serwerów, pamięci, magazynu danych itp.) dostarczanych przez dostawcę usług chmurowych.

## 2 Zagrożenia związane z wielodostępem

Chociaż model wielodostępu ma wiele zalet, takich jak elastyczność i redukcja kosztów, to może on również stwarzać pewne zagrożenia. Działania jednego klienta mogą wpływać na innych, zwłaszcza jeśli chodzi o wydajność i bezpieczeństwo. Na przykład, jeśli jeden klient zacznie korzystać z nadmiernie dużej ilości zasobów (tzw. "złego sąsiada"), może to wpłynąć na wydajność usług dla innych klientów.

## 3 Eliminowanie ryzyka wielodostępu

Ryzyko związane z wielodostępem można zminimalizować poprzez korzystanie z pełni dedykowanego, prywatnego środowiska chmurowego. W takim modelu, organizacja posiada swoje własne, niepodzielone zasoby w chmurze. Nie ma wtedy innych klientów, którzy mogą wpływać na te zasoby, co eliminuje ryzyko związane z wielodostępem.

## 4 Praktyczny przykład

Wyobraźmy sobie Junior Java Developera pracującego dla firmy korzystającej z usług chmurowych. Firma ta korzysta z publicznej chmury obliczeniowej, co oznacza, że dzieli zasoby (serwery, przestrzeń na dyskach itp.) z innymi firmami.

Pewnego dnia, developer zauważa, że wydajność oprogramowania, które tworzy, gwałtownie spada. Po zbadaniu sprawy okazuje się, że inna firma korzystająca z tych samych zasobów chmurowych uruchomiła bardzo zasobożerne zadania, co negatywnie wpłynęło na wydajność oprogramowania.

Aby uniknąć takich problemów w przyszłości, firma decyduje się na przejście do prywatnej chmury. Tym samym otrzymuje własne, dedykowane zasoby, które nie są dzielone z innymi firmami. Dzięki temu nie ma ryzyka, że działania innej firmy wpłyną na wydajność oprogramowania, a tym samym na pracę Junior Java Developera.