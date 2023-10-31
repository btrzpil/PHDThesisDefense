# Zapis dyskusji w trakcie obrony doktorskiej mgr. inż. Beaty Trzpil-Jurgielewicz pt. "Opracowanie wielokanałowego układu scalonego w technologii CMOS do rejestracji aktywności neuronalnej oraz jego aplikacja w funkcjonalnych badaniach mózgu" z dnia 30.10.2023 r., która odbyła się sali seminaryjnej ACMiN, przy ul. Kawiory 50 w Krakowie

## Odpowiedzi na uwagi recenzentów

pf i kom

*Autorka nie sformułowała tezy rozprawy, co wynika ze specyfiki pracy, natomiast celem praktycznym było opracowanie takiego rozwiązania konstrukcyjnego przedwzmacniacza, aby umożliwić skuteczną realizację zintegrowanego narzędzia do badań mózgu przez zespół Katedry Oddziaływań i Detekcji Cząstek AGH.*

*W przypadku przedstawionej pracy Autorka precyzyjnie przedstawiła główny cel pracy oraz wyszczególniła kolejny etapy pracy prowadzące do realizacji celu głównego.
Niestety w pracy nie zauważyłem wyszczególnionych tez pracy.  Jakie są zatem cele pracy? Czy tezy pracy zostały udowodnione?*

btj

Wydaje mi się, że zostało to wyjaśnione w międzyczasie, że tezy pracy są tożsame z celem i nie zostały explicite odrębnie sformułowane.
Teraz z perspektywy, widzę, że byłoby to przydatne podczas czytania.

---

kom

*Struktura rozprawy jest logiczna, jednak w pracy występuje pewna (moim zdaniem stanowczo zbyt liczna) liczba uchybień edycyjnych (tekstowych, językowych), np. forma gramatyczna, powtórzenia, brak przedimków lub słów itp.*

btj

Przepraszam za wszystkie uchybienia edycyjne, gramatyczne, które pojawiły się w tekście.

pf

To było do przeżycia.

kom

Powiem, że zdarzało mi się czytać gorzej zredagowane teksty.

---

pf

*W tekście pracy jest relatywnie dużo literówek, występują też drobne błędy gramatyczne, co świadczy prawdopodobnie o nadmiernie pospiesznym finalizowaniu rozprawy. 
Innych niedociągnięć jest niewiele, np.: na rysunkach 3.13 i 3.14 na osi odciętych skala częstotliwości obejmuje zakres od 0.1 Hz do 100 Hz, podczas gdy w podpisie podano pasmo 1 Hz -- 10 kHz. 
Ponadto tabela 4.3 jest wadliwie zbudowana i bez dodatkowego opisu nieczytelna.*
            
btj

Można było lepiej skonstruować ten wykres, ponieważ legenda powinna być zatytułowana "ekwiwalentne szumy wejściowe", które zostały policzone w zakresie 1 Hz -- 10 kHz.
Jednak na wykresie przedstawiłam węższy zakres, ponieważ najważniejsze rzeczy dzieją się w tym paśmie.
Gdyby wykres zawierał dodatkowe trzy dekady, wykres byłby mniej czytelny.

W przypadku wspomnianej tabeli dla danego prądu polaryzującego wzmacniacz oraz częstotliwości granicznej pokazywałam ekwiwalentne szumy wejściowe z zakresu sygnału LFP oraz AP.
Faktycznie w tej tabeli brakowało nagłówka, teraz powinno być bardziej zrozumiałe.

pf

Ja się domyśliłem. To są drobiazgi.

---

pf

*Zwykle jednak wymagania projektowe formułowane są explicite w formie granicznych wartości istotnych parametrów, lecz takich na dla pracy nie określono. 
W tej sytuacji pierwszorzędnego znaczenia nabiera porównanie wartości osiągniętych parametrów zaprojektowanego wzmacniacza z danymi dostępnymi z literatury. 
Brak zestawienia porównawczego w formie tabeli budzi pewien niedosyt. 
Wprawdzie standardowo w odniesieniu do zniekształceń harmonicznych wartość THD podawana jest zwykle dla częstotliwości 1 kHz, a nie w szerszym zakresie, to jednak takie zestawienie byłoby zasadne, uwzględniając zarówno ogólne stwierdzenia, jak i wartości innych parametrów.*

btj

Powodem, dla którego nie podano sztywnych wartości, wynika z tego, że celem projektu było zbadanie możliwości zbudowania takiego wzmacniacza w wybranej technologii i nie celowano w konkretny zestaw parametrów.
Powierzchnia, moc, szumy są parametrami, które się wymieniają -- optymalizując jeden z nich, można pogorszyć pozostałe.
W trakcie opracowywania projektu oczywiście miałam w głowie te własności w kontekście późniejszego zbudowania wielokanałowego układu odczytowego.
Podanie uzyskanych wartości jako celów do osiągnięcia wyglądało nienaturalnie.

Natomiast, nawiązując do tabeli zbiorczej, powód był taki, że nie chciałam porównywać zniekształceń, ponieważ w literaturze typowo nie są podawane. 
 
----

kom

*Omówiono również inne koncepcje eliminacji składowej stałej: technikę wzmacniaczy z modulacją [...] oraz zastosowanie wzmacniacza o małym lub jednostkowym wzmocnieniu i przetwornika analogowo-cyfrowego o dużej rozdzielczości.
Z uwagi na rosnącą popularność tego ostatniego rozwiązania w przypadku akwizycji sygnałów biologicznych i biomedycznych uważam, że ta część rozdziału powinna być bardziej szczegółowa.*

btj

Ten temat mógł zostać poszerzony, ale te rozwiązania bardzo często tyczą się zastosowań w EEG -- ze względu na rejestrowane sygnały wymagania są trochę inne dotyczące ilości kanałów pomiarowych, rozmiarów oraz technologii.
W związku z tym zdecydowałam się nie poszerzać tego rozdziału o te zastosowania.

kom

Ja tutaj dalej mam pewne wątpliwości, które myślę dotyczyłyby samej metody, bo gdy pojawiły się tak dokładne rozwiązania (układy scalone, które to implementują).
Cały czas się zastanawiam, czy taka technologia na zasadzie budowy elektrod aktywnych, czyli małych prosty wzmacniacz, potem jakiś tor pomiarowy odporny na szum i później przetwarzanie za pomocą przetworników o dużej rozdzielczości, które umożliwiają przetwarzanie sygnału na poziomie cyfrowym, dając dużo większe możliwości.
Wtedy pozbywamy się tych zniekształceń, które te układy wprowadzają, ale to mój komentarz być może to będzie przyszłość.

btj

Te rozwiązania charakteryzują się większymi powierzchniami. 
Jeżeli celem jest stworzenie układu wielokanałowego (nawet 5000 kanałów odczytowych) to proponowane rozwiązanie jest bardziej korzystne.

kom

Zgadzam się z tym, ale w pracy można było napisać dwa zdania, dlaczego tego właśnie nie omawiam.

---

kom

*W pracy występuje dość obszerna część medyczno-biologiczna służąca w zasadzie do uzasadnienia podziału sygnałów na dwie grupy LFP i AP o odpowiednich charakterystykach (pasmo i zakres amplitud).
Materiał ciekawy i ważny z punktu widzenia pracy, ale być może mógłby być krótszy.*

btj

Przjymuję to, jednak drugi recenzent stwierdził, że materiał ten mógł zostać poszerzony.
Ze względu na interdyscyplinarny charakter pracy trudno...

kom

Ze względu na to, że pracujemy w różnych dyscyplinach, każdy z nas zwraca uwagę na inne fragmenty

buch

Chciałem zwrócić uwagę, Panie Profesorze, że zostaliśmy politycznie rozegrani.

btj

Zaczęłam pisać pracę od tego rozdziału. 
Jak zaczyna się pisać, to pisze się bardzo dużo, a potem im bliżej finalizacji to trzeba dojść do tych wyników, które są kluczowe w danej pracy.

pf

Ja chętnie przeczytałem.

---

kom

*Niektóre używane w pracy określenia moim zdaniem są nietypowe, głównie dotyczy to określenia "układ odczytu" zamiast wzmacniacz.
[...]
Podobnie użycie słowa "zaadresowany".
Wyrażenie "mniejsze multipleksery" (str. 34) jest mało precyzyjne, a właściwie w użytym kontekście nieprawidłowe.
Również definicja wyrażenia "front-end" (str. 35) budzi moje wątpliwości.
Użycie wyrażenia "może zostać drastycznie zmniejszona" wydaje mi się również niezbyt fortunne.
Autorka rozprawy dosyć często używa wyrażenia offset wyjściowy, moim zdaniem jednak poprawnie powinno się stosować wyrażenie offset napięcia wyjściowego.*

## Publiczna dyskusja: