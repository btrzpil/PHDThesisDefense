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

buch

*Język rozprawy jest bardzo dobry, odnotowano jedynie nieliczne przypadki łączenia imiesłowu przysłówkowego ze stroną bierną.*

*Nie jest zachowany klasyczny układ publikacji naukowej, natomiast zaproponowany układ jest logiczny i przejrzysty.*

*Użycie bibliografii jest nieco utrudnione przez brak sortowania alfabetycznego.*

btj

Stosując sortowanie alfabetyczne, prawdopodobnie łatwiej byłoby się odnosić do artykułów poszczególnych autorów.

---

buch

*Cytowanie na ogół jest poprawne, jedynie cztery źródła to źródła internetowe, dla których jedynym adresem publikacyjnym jest strona www. 
Podane są one [...] bez daty dostępu, co jest błędem, jednak ich charakter nie wskazuje na ulotność, ponieważ są to w większości strony firmowe, zawierające charakterystyki produktów.*

btj 

Faktycznie doszło do pominięcia tych informacji.

---

buch 

*natomiast rysunki stanowiące autocytaty z prac, których współautorką jest Autorka, nie są oznaczone jako takie.*

Tak wykorzystywałam w pracy rysunki z publikacji, ale zostały one dostosowane i przeredagowane na potrzeby omawianej pracy.
Uznałam, że nie ma konieczności oznaczania ich jako autocytaty, w szczególności, że była autorem wszystkich tych grafik źródłowych również.

buch

W kontekście oryginalności dorobku spotkałem się z takim standardem, że rysunki, które były wcześniej opublikowane oddzielnie, przy czym lista autorów była dłuższa niż jeden, są odnoszone np. "porównaj", "zmodyfikowane wg."
W tym momencie nie ma wątpliwości dotyczącej tego, że...
W zasadzie, gdyby nie fakt, że jest to Pani praca, to należałoby zakwalifikować jako (auto)plagiat.

---

buch

*Protokół badania nie jest dokładnie opisany, ale zakłada badanie odpowiedzi wywołanej na mechaniczne drażnienie wibrys u szczura, z jednoczesną rejestracją aktywności LFP w obszarze od kory mózgowej (Cx) do wnętrza mózgu (Th).*

btj

Chciałam podkreślić, że eksperyment był wykonywany w Instytucie Biologii Doświadczalnej przy współudziale dr hab. Ewą Kublik zgodnie ze standardowo stosowaną przez nią procedurą badania odpowiedzi neuronalnych w korze mózgowej na mechaniczne drażnienie wibrys szczura oraz aktywności spontanicznej.
Protokół badania jest opisany na tyle, na ile wydawało mi się konieczne do zrozumienia zarejestrowanych przebiegów.
Ta procedura biologiczna, liczba powtórzeń i uśrednianie odpowiedzi było zaproponowane właśnie przez dr hab. Ewę Kublik wykonującej takie eksperymenty bardzo często, przez co ma odpowiednie doświadczenie.

buch

Tak to jest jasne.

---

buch

*Kod źródłowy skryptów wypracowanych w ramach pracy nie jest częścią rozprawy ani nie jest dostępny w publicznym repozytorium, choć publikacja kodu pomogłaby w ocenie kompetencji Autorki.*

buch

Moża przejść dalej...

---

buch

*w analizie stanu sztuki Autorka pomija dorobek jej macierzystego zespołu, chociaż go cytuje [...].
W związku z tym recenzent skazany jest na domysły.
Należy przyjąć, że istotną nowością omawianej pracy jest użycie pseudorezystorów, ponieważ ta technika nie pojawia się w tytułach wymienionych [...] powyżej pozycji dorobku.*

btj

Czy ta odpowiedź...

buch

Tak absolutnie. Sam ją zasugerowałem.
To jest inny przypadek, jeżeli mamy silny zespół pracujący przez dłuższy czas w tym samym obszarze tematycznym, w którym wiedza jest po prostu dokładana przez kolejne osoby wchodzące w badania.
Pani bardzo szczegółowo opisała stan sztuki w ogóle rozwiązań do pomiarów biologicznych.
Natomiast mi w tym stanie sztuki zabrakło dorobku macierzystej jednostki, która by pokazała, gdzie był ten punkt odcięcia, w którym Pani wkroczyła na scenę i zaczęła generować oryginalny, twórczy wkład.
Ponieważ zadaniem recenzji jest wyodrębnienie Pani wartości dodanej na bazie również wyników zespołu, również w kontekście faktu, że lista autorów publikacji jest szersza.
W związku z tym, gdyby taki rozdział się tam znalazł na koniec opisu stanu sztuki (opis dorobku zespołu badawczego), no to oczywiście by ułatwiło ocenę oryginalności Pani wkładu.

btj

To był całkowicie nowy projekt.

buch

Tak się domyśliłem.

---

buch

*Metodykę procesu badawczego należy podzielić na dwa etapy [...]. 
Pierwszy z tych etapów nie budzi zasadniczych wątpliwości. 
Jedyny zidentyfikowany brak dotyczy wspomnianych na str. 68 wolnozmiennych oscylacji, które nie zostały uwzględnione w scenariuszach testowych, a jak wspomniano wcześniej w tekście, mają istotne znacznie dla działalności wzmacniacza.*

btj

Pozwoliłam zaprezentować tutaj wykres, który przedstawia zależność współczynnika THD od częstotliwości sygnału wejściowego dla różnych ustawień częstotliwości granicznej.
Chciałam tutaj podkreślić, że pomiar tego typu charakterystyk wymaga bardzo długich pomiarów ze względu na uśrednianie sygnałów.
Nie byłam w stanie zmierzyć tego dla niższych częstotliwości, ponieważ w ich przypadku pomiar jednej krzywej trwałby kilka dni.

buch

Tu zasadniczo też jest dla mnie oczywiste, dlaczego Pani tak zrobiła, ale podobnie jak kolega, powiem, że właściwie zabrakło jednego zdania, które by wskazywało na to, że Pani jest świadoma tego, że warunki testowe, które Pani aplikuje do testowania konstrukcji, nie obejmują pełnego zakresu zniekształceń, z którymi może się Pani zetknąć w rzeczywistym pomiarze.

---

buch 

*W tekście cytowanych jest kilka rodzin modeli symulacyjnych tranzystora MOS, należy się domyślać, że w dalszym ciągu użyty został model EKV.*

btj

Model EKV nie jest zaimplementowany dla modeli tranzystorów w środowisku CADENCE, czyli narzędziach, które służą przeprowadzaniu symulacji submikronowych procesów technologicznych CMOS, ale jest pożyteczny w kontekście zrozumienia zjawisk fizycznych i porównaniu wyników symulacyjnych z tym, co otrzymujemy w szczególności, gdy opieramy się na parametrach brzegowych technologii.

buch

To ewidentnie wynika z interdyscyplinarności i pewne braki wiedzy oczywiście da się odczuć.

pf

Właśnie miałem o to pytać, dlaczego w ogóle Pani pisze o tym (modelu EKV), gdy w CADENCE PSIM, więc dostałem już odpowiedź.
Mówiąc o tym, że to ułatwia zrozumienie -- model powinien być jak najbliższy odtwarzaniu zjawisk fizycznych, żeby eliminować parametry strojenia i aproksymacji matematycznych z sufitu.
Czy Pani to w pracy wykorzystała w jakiś sposób?

btj

Nie, używałam modeli symulacyjnych z CADENCE. 
Jednak przy próbie interpretacji właściwości bez fizycznego układu używałam EKV.

pf

Dziękuję

---

buch

*Pewne wątpliwości budzi natomiast metodyka procesu weryfikacji w eksperymencie neurofizjologicznym.
W przypadku pomiarów o charakterze unikatowym nie ma możliwości porównania wyniku z urządzeniami referencyjnymi.
Wydaje się jednak, że ten przypadek tu nie zachodzi.
Bardziej właściwe wydaje się porównanie omawianego urządzenia pomiarowego z urządzeniem referencyjnym w sposób, który wykaże prawidłowość realizowanych za jego pomocą pomiarów.
Istnieją również wspierające ten proces metody statystyczne, takie jak metoda Blanda-Altmana.*

*W przypadku niniejszej pracy zastosowano jakościową metodę weryfikacji, którą jest zgodność otrzymanych z użyciem urządzenia wyników z oczekiwaniami eksperymentatora.
Oczekiwania te zbudowane są na podstawie dostępnej wiedzy, a ta zawiera oczywiście wyniki pomiarów, które można uznać za referencyjne.
Jednak nie ulega wątpliwości, że tego typu analiza jest dużo słabsza z perspektywy matematycznej niż analiza porównawcza dwóch urządzeń korzystających z tego samego źródła sygnału.*

btj

Eksperyment biologiczny był przeprowadzony całkowicie w oparciu na doświadczeniu i autorytecie dr hab. Ewy Kublik.
Ona ma do czynienia z różnymi systemami pomiarowymi, stąd uznałam takie podejście za wystarczające. 

---

buch

*wykres przedstawiony na rys. 2.4 przedstawia filtr górnoprzepustowy, a nie dolnoprzepustowy (wysoka impedancja występuje w paśmie niskich częstotliwości, a impedancja w paśmie wysokich częstości jest niska).*

btj

Ten model nie przedstawia filtru, tylko model impedancji elektrody w zależności od częstotliwości sygnału.

---

buch

*Autorka opisuje proces inżynierski z perspektywy ex post. 
W związku z tym zdarza się, że relacjonując wykonane badanie, czy analizę nie umieszcza na końcu rozdziału wniosków z tego badania.
Pojawiają się one niejako mimochodem jako uzasadnienie decyzji projektowej, której podjęcie jest relacjonowane w rozdziale następnym.
Taka sytuacja występuje na granicy rozdziałów 3.2.1 i 3.2.2, kiedy zostaje w zasadzie podjęta decyzja o eliminacji z dalszych rozważań konfiguracji variable-$V_{gs}$, do czego przesłanki dostarcza rozdział 3.2.1.
Co do rozdziału 3.2.1 to skądinąd nie jest od początku jasne, w jakim celu są prowadzone opisywane w nim rozważania.
Staje się to jasne w rozdziale 3.2.2, kiedy okazuje się, że celem tego rozdziału było rozważenie przesłanek za wyborem jednej z dwóch konfiguracji.*

*Zdarza się również, że Autorka uznaje, że wniosek w sposób oczywisty wynika z przedstawionych wykresów, co nie jest oczywiste w interdyscyplinarnym środowisku odbiorców.
Taka sytuacja występuje na granicy rozdziałów 3.3 oraz 3.4.
Wniosek z rysunku 3.12, który kończy analizę z rozdziału 3.3, jest podsumowany w pierwszym akapicie rozdziału 3.4.
Takich sytuacji jest więcej, ale nie spotkałem się z oczywistą luką i brakiem informacji, a co najwyżej z jej nieodpowiednią lokalizacją.*

btj

Nie jestem już w stanie niestety poprawić tekstu, ale rozumiem uwagi, że całość mogła przysporzyć trudność podczas czytania.

---

buch

*Kilkukrotnie Autorka traktuje uzyskane wyniki jako oczywiste i nie tłumaczy, która z cech wykresu dowodzi wyciąganego wniosku.
W kilku przypadkach cechą tą jest różnica nachyleń między dwoma połówkami wykresy -- sytuacja ta dotyczy rys 3.11 oraz 5.18.*

btj

O które nachylenia chodziło Panu konkretnie w tych przypadkach?

buch

Nie przypomnę sobie precyzyjnie, ale z tego, co pamiętam, konkluzja płynąca z rysunku wynikała z faktu różnicy nachyleń, która nie była komentowana, ale później oczywiście *[fragment nieczytelny]*

---

buch

*Z całkowitych drobiazgów należy zwrócić uwagę na tabelę 3.1, w której zmienna $R_f$ powinna stanowić kolejną kolumnę tabeli.*

btj

Tak, ta tabela mogłaby wyglądać tak, jak na prezentowanym slajdzie.

---

buch

*Warto również odnotować niekonsekwentny charakter opisu procesów fizykochemicznych zachodzących po stronie tkanki, które czasem opisywane są jako procesy jonowe, czasem jako procesy elektrochemiczne, a czasem odnoszone są do pojęcia warstwy podwójnej i efektów pojemnościowych.
Co do zasady użyte modele matematyczne nie budzą wątpliwości, choć model matematyczny tkanki jest zdawkowy [...]*

btj

Uznałam, że na potrzeby wyznaczenia celów projektowych jest to wystarczające.
W pracy skupiałam się na optymalizacji parametrów przedwzmacniacza.

buch

Możemy do tego wrócić ewentualnie w dyskusji, ale wytłumaczę się, skąd się bierze moja wątpliwość.
W schemacie tego pomiaru, który zakłada te izolujące kondensatory na wejściu, które powodują, że sprzężenie na wejściu jest zmiennoprądowe, to Pani odnosi się do wartości pojemności tych kondensatorów i później na nich opiera późniejsze wymagania dotyczące własności tych konstrukcji, czyli np. dotyczące częstotliwości odcięcia.
Te parametry pojemności są elementem ujawnionym w procesie projektowym.
Kiedy popatrzyłem na ten wykres, zacząłem się zastanawiać, czy to są jedyne pojemności, które w tym procesie należałoby uwzględnić i co się dzieje po drugiej stronie tych kropeczek, które zaczynają ten tor pomiarowy.
Jeżeli tam też występują jakieś pojemności, to one zasadniczo również się tu dodadzą.
Jestem świadom, że nie jest to zarzut do Pani, dlatego że założenie o rezystancyjnym charakterze tkanki jest absolutnie powszechne.
Proszę więc nie odbierać tego, jako personalny zarzut.
Natomiast te moje wątpliwości się w pewnym sensie potwierdziły w obserwacji, do której się Pani odnosi we własnych pomiarach, czyli tym odwróceniu fazy na "zerowej" elektrodzie, które było pokazane w części pomiarowej.
Oczywiście nie badałem głębiej tego zjawiska, to jest analiza na poziomie "machania rękami".
Być może wpływ własności pojemnościowych tkanki należałoby się doszukiwać w źródłach tego zjawiska, dlaczego tak się stało że tam się ta faza odwróciła przy niewielkiej odległości między elektrodami.
To jest taki temat, który stawiam bardziej ze znakiem zapytania niż z kropką.

btj

Do tego jeszcze przejdę za chwilę.

---

buch

*Co do mankamentów merytorycznych, występujących w dysertacji, jest ich kilka.
Pierwszy z nich [...] dotyczy faktu, że model źródła, tkanki i sprzężenia jest niejednoznaczny i nie do końca odpowiada rzeczywistości pomiarowej.
Niezależnie od widma samego źródła, skumulowane efekty pojemności i lokalnego przewodzenia w tkance, nakładają na źródła swoją charakterystykę, która faworyzuje niskie częstotliwości [8].
Efekty jonowe są składową tego zjawiska [9] ale nie mają dominującego charakteru [10].*

*Potencjał stały jest przede wszystkim efektem brzegowym, związanym z tworzeniem warstwy podwójnej, które z kolei wynika z różnicy potencjałów chemicznych między kontaktującymi się fazami [10].
Oczywiście rozdzielenie ładunku objętościowego również zachodzi [9], ale jest to efekt fizyczny, a nie fizykochemiczny.
Przemiany elektrochemiczne modą zachodzić, dopiero gdy przekroczona jest określona energia aktywacji [10].
W odniesieniu do elektrod stymulujących piszą o tym Merrill i wsp. -- pozycja [113] literatury -- te rozważania można rozszerzyć na elektrody pomiarowe [8-10].*

*Fluktuacje termiczne dotyczą nie tylko rezystancji, ale również pojemności -- taki proces jak tworzenie warstwy podwójnej również jest poddany fluktuacjom.
W związku z tym nie ma potrzeby odwoływania się do rezystancyjnej natury tkanki, po to, żeby uzasadnić użycie twierdzenia Nyquista.
Należy to raczej uznać za brak modelu.
Również rezystywny charakter tkanki nerwowej można poddać w wątpliwość -- cytowany przez Autorkę Destexhe ma w swoim dorobku pracę [7] poświęconą temu zagadnieniu.*

btj

W pracy podczas wyznaczania wymagań dla systemu, ze względu na charakter sygnałów, opierano się na wiedzy literaturowej oraz doświadczeniu osób rejestrujących takie sygnały.
Dodatkowo zakładano, że w przypadku mikroelektrod umiejscowionych w bezpośrednim sąsiedztwie komórki nerwowej główny dominujący wpływ ma rezystywny charakter medium. 
Wiem, że w pomiarach EEG wyzwaniem jest modelowanie charakteru rejestrowanych odpowiedzi, ponieważ tam występuje silne tłumienie przez czaszkę przez kolejne różne struktury o odmiennym charakterze impedancyjnym.
Tu stosowano się do uproszczonego modelu.

buch

Nawet jeżeli ostatni stopień jest rezystancyjny, bo czaszka można się spodziewać, że ma taki charakter, to w tym momencie należy uznać, że to sprzężenie następuje z pojemnościami, które są głębiej.
Tutaj ze zdaniem Pani, że w niskich częstotliwościach efekty pojemnościowe nie występują, to ja bym raczej polemizował, bo jeżeli efekty pojemnościowe gdzieś występują to właśnie w niskich częstotliwościach ze względu na charakter dyspersji.
Jeżeli się spytać rasowego elektroników, gdzie kondensator ma większą pojemność, a gdzie mniejszą to oni natychmiast odpowiedzą, że w wysokich częstotliwościach ma mniejszą pojemność.
Idźmy dalej.

---

buchner

*Czynnikiem, który w sposób zasadniczy wpływa na model błędu i model sprzężenia tkanki z elektrodą jest lokalizacja elektrody referencyjnej.
Nie ulega wątpliwości, że sonda MEA jest czymś zupełnie innym niż elektroda referencyjna, więc pomiar jest asymetryczny.
Nie zmienia to jednak faktu, że nadal jest to pomiar bipolarny.
Niektóre konstrukcje, takie jak opisywany przez Autorkę Neuropixel, są bipolarne i symetryczne (por rys. 2.8, także rys. 2.13) inne nie są (rys. 2.12, 3.7!).
Zdecydowanie brakuje odniesienia do tej fundamentalnej różnicy.
Im dalej umieszczona jest elektroda referencyjna, tym większy wpływ na sygnał ma interferencja 50 Hz, oraz wszystkie źródła endogenne, w szczególności silny sygnał kardiogenny.
Przy odległej lokalizacji elektrody odniesienia trudno jest interpretować otrzymane przebiegi jako neurogenne.*

btj

W praktyce trudno jest zapewnić idealnie symetryczny pomiar, ponieważ impedancja elektrody referencyjne jest zawsze inna niż elektrody pomiarowej, nawet w przypadku sondy Neuropixel. 
Możliwym rozwiązaniem, stosowanym zresztą powszechnie, jest wykonanie elektrody referencyjnej o możliwie małej impedancji, co zapewni lepszą symetryzację tych wejść.
Oczywiście nie zapewnia to tłumienia sygnałów współbieżnych generowanych w badanej tkance, ale pomaga w tłumieniu sygnałów współbieżnych pochodzących z zakłóceń elektromagnetycznych. 
Na przykładzie, wzmacniacz Neuropixel jest różnicowo-różnicowy, czyli wyjście jest różnicowe, ale tak jest w najnowszej jego wersji -- poprzednio było to różnicowo-singlended, czyli z pojedynczym wyjściem sygnału.
Wynika z tego, jak komponowany jest kolejny stopień.
Jest to związane z tym, o czym mówiłam wcześniej.
Ten model, do którego się Pan odnosi z jedną linią sygnałową, jest to uproszczony schemat przedstawiający przesłuchy na poszczególnych kanałach.
Wzmacniacz jest oczywiście różnicowy, jednak aby zamodelować efekty przesłuchów tak to narysowałam dla ułatwienia.

buch

Proszę mieć świadomość, że jeśli umieści Pani elektrodę referencyjną np. na prawej nodze, w tym momencie źródłem sygnału staje się wszystko, co jest między badanym punktem na sondzie neuronowej a prawą nogą.
To jest ta świadomość, której również dość powszechnie w tych pomiarach brakuje.
Jak widzę wielokanałowe zapisy z powierzchni klatki piersiowej, tam nie ma nigdzie informacji, o tym, gdzie została zlokalizowana elektroda referencyjna.
To jest, znowu, ogólna uwaga.

---

buch

*Odwrócenie amplitudy obserwowane na elektrodzie $0$ wygląda w pierwszym przybliżeniu na wynik zmiany fazy wynikający ze sprzężenia pojemnościowego -- trudno byłoby zinterpretować odwrócenie amplitudy wprost jako odwrócenie kierunku prądu -- jest to jeden z najciekawszych wyników dotyczących samych narzędzi, sugerujący konieczność dalszego rozwoju techniki modelowania.*

btj

Różnica czasu między poszczególnymi rejestracjami wynosiła ok. 100 minut.
Na podstawie wcześniejszych eksperymentów, może dochodzić do efektów mechanicznej relaksacji tkanki i względnego przemieszczenia się źródeł.

buch

Jeżeli do implantowania elektrody dochodzi do powstania np. krwiaka, który w funkcji czasu jest niestabilny, to jest to czynnik, który ma wpływ na pomiary.
Natomiast można to wyeliminować poprzez kilkukrotne powtarzanie eksperymentu na różnych zwierzętach, zmieniając kolejność pomiarów.
W tym momencie można do pewnego stopnia to zniwelować

btj

W tym eksperymencie, ze względu na możliwości nie mogłam powtórzyć pomiaru.

buch

Nie dyskutuję.

---

buch 

*Odnośnie podnoszonego przez Autorkę faktu zniknięcia podwójnego maksimum widma THD, warto zauważyć, że rozwiązanie takie występowało już jako jeden z wariantów widma w analizie Monte-Carlo (rys 4.9) oraz wykazywało silną zależność od pojemności $C_{gb}$ (rys 3.10), co mogło być przyczyną obserwowanych różnic między widmem zmierzonym a wynikami symulacji.*

btj

Środowisko symulacyjne nie uwzględnia wszystkich efektów brzegowych -- bardziej wiarygodne są wyniki z weryfikacji elektronicznej.
Zatem aż tak bardzo nie przywiązywałam się do tego, że te dwa maksima występują.
Silna zależność od częstotliwości granicznej *[fragment nieczytelny]* i wartość amplitudy są porównywalne, co świadczy o dobrym opisie danych przez symulację.
Jednak wpływ tych pojemności nie jest dokładnie taki, jaki przewidują modele.

buch

Jestem usatysfakcjonowany.

__*Koniec odpowiedzi do uwag wyrażonych w recenzjach*__

## Publiczna dyskusja:

żoł

Proszę mi powiedzieć, dlaczego to THD jest tak ważne dla tych niskich częstotliwości? Nie dla wysokich (AP).

btj

Krytyczny zakres LFP 0,5 Hz do 100 Hz -- w takim zakresie zniekształcenia 20% czy 10% są bardzo duże.
W literaturze typowo podaje się ten współczynnik dla 1 kHz i tam THD jest stosunkowo niższy.

żoł

Jeszcze raz -- dlaczego to ma znaczenie i co oznaczają te kreski czerwone?

btj

To jest zakres zakłóceń elektromagnetycznych sieci 50Hz/60Hz.
LFP pokrywają się z tym zakresem -- krytyczne jest też uwzględnianie tego efektu w CMRR również.

żoł

Jakby mogła Pani pokazać slajd z pomiarów na szczurach z LFP -- no właśnie dlaczego akurat w tej części pasma te zniekształcenia mają znaczenie>?

btj 

Tutaj obserwowaliśmy odpowiedź na mechaniczną stymulację wibrys w korze baryłkowej jako przykład sygnałów LFP, który można rejestrować.
Kształt odpowiedzi pokrywa się z oczekiwanym,

żoł

Dlaczego tutaj ma to znaczenie, a nie w AP?

btj

Bo tam są one na akceptowalnym poziomie, więc nie ma znaczenia THD w przypadku potencjałów czynnościowych, ponieważ ich częstotliwość jest w okolicy tego 1 kHz.

żoł

Chodzi mi o analizę sygnałów późniejszą. Jakie to ma znaczenie dla analizy

btj

LFP, czyli odpowiedź lokalnej populacji neuronów.
Zasięg tych sygnałów może być jednak szerszy -- silne źródła sygnału w dalszej odległości i bliższe źródła, ale słabsze.
Jeżeli zniekształcenia będą duże, nie da modelować charakteru źródeł sygnałowych na podstawie rejestracji.

żoł
Jak te zniekształcenia będą duże, tym trudniej jest...

btj

*[fragment nieczytelny]*

żoł

A ten 1% skąd się bierze? To jest hołd dla systemu dziesiętnego czy coś więcej?

btj

Tak. Należało wybrać jakąś wartość.
Nieraz w literaturze pojawia się "1% osiągnięto dla amplitudy sygnału $10 mV_{pp}$ i częstotliwości 1 kHz.
Stąd wzięłam ten 1% jako satysfakcjonujący wskaźnik.

żoł

Rozumiem, Pani bardziej optymalizowała, niż poszukiwała wartości.

btj

Tak jak powiedziałam wcześniej, należałoby przeprowadzić analizę sygnałów biologicznych do określenia, jaki poziom zniekształceń jest wystarczający.

żoł

Ten parametr możemy polepszać lub pogarszać kosztem czego głównie? Jakiego parametru?

btj

Pojemność.

żoł

Pojemność miałaby wpływ na co?

btj

Na powierzchnię.
Używamy tranzystorów jako elementów rezystancyjnych -- one mają charakter nieliniowy.
Można zmniejszyć udział rezystancji w sprzężeniu zwrotnym i dać większy udział pojemności, która będzie bardziej liniowa (będzie to też korzystniejsze pod kątem szumów).
Nie można jednak w nieskończoność zwiększać tej pojemności, ponieważ to kosztuje powierzchnię.
Pojemność $4 pF$ dla jednego kondensatora zajmuje $200 \mu m^2$, a powierzchnia całego przedwzmacniacza, czyli tego całego układu ze wzmacniaczem transkonduktancyjnym z dwoma pojemnościami, rezystorem wynosi tyle *[wartość na slajdzie]*. 
*[Fizyczna wielkość elementu pojemnościowego]* stanowi to znaczący czynnik optymalizowany w tego typu wielokanałowych systemach.

dąb

Tutaj Pani wspomniała, jednak w pracy nie ma dyskusji na ten temat -- ten wzmacniacz może znaleźć zastosowanie w rozwiązaniach z jednoczesną stymulacją elektryczną.
Kiedy robimy stymulację elektryczną, to generujemy olbrzymie artefakty.
Kasowanie tych artefaktów zachodzi różnymi technikami, ale będzie się sprowadzać do odejmowania jakichś dwóch sygnałów -- tego artefaktu stymulacyjnego i rejestracji.
Kiedy zaczynamy odejmować dwie duże wielkości, to te zniekształcenia sygnału jeszcze bardziej się uwidaczniają i jest to jeszcze bardziej krytyczne.
Jest to ten drugi aspekt, trochę z tyłu głowy, w kontekście dalszego rozwoju tej techniki.

buch

Warto jeszcze zauważyć, że ta pojemność, która jest krytyczną czynnikiem, jeżeli chcemy ją zamknąć w układzie scalonym, to jest elementem ograniczającym.
Natomiast można ją wyprowadzić na zewnątrz do elektrody i w tym momencie użycie warstw pojemnościowych na interfejsie między metalem a mierzoną tkanką.
Tam są duże możliwości, jeśli chodzi o nowe materiały, które również u Państwa są budowane odnośnie tego, by zbudować tam układ pojemnościowy poza strukturami przedwzmacniacza.

ph

A czy taka pojemność nie będzie miała potem takiego upływu DC?

buch

To znaczy elektrody AgAgCl są stosowane powszechnie w praktyce medycznej, i możemy dyskutować.

btj

Ale jest jeszcze sprawa dopasowania impedancji do wzmacniacza, by nie powodować tłumienia sygnału

buch 

Zostawmy może ten temat i przejdźmy do dalszej dyskusji.

żoł

Tak się głośno zastanawiam.
Jeśli pójść w tym kierunku ADC, czy to jest tak ważne, żeby te nieliniowości *[fragment nieczytelny]*

buch

Wspomniany tu był potencjał kontaktowy o dużej składowej stałej.
Użycie elektrod AgAgCl pozwala na automatyczne kompensowanie składowej stałej, tak przynajmniej twierdzą elektrochemicy -- ja nigdy tego nie weryfikowałem.

---

pf

Jako ciekawski troszkę o technologię.
Mianowicie Pani wspomina w projekcie masek technologicznych, czyli przy projektowaniu topografii o tym, że jest to projekt krytyczny ze względu na zapewnienie jednorodności wzmocnienia kanałów odczytowych.
Co Pani przez to stwierdzenie rozumie? Jak to się przekłada na projekt, który Pani wykonała?

btj

Integracja wielu kanałów odczytowych powinna skutkować jednorodnością parametrów elektronicznych, żeby rejestrowane sygnały były porównywalne.
Stosowanie indywidualnej korekty jest możliwe, jednak te bloki będą zajmowały dodatkową powierzchnię. 
Dla prezentowanego systemu stworzyłam blok korekty.
Polaryzacja tranzystorów zależy od napięcia pomiędzy bramką a źródłem. 
Rozrzut technologiczny tych par tranzystorów mógłby spowodować różnicę rezystancji, co implikowałoby różnicę częstotliwości granicznej np. 0.1 Hz vs 0.2 Hz między kanałami.
Blok ten umożliwiałby kalibrowanie systemu i uzyskanie jednorodnych parametrów w całym układzie.

pf

Rozumiem. Ja troszkę inaczej odebrałem to stwierdzenie, że Pani zastosowała pewne specyficzne zabiegi przy projektowaniu topografii poszczególnych elementów.

btj

Tylko standardowe techniki dotyczące np. rozmieszczania pary różnicowej.

pf

To jak Pani zrealizowała parę różnicową w kontekście zaburzeń procesu technologicznego?
Pani zrobiła analizy Monte-Carlo -- one odnoszą się wyłącznie do zaburzeń o charakterze pseudolosowym. 
Natomiast mamy też deterministyczne

btj

Jak layout optymalizowałem?

pf

Tak, bo Pani tutaj o projekcie masek napisała, dlatego o to zapytałem. 
Jak Pani parę różnicową zaprojektowała?

btj

Niestety nie mam tego obrazka...

pf 

To może Pani opowiedzieć.

btj

Jest znaczna różnica "W" i "L".
Obie pary różnicowe muszą znajdować się blisko siebie i muszą być skonfigurowane na centroidowej tak samo.

pf

"Common centroid", tak?

btj

Tak. *[fragment nieczytelny]*

pf

Dobrze, już wiem, co Pani zrobiła, dziękuję.

---

żoł

Jak wyglądał układ pomiarowy do pomiarów in-vivo czy to jest ten sam, który był na zdjęciu wcześniej?

btj

Tak, to ta sama płytka, jednak z drobnymi zmianami. 
Trzeba było zmodyfikować system akwizycji danych oraz wejście sygnałów.
Wykorzystanie przełączników umożliwiło wykorzystanie wejść z sondy Neuronexus.

żoł

W takim razie odległość między układem scalonym a elektrodą była dosyć znaczna.
Te sygnały są stosunkowo słabe.

btj

Pomiary odbywały się w klatce Faradaya, co separuje od zewnętrznych źródeł.

żoł

Sama pojemność przewodu musiała być znaczna, który prowadził ten sygnał do układu scalonego. Kilka centymetrów, koncentryczny kabel, ale sobie radziło, jak rozumiem?

btj

Tak, opieraliśmy się też na wiedzy eksperymentatora i w jej opinii to nie było problemem.

żoł

Właśnie mówię o AP, gdzie mamy $10 \mu V$ .

btj

Dla LFP to nie będzie problemem.
W tym konkretnym przypadku obserwowano potencjały czynnościowe o amplitudzie $1 mV$.

żoł

Dosyć mocne.

btj

Tak. Rejestracja przebiegała we wzgórzu, a nie w korze, ponieważ tam występują mocniejsze potencjały czynnościowe i to są również jedne z większych amplitud znanych w literaturze ($50 \mu V$ do właśnie $1 mV$). 

żoł

To właśnie wydawało mi się podejrzane. Tak właśnie kojarzę AP o amplitudach rzędu $100 \mu V$, a tutaj widzę, że się właśnie nie zgubiły.

buch

Taki temat: impedancja falowa tego obwodu wejściowego

btj

Impedancja falowa będzie miała znaczenie przy wyższych częstotliwościach sygnału -- tutaj jednak to nie są gigahertze i nie ma linii długiej.

żoł

Jakie jeszcze były zabiegi związane z zasilaniem tego układu scalonego by nie interferowało to z rejestrowanymi sygnałami? Stabilizator? Kondensator?

btj

Na płytce drukowanej zostały zastosowane pojemności odsprzęgające.

buch

W badaniach tego typu nie ma wymogu stosowania transoptora?

btj

Translatora napięć?

buch

Transoptora.

żoł

Chodzi o to, że z drugiej strony jest duża karta cyfrowa i cały pecet, który bardzo mocno "sieje".

buch

Chodzi o izolację galwaniczną toru pomiarowego od źródeł zasilania.
W ludzkich pomiarach np. 

btj

*[fragment nieczytelny]*

kom

Chodzi o barierę galwaniczną, czyli odseparowanie zasilania od toru pomiarowego. 
Czy przeprowadzała Pani pomiary na pececie zasilanym z gniazdka, czy na notebooku zasilanym z baterii?

btj

Z gniazdka.

buch

Tak jak już kilka razy padło, nie miała Pani wpływu na schemat układu pomiarowego i warunki wykonywania pomiaru były standardowe.
W związku z tym również świadomość osób wykonujących te pomiary też była standardowa...

kom

Czy wykorzystano kartę pomiarową National Instruments?

btj

Tak.

kom 

Czy miała izolację galwaniczną? *[fragment nieczytelny]*

btj

Nie.

dąbr

Nie, na pewno nie.

kom

To bardziej dotyczy bezpieczeństwa tak naprawdę, gdyż tej sieci w sygnałach nie było widać.

btj

Sygnał sieci był widoczny przy weryfikacji elektronicznej.

kom

Z moich doświadczeń wynika, że użycie notebooka w tego typu pomiarach z zasilaniem bateryjnym znacząco pomaga.
O ile jest taka możliwość. 

żoł

Te szumy zmierzone, jaką miały wartość?

btj

Takie jak wynika z tabeli na slajdzie.

żoł

Te szumy są dosyć dobre.

---

pf

Jeszcze wrócę do technologii.
Inżynier, jak chce coś zaprojektować, musi wybrać producenta i odpowiednią generację technologii i Pani w jednym z rozdziałów rozważa wpływ na zniekształcenia powierzchni bramki i grubości tlenku i porównuje Pani wyniki dla trzech wybranych technologii o różnym wymiarze charakterystycznym.
Ponieważ powierzchnie, jakie Pani stosuje, są duże, no to ten wymiar minimalny nie ma właściwie żadnego znaczenia, tylko grubość tlenku.
Pani tylko wspomina o tym, że grube tlenki Pani wybierała, ale czy mogłaby Pani to jakoś skonkretyzować.
W większości technologii dostępne są tranzystory na różne napięcia progowe.
W różny sposób to można kształtować m.in. grubością tlenku.
Czy Pani może pamięta, jakie to były grubości? 
Co to znaczy gruby tlenek tutaj?

btj

Technologia zapewnia podstawowe wersje elementów, które można modyfikować, stosując grubszą warstwę tlenku i dostosowywać tym samym do wyższych napięć zasilania.
W wariancie podstawowym jest to $1.8 V$, a ja wykorzystywałam tranzystory $5 V$ - nie pamiętam jednak konkretnych wymiarów. 

pf

Tak, chodziło mi o grubość, z ciekawości.

btj

Ta technologia miała też inne korzystne własności: warstwa SOI, izolacja podłoża.

pf

Dobrze, dziękuję.

__*koniec dyskusji*__

Opracowanie: dr inż. Paweł Jurgielewicz 