# Rozdział: Model współdzielonej odpowiedzialności w chmurze

W świecie chmurowych usług informatycznych, kluczowym konceptem jest model współdzielonej odpowiedzialności. W zależności od wybranego modelu usługi, różne aspekty zarządzania i bezpieczeństwa systemu są dzielone między dostawcę usług chmurowych (CSP) i klienta.

## 1. Infrastructure as a Service (IaaS)

Przykładem usługi IaaS jest Amazon Web Services (AWS) - Elastic Compute Cloud (EC2). Kiedy korzystasz z EC2, Amazon dostarcza Ci podstawową infrastrukturę - serwery, pamięć, sieć - i jest odpowiedzialny za jej utrzymanie i bezpieczeństwo. Jako deweloper, masz możliwość wdrażania swojego oprogramowania na tych serwerach, ale jesteś odpowiedzialny za jego bezpieczeństwo i prawidłowe działanie.

W takim modelu, AWS odpowiada za "bezpieczeństwo chmury" - czyli fizyczną infrastrukturę, serwery, oprogramowanie, które je obsługuje, sieć, itd. Z drugiej strony, klient jest odpowiedzialny za "bezpieczeństwo w chmurze" - to znaczy za oprogramowanie, które uruchamia na tych serwerach, za dane, które przechowuje, za to, jak te dane są zabezpieczone, itp.

## 2. Software as a Service (SaaS)

Przykłady usług SaaS to Gmail od Google lub Office 365 od Microsoft. W modelu SaaS, dostawca usług chmurowych jest odpowiedzialny nie tylko za infrastrukturę, ale również za oprogramowanie i jego działanie. To oznacza, że dostawca musi zapewnić nie tylko "bezpieczeństwo chmury", ale również "bezpieczeństwo w chmurze".

Jako użytkownik usługi SaaS, jesteś odpowiedzialny głównie za bezpieczeństwo na poziomie użytkownika. Obejmuje to takie aspekty jak zarządzanie tożsamością i dostępem, zabezpieczanie danych użytkownika, zarządzanie hasłami, korzystanie z zabezpieczeń dwuetapowych itp.

## 3. Porównanie IaaS i SaaS

Z perspektywy bezpieczeństwa, najważniejsza różnica między IaaS i SaaS polega na tym, gdzie kończy się odpowiedzialność dostawcy usług chmurowych, a zaczyna odpowiedzialność klienta.

W przypadku IaaS, jak AWS EC2, odpowiedzialność dostawcy kończy się na infrastrukturze. Klient musi sam zapewnić bezpieczeństwo swojego oprogramowania i danych.

Natomiast w przypadku SaaS, jak Gmail lub Office 365, dostawca usług chmurowych jest odpowiedzialny za całość - zarówno infrastrukturę, jak i oprogramowanie. Jako użytkownik, musisz jedynie zadbać o bezpieczeństwo na poziomie użytkownika.

To porównanie pokazuje, dlaczego model SaaS nakłada największą odpowiedzialność na dostawcę usług chmurowych. Nie tylko muszą oni zapewnić bezpieczną i niezawodną infrastrukturę, ale również muszą zapewnić, że oprogramowanie, które dostarczają jako usługę, jest bezpieczne i działa prawidłowo.