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

btj

Tor odczytu obejmuje wzmacniacz, przetworniki, multipleksery i jest pojęciem szerszym, aniżeli wzmacniacz, dlatego używałam pojęcia "tor odczytu" w kontekście całego toru, a wzmacniacz jako ten fragment, który za pierwszy stopień wejściowy.

Kolejno "front-end", to pewnie wynika z tego, że w kontekście struktur scalonych jest to powszechnie używane pojęcie, które opisuje ten tor odczytu, wstępne przetwarzanie.

kom

Pozwolę sobie na drobny komentarz. 
Zastanawiałem się nad definicją "front-endu".
Kiedyś spotkałem się pierwszy raz w swojej historii, było to kilkanaście lat temu -- jak to tłumaczyć na polski? Dlaczego "front"? Dlaczego "end"?
Kiedyś znalazłem publikację "front", czyli analogówka, zakończona przetwornikiem cyfrowym "end".

pf

Ja nie cierpię określenia "front-end" i "back-end", ponieważ w różnych środowiskach jest to troszeczkę inaczej używane.
Więc ja się zgadzam z Panem Profesorem, że lepiej tego nie używać.
Natomiast nie odniosłem wrażenia, że jest użyte błędnie, bo ja się już z tym spotykałem w środowisku elektroników, niektórzy lubią.

dąbr

W ramach komentarza to jest coś, co mnie od długiego czasu też gnębiło, co zrobić w języku polskim z tym.
Nasza działalność, oprócz tej działalności, to jest również detekcja promieniowania i tam ten "front-end" jest tak powszechnie używany.
Ja się powołuję na naszego profesora seniora Korbla, który był purystą językowym.
W pewnym momencie wydał książeczkę z tytułem "front-end".
Od tego czasu uznałem, że to zostało w języku polskim usankcjonowane, aczkolwiek w odniesieniu do elektroniki związanej z detekcją promieniowania.

btj

Kontynuując, w kontekście sformułowania "może zostać drastycznie zmniejszona" w pracy chodziło mi o multipleksery obejmujące mniejszą liczbę kanałów wejściowych.
Jeżeli mamy mniejszą liczbę kanałów, można wykorzystywać mniejsze częstotliwości zegarów odpowiedzialnych za próbkowanie sygnałów.

---

kom

*Wzmacniacz LNA występuje w każdym kanale, skąd następnie sygnał jest przesyłany poprzez MUX z podziałem czasu.
Wadą tego rozwiązania jest to, że gdy liczba kanałów wzrasta, częstotliwość próbkowania ADC również wzrasta, co powoduje większy pobór mocy. - Częstotliwość próbkowania powinna być zależna od właściwości próbkowanego (rejestrowanego) sygnału, a nie zależeć od architektury systemu.*

btj

Oczywiście częstotliwość próbkowania jest zdeterminowana charakterystyką sygnału zgodnie z twierdzeniem Nyquista.
W powyższym stwierdzeniu nieumiejętnie próbowano przekazać, że częstotliwość ADC zależy od architektury, a konkretnie od ilości obsługiwanych kanałów w przetworniku.
Jeżeli użyjemy ADC obsługujące jeden kanał jego częstotliwość próbkowania jest tożsama z częstotliwością próbkowana sygnału, ale w przypadku multipleksowania wielu kanałów do jednego ADC jego częstotliwość systemu musi być odpowiednio większa.

kom

Ja mam na myśli, że ma Pani tu na myśli częstotliwość taktowania.
Częstotliwość próbkowania oraz częstotliwość taktowania to są dwie różne rzeczy.
Zgodzę się, że w tego typu układach pobór mocy jest większy i zależy od częstotliwości taktowania.

---

kom 

*Impedancja mikroelektrody jest ważnym parametrem dla rejestracji zewnątrzkomórkowej, ponieważ określa szumy elektrody oraz tłumienie sygnału. -- w jaki sposób impedancja określa te parametry?*

btj

Tutaj przywołuję wykres zależności impedancji od...

kom

Ja Pani przerwę, gdyby Pani napisała "wpływa" to by było poprawnie.
Impedancja nie "określa" szumów.
Można przejść dalej

---

kom

*Niektóre fragmenty tekstu są dla mnie niezrozumiałe lub budzą pewne wątpliwości
Z punktu widzenia minimalizacji poboru mocy najkorzystniejsza jest polaryzacja tranzystorów w zakresie słabej inwersji, ponieważ w tym zakresie transkonduktancji do prądu polaryzacji tranzystora jest największy [48].*

btj

Szumy termiczne są odwrotnie proporcjonalne do wartości transkonduktancji, więc zależy nam na tym, żeby ta wartość transkonduktancji była jak największa.
Na nią wpływa prądu drenu, zależnie od zakresu pracy tranzystora.
W obszarze podprogowym zależność ta jest liniowa, natomiast w silnej inwersji pierwiastkowa.

---

kom 

*Niektóre fragmenty tekstu są dla mnie niezrozumiałe lub budzą pewne wątpliwości
[...] ale przy stałym stosunku $C_{in}/C_{f} = 20 V/V$*

*W pracy przyjęto wzmocnienie dla pierwszego stopnia projektowanego wzmacniacza na poziomie $K = 20 V/V$.
Czy w kontekście możliwości pojawienia się składowej stałej napięcia na wejściu wzmacniacza spowodowanego zjawiskami zachodzącymi na styku tkanka--elektroda wartość ta nie jest zbyt duża i czy nie będzie powodowała nasycenia stopnia wejściowego wzmacniacza?*

btj

Przede wszystkim, wzmocnienie takiego układu z definicji wynika ze stosunku pojemności i ono jest stałe, w tym przypadku $20 V/V$ -- pojemności nie są wyrażone w tych jednostkach oczywiście.

Sprzężenie zmiennoprądowe zapewnia usunięcie składowej stałej i nie ma obawy o nasycenie, ponieważ pojemności eliminują składową stałą sygnału.

---

kom 

*Niektóre fragmenty tekstu są dla mnie niezrozumiałe lub budzą pewne wątpliwości
[...]
Jak wspomniano wcześniej, w docelowym rozwiązaniu przewiduje się zastosowanie drugiego stopnia wzmacniającego. 
Przy założeniu, że kolejny stopień będzie miał wysoką impedancję wyjściową, może on być sterowany bezpośrednio z kaskody o wysokiej impedancji wyjściowej. 
Dla celów testowych potrzebujemy jednak stopnia wyjściowego o relatywnie niskiej impedancji wyjściowej, który skutkowałby zwiększeniem poboru mocy układu prototypowego.*

kom

Myślę, że to możemy pominąć, bo myślę, że to była tylko niefortunna gra słów.

---

kom

*Wzór 2.2 na str. 88 -- brak liczby 4 w mianowniku pod pierwiastkiem, nie wszystkie składowe wzoru są wyjaśnione i opisane.*

btj

Oczywiście brakowało czynnika 4 we wzorze, a poszczególne symbole nie zostały wytłumaczone w tekście rozprawy.
Sam wzór natomiast dotyczy jakościowego porównania krytycznych parametrów przedwzmacniacza: polaryzację, szumy wejściowe i zakres.

---

kom

*W pracy skupiono się na analizie własności i projektowaniu rezystora półprzewodnikowego, nieco mniej zajmując się samym wzmacniaczem -- który jest najważniejszym elementem pracy.
W szczególności dotyczy to parametru CMRR wzmacniacza.
Podobnie niewiele uwagi poświęcono napięciu offsetu wzmacniacza, chociaż jego obecność jest widoczna we wszystkich zarejestrowanych przebiegach.
Tu przydatne byłoby jakieś oszacowanie.
Konsekwencją takiego podejścia jest dość zwięzły opis samej struktury wzmacniacza i jego własności tu przydałaby się nieco bardziej obszerna analiza.*

*Wybór współczynnika THD do oceny parametrów wzmacniacza jest poprawny, ale w mojej opinii w pracy trochę za mało uwagi poświęcono innym, dość istotnym parametrom wzmacniacza mających wpływ na jakość rejestrowanych sygnałów np. takich jak liniowość fazy, odpowiedź na skok jednostkowy czy szybkość narastania (SR -- ang. slew rate).*

btj

Celem w tej pracy była głównie analiza nieliniowości pseudo-rezystora, dlatego skupiono się na opisie tej struktury i jej własności. 
Przy projektowaniu wzmacniacza wszystkie te parametry były brane pod uwagę, razem z innymi parametrami jak szumy czy wejściowe napięcie niezrównoważenia i szumy, co uznano za standardową procedurę optymalizacji pary różnicowej wchodzącej w skład teleskopowej kaskody pracującej jako operacyjny wzmacniacz transkonduktanycyjny

kom

Po prostu można było tylko podać te parametry albo założenia. Tak na przyszłość.

btj

Wracając do poziomu DC, który widać na poszczególnych kanałach. 
Wynika on z właściwości wtórnika źródłowego, który jest na wejściu i zapewnia odpowiednią impedancję wejściową.
Wspomniany efekt jest widoczny systematycznie na wszystkich kanałach -- ta wartość nie wynika z poziomu samego przedwzmacniacza, tylko ze wspominanej impedancji.

buch

Czyli to jest artefakt?

btj

W pewnym sensie można tak to nazwać.

---

kom

*Teza o dużym znaczeniu współczynnika THD dla niskoczęstotliwościowych składowych sygnałów nie jest poparta odpowiednimi przykładami uzasadniającymi to znaczenie.
Jednak wymagałoby to dokładniejszej analizy własności rejestrowanych sygnałów neuronalnych, co jednak wykracza poza zakres pracy.*

btj

Tutaj chcę podkreślić, że THD na poziomie 1 % nie jest wartością wyśrubowaną.
W pracy nie podejmowano dalszej optymalizacji THD, bo wtedy trzeba byłoby szukać uzasadnienia praktycznego.
THD jest powszechnie stosowaną miarą nieliniowości sygnału.
W literaturze spotkałam się tylko z jedną pracą, która pokazywała zależność współczynnika THD od sygnału.
Ci autorzy porównują swój układ z tą konwencjonalną metodą.
Zaproponowali własne rozwiązanie, ale sygnał wejściowy miał amplitudę $1,4 mV_{pp}$.
Ja optymalizowałam do $10 mV_{pp}$, ponieważ pokrywa on zakres sygnałów LFP, co będzie pokazane później na przykładzie zarejestrowanych danych z eksperymentu elektrofizjologicznego.

---

kom

*Zastanawiający jest brak w analizach widmowych zarejestrowanych sygnałów, składowych sieci i ich harmonicznych.
Być może zostały użyte filtry typu notch, ale nie wspomniano o tym w pracy.*

btj

Tutaj pozwoliłam sobie przedstawić wyniki weryfikujące widmową gęstość mocy szumów.
Po lewej są te z weryfikacji elektronicznej z uziemionymi wszystkimi wejściami.
Natomiast te po prawej zmierzono już razem z sondą wieloelektrodową w eksperymencie ze zwierzętami.
Odpowiednie dostosowanie warunków w eksperymencie elektrofizjologicznym umożliwia znaczną redukcję składowych sieci.
Jest widoczne delikatne 50 Hz, potem 150 Hz -- nie wymagało to jednak stworzenia osobnego filtru notch.
W laboratorium elektronicznym składowe te były trochę większe i je usuwałam w trakcie analizy danych.

---

## Publiczna dyskusja:

Opracowanie: dr inż. Paweł Jurgielewicz 