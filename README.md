#Simple CGM 2009 Edycja Szkolna
Copyright (c) 2016 <a href="mailto:simple.cgm.2009@gmail.com" title="Mariusz Woźnica">Mariusz Woźnica</a>

![logo](/Images/scanner-os.png)

Aplikacja mobilna **Simple CGM 2009 Edycja Szkolna** powstała dzięki inicjatywie **[Teresy Woźnicy](http://www.facebook.com/teresa.woznica.58)**, grupa Facebook **[Cukrzyca typ 1 - odzyskajmy kolory zycia :)](https://www.facebook.com/groups/140046209720733/)**, która przekazała jasne i praktyczne oczekiwania funkcjonalne w stosunku do aplikacji.

Korzystając z okazji, pragnę w tym miejscu, jeszcze raz serdecznie podziękać **[Teresie](http://www.facebook.com/teresa.woznica.58)** za jej pomoc, inspirację i okazaną cierpliwość. Merytoryczne uwagi, z perspektywy **Mamy** opiekującej się dzieckiem z CT1 w wieku szkolnym, oparte na zdrowym rozsądku, pozwoliły zbudować proste i użyteczne narzędzie. Mam nadzieję, że dzięki temu, aplikacja **Simple CGM 2009 Edycja Szkolna**, okaże się równie pomocna dla wszystkich zainteresowanych.

Dodatkowo publikuję aplikację mobilną **[Simple CGM 2009](https://github.com/woznica1970/simple-cgm)**, o większym zakresie funkcjonalnym.

# O aplikacji

**Simple CGM 2009 Edycja Szkolna** powstała jako responsywna aplikacja mobilna i służy do wizualizacji pomiarów glikemii na podstawie wartości odczytywanych z sensora *[FreeStyle Libre](http://www.freestylelibre.pl/)* przez aplikację *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)*, zapisywanych następnie w aplikacji *[Nightscout](http://nightscout.pl/instalacja/)* oraz usłudze *[Dropbox](https://www.dropbox.com/)*, w celu udostępniania osobom sprawującym opiekę nad dzieckiem z CT1 np. nauczycielowi, podglądu wartości glikemii u dziecka na jego prywatnym smartfonie.

Aplikacja może pracować w trybie **publicznym** lub trybie **prywatnym**. Pozwala to ograniczyć dostęp do danych medycznych dziecka i zapewnić odpowiednią ochronę prywatności, a równocześnie pozwala ich opiekunom na podgląd wartości glikemii w określonych dniach i godzinach.

Brzmi to może trochę skomplikowanie, ale nie wiem jak opisać to rozwiązanie w prosty sposób, dlatego na poniższym schemacie staram się zilustrować poszczególne elementy systemu.

W naszym przypadku, dziecko może skanować się zarówno za pomocą zegarka [Sony SmartWatch 3 SWR50](http://www.sonymobile.com/pl/products/smart-products/smartwatch-3-swr50/#yellow), jak i za pomocą smartfonu [Sony Xperia E5](http://www.sonymobile.com/pl/products/phones/xperia-e5/). Podczas pobytu w szkole, smartfon schowany jest do teczki, a dziecko skanuje się tylko zegarkiem. Dodatkowo nauczyciel widzi pomiar glikemii na swoim smartfonie za pomocą aplikacji *[Simple CGM 2009 Edycja Szkolna](https://github.com/woznica1970/simple-cgm-school)*. Aplikacja *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* przesyła pomiar glikemii z zegarka, za pomocą smartfonu do aplikacji *[Nightscout](http://nightscout.pl/instalacja/)*, zainstalowanej w serwisie *[Azure](https://azure.microsoft.com/pl-pl/)*. Sama aplikacji *[Nightscout](http://nightscout.pl/instalacja/)* przechowuje  pomiary glikemii w bazie *[mLab](Https://mlab.com/welcome/)*. Równolegle aplikacja *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* przesyła pomiar glikemii do pliku przechowywanego w serwisie *[Dropbox](https://www.dropbox.com/)*.

**Simple CGM 2009 Edycja Szkolna** jest zainstalowana w serwisie *[Azure](https://azure.microsoft.com/pl-pl/)*, obok aplikacji *[Nightscout](http://nightscout.pl/instalacja/)* i pobiera pomiary glikemii **jednocześnie** z bazy *[mLab](Https://mlab.com/welcome/)* oraz z pliku zapisanego w serwisie *[Dropbox](https://www.dropbox.com/)*.

Dzięki temu otrzymujemy większą gwarancję niezawodności działania systemu, ponieważ na wypadek awarii jednego ze źródeł danych, możemy w dalszym ciągu wyświetlić pomiar glikemii na naszym smartfonie.

![schemat](/Images/Demo/schemat.jpg)

**Simple CGM 2009 Edycja Szkolna** możesz uruchomić na dowolnym urządzeniu obsługującym przeglądarkę internetową z włączoną obsługą JavaScript, takim jak komputer, tablet, smartfon.
Działanie **Simple CGM 2009 Edycja Szkolna** przetestowałem w popularnych przeglądarkach Chrome, Safari, Firefox, Opera, IE, oraz w systemach operacyjnych Android, iOS, Windows Phone. Aplikacja działa prawidłowo na wszytkich współczesnych smartfonach popularnych producentów. Wydajność aplikacji zależy oczywiście od specyfikacji technicznej konkretnego smartfona oraz jakości połączenia do Internetu.

Zachęcam użytkowników smartfonów **iPhone** do utworzenia skrótu do **Simple CGM 2009 Edycja Szkolna** na pulpicie za pomocą funkcji menu *Dodaj do ekranu początkowego* z przeglądarki Safari . Pozwoli to na uruchamianie aplikacji w trybie pełnoekranowym. Proszę tylko pamiętać, że aplikacja uruchomiona w trybie pełnoekranowym wymaga ponownego wpisania **Secret Key**. Podobna funkcjonalność jest również dostępna dla użytkowników smartfonów z systemem Android.


**Simple CGM 2009 Edycja Szkolna** wymaga do poprawnego działania, abyś wcześniej posiadał poprawnie zainstalowane i skonfigurowane aplikacje *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)*, *[Nightscout](http://nightscout.pl/instalacja/)* oraz konto w serwisie *[Dropbox](https://www.dropbox.com/)*.
Pamiętaj również, aby w aplikacji *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* zdefiniować w menu **_Options\Remote glucose monitoring_** dwa konta *[Dropbox](https://www.dropbox.com/)* i *[Nightscout](http://nightscout.pl/instalacja/)*.


**Simple CGM 2009 Edycja Szkolna** uruchamiasz wpisując do przeglądarki internetowej **adres url**, zdefinowany przez Ciebie dla aplikacji podczas procesu instalacji w serwisie *[Azure](https://azure.microsoft.com/pl-pl/free/)*.


**Simple CGM 2009 Edycja Szkolna** nie jest aplikacją oficjalnie zatwierdzoną przez firmę [Abbott](http://xidoneo.pl/) i nie daje żadnej gwarancji co do poprawności odczytu wartości glikemii z z sensora *[FreeStyle Libre](http://www.freestylelibre.pl/)* oraz nie jest przeznaczona jako substytut lekarza diabetologa. W przypadku jakichkolwiek pytań lub wątpliwości musisz skontaktować się ze swoim lekarzem specjalistą.

Instalując i uruchamiając aplikację **Simple CGM 2009 Edycja Szkolna** wyrażasz zgodę na jej używanie wyłącznie na własne ryzyko oraz akceptujesz warunki <a href="LICENSE.md">Licencji</a>.


W razie problemów z działaniem aplikacji lub pytań, proszę o wysłanie mi wiadomości email na adres <a href="mailto:simple.cgm.2009@gmail.com" title="simple.cgm.2009@gmail.com">simple.cgm.2009@gmail.com</a>.

Serdecznie dziękuję za wszystkie opinie i uwagi związane z działaniem i zakresem funkcjonalnym  **Simple CGM 2009 Edycja Szkolna**.


# Wygląd i funkcjonalność

![monitor](Images/Demo/monitor.jpg)
![monitor](Images/Demo/ustawienia.jpg)

Tak jak już wspominałem, **Simple CGM 2009 Edycja Szkolna** zawsze pobiera wartość ostatniego pomiaru glikemii **równocześnie z dwóch źródeł** tzn. serwisu *[Dropbox](https://www.dropbox.com/)* oraz serwisu *[Azure](https://azure.microsoft.com/pl-pl/free/)*, a następnie wyświetla ostatni pomiar glikemii ze źródła, które udostępnia w danej chwili bardzej bieżący wynik.
Zaobserwowałem, że źródło *[Dropbox](https://www.dropbox.com/)* odświeża się szybciej, niż źródło *[Azure](https://azure.microsoft.com/pl-pl/free/)*. Czasami na wynik pomiaru glikemii ze źródła *[Azure](https://azure.microsoft.com/pl-pl/free/)* trzeba czekać kilka minut. Dlatego taka funkcjonalność jest bardzo pomocna, jeżeli zależy nam na szybkim odczytaniu wartości ostatniego pomiaru glikemii, bez względu na źródło.<p/>

####Widok *Monitor* pokazuje:####

- u góry po prawej stronie ikonę oznaczającą bieżący tryb pracy aplikacji:
 - ikona 'Aparat fotograficzny' oznacza, że aplikacja pracuje w trybie **publicznym**, a wartość gilkemii pochodzi z rzeczywistego pomiaru,
 - ikona 'Dom' oznacza, że aplikacja pracuje w trybie **prywatnym**, a wartość glikemii jest generowana losowo przez aplikację w granicach normy,	
- centralnie u góry, jeden z 5 komunikatów w zależności od wartości glikemii:
 - Poziom cukru w normie
 - Poziom cukru niski
 - Poziom cukru bardzo niski
 - Poziom cukru wysoki
 - Poziom cukru bardzo wysoki
- poziom glikemii w normie wyświetlany jest w kolorze zielonym,
- poziomy glikemii poza normą wyświetlane są kolorem czerwonym,
- dodatkowo poziom glikemii bardzo niski oraz bardzo wysoki sygnalizowane są dodatkowym pulsowaniem komunikatu,
- poniżej komunikatu, jako dużą cyfrę, ostatni pomiar glikemii ze strzałkami trendów, jeżeli trendy są dostępne,
- po lewej stronie, czas wyświetlanego pomiaru np. 85 min temu, oraz zmianę w stosunku do poprzedniego wyniku,
- u dołu ekrany, znajduje się duży przycisk do odświeżania wartości pomiaru glikemii

**Simple CGM 2009 Edycja Szkolna** udostępnia 1 widok dzienny, oraz 1 widok nocny, które można wybrać w menu **_Ustawienia_** jako opcje **Dzień** (barwy jasne) oraz **Noc** (barwy ciemne).

**Simple CGM 2009 Edycja Szkolna** pozwala również określić, które źródło danych jest traktowane jako główne, a które jako pomocnicze, w menu **_Ustawienia_** jako opcje **Dropbox** oraz **Azure**.

W menu **_Ustawienia_** widać również wartości kluczy zdefiniowane w sekcji *Ustawienia aplikacji* usługi **Azure** dla poszczególnych progów glikemii:

- dolnej normy glikemii
- górnej normy glikemii
- hipoglikemii
- hiperglikemii

Powyższe wartości służą do sterowania komunikatami wyświetlanymi w widoku **Monitor**.


# Instalacja - Wstęp

Poniżej znajdziesz informacje jak skonfigurować i uruchomić **Simple CGM 2009 Edycja Szkolna** oraz wszystkie potrzebne dodatkowe usługi. Informacje te są natury technicznej i w związku z tym, mogą być trudne do zrozumienia dla osób bez doświadczenia informatycznego. Jeżeli masz problem z ich interpretacją i wdrożeniem, najlepiej zwrócić się o pomoc do zaprzyjaźnionego i zaufanego informatyka, zwłaszcza, że podczas konfiguracji usługi **_Azure_** zostaniesz poproszony o podanie i zapisanie danych z Twojej karty kredytowej.

1. Instalacja aplikacji **_Glimp_** (do skanowania sensora smartfonem) - [Instrukcja](http://nightscout.pl/freestyle-libre/glimp/)
2. Instalacja elementów **_Nightscout_** (do odczytywania pomiaru glikemii przez Internet):
 1. Instalacja konta **_GitHub_** (do udostępniania kopii *Nightscout* oraz *Simple CGM 2009 Edycja Szkolna* dla usługi *Azure*) - [Instrukcja](http://nightscout.pl/instalacja/github-konfiguracja/)<br/>
 2. Instalacja konta **_mLab_** (do przechowywania i udostępniania pomiaru glikemii) - [Instrukcja](http://nightscout.pl/instalacja/mlab-konfiguracja/)<br/>
 3. Instalacja usługi **_Azure_** (do instalacji i uruchamiania *Nightscout* oraz *Simple CGM 2009 Edycja Szkolna*) - [Instrukcja](http://nightscout.pl/instalacja/azure-konfiguracja/)
3. Tworzenie konta **_Dropbox_** (do równoległego przechowania pomiaru glikemii) - [Logowanie](https://www.dropbox.com/login)


**_Instalacja powyższych elementów może zabrać trochę czasu, ale są to elementy obowiązkowe i nie mogą być pominięte._**

# Instalacja - Simple CGM 2009 Edycja Szkolna

### Konfiguracja konta *Dropbox* ###

####1. Sprawdzenie czy *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* zapisuje wyniki skanowania na koncie *[Dropbox](https://www.dropbox.com/login)*####

 1. Zainstaluj i skonfiguruj aplikację *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* według podanych powyżej instrukcji na smartfonie z włączonym czytnikiem NFC.
 2. Zeskanuj działający sensor *[FreeStyle Libre](http://www.freestylelibre.pl/)* za pomocą smartfonu z  włączoną aplikacją *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* i aktywnym połączeniem do Internetu.
 3. Zaloguj się do konta *[Dropbox](https://www.dropbox.com/login)* i sprawdź, czy widzisz katalog: ***/home/Aplikacje/Glimp***, oraz czy znajduje się w nim plik: ***GlicemiaNightscout.csv***.
 4. Jeżeli NIE widzisz danych z *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)*, to sprawdź, czy konfiguracja *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* na smartfonie jest prawidłowa, a smartfon ma aktywne połączenie z Internetem.

Uwaga, czasami *[Dropbox](https://www.dropbox.com/login)* zapisuje pliki z aplikacji *[Glimp](http://nightscout.pl/freestyle-libre/glimp/)* w katalogu **Apps** zamiast w katalogu **Aplikacje**.

```
https://www.dropbox.com/home/aplikacje/glimp/GlicemiaNightscout.csv
lub
https://www.dropbox.com/home/apps/glimp/GlicemiaNightscout.csv
```

![dropbox1](Images/Demo/dropbox1.jpg)


####2. Pobranie *Dropbox Access Token* do późniejszego użycia w serwisie *[Azure](https://azure.microsoft.com/pl-pl/free/)*####

1. Przejdź do strony [Dropbox API Explorer download](https://dropbox.github.io/dropbox-api-v2-explorer/#files_download).
2. Kliknij przycik ***Get Token*** - token zostanie utworzony i pokazany w polu *Access Token*.
3. Wpisz do pola **_path_** ścieżkę dostępu do pliku *GlicemiaNightscout.csv* (zobacz przykład w ramce poniżej).
4. Naciśnij przycisk ***Submit Call*** i potwierdź chęć nadania uprawnień dostępu do żądanego katalogu i pliku.
5. *[Dropbox](https://www.dropbox.com/login)* powinien wyświetlić poniższy widok z klawiszem ***Download GlicemiaNightscout.csv***.

![dropbox2](Images/Demo/dropbox2.jpg)

Oznacza to, że wygenerowany token działa prawidłowo. Możesz teraz zapisać **_Dropbox Access Token_** znajdujący się w polu **_Access Token_**, tak abyś mógł potem użyć go podczas konfiguracji parametrów połączeń aplikacji w usłudze *[Azure](https://azure.microsoft.com/pl-pl/free/)*. 

Jeżeli **nie widzisz** powyższego ekranu, sprawdź czy prawidłowo wpisałeś ścieżkę dostępu w polu *path* oraz czy plik *GlicemiaNightscout.csv* znajduje się w podanym katalogu.

```
/aplikacje/glimp/GlicemiaNightscout.csv
lub
/apps/glimp/GlicemiaNightscout.csv
```

### Konfiguracja konta *[GitHub](https://github.com/)* ###

1. Zaloguj się na swoje konto [GitHub](https://github.com/).
2. Utwórz nowy **_Fork_** do repozytorium [https://github.com/woznica1970/simple-cgm-school](https://github.com/woznica1970/simple-cgm-school), postępując według [instrukcji](http://nightscout.pl/instalacja/github-konfiguracja/), punkt od 7 do 10, używając ***woznica1970/simple-cgm-school*** zamiast ***nightscout/cgm-remote-monitor***.

### Konfiguracja usługi *[Azure](https://portal.azure.com/)* ###

#### 1. Tworzenie nowej *Aplikacji Sieci Web* ####

1. Zaloguj się na swoje konto do usługi [Azure](https://portal.azure.com/).
2. Utwórz nową **_Aplikację Sieci Web_**, analogicznie jak przy tworzeniu *Aplikacji Sieci Web* dla *Nightscout* według [instrukcji](http://nightscout.pl/instalacja/azure-konfiguracja/), punkt 11. 
3. Użyj tej samej **_Subskrypcji_** co w przypadku aplikacji *Nightscout*, oraz 
4. Ten sam **_Plan/lokalizacji usługi App Service_**.
5. Nadajesz tylko nową **_Nazwę aplikacji_** oraz tworzysz nową **_Grupę zasobów_**. 
6. Możesz też przypiąć aplikację do pulpitu. 
7. Osobiście ustawiam **_App Insights_** jako wyłączone. 

Usługa *[Azure](https://portal.azure.com/)* na podstawie pola **_Nazwa aplikacji_** utworzy nowy adres **url** dla aplikacji **Simple CGM 2009 Edycja Szkolna**, który będziesz używał do uruchomiania aplikacji na smartfonie np. **_https://mojanazwaaplikacji.azurewebsites.net_**.

#### 2. Tworzenie kluczy w sekcji *Ustawienia aplikacji* ####

Utwórz poniższe klucze i ustaw odpowiednie wartości kluczy zgodnie z własnymi preferencjami, postępując według [instrukcji](http://nightscout.pl/instalacja/azure-konfiguracja/), punkt 22.

```
Secret.Key
Norm.Min
Norm.Max
Alert.Hipo
Alert.Hiper
Time.Zone
Monitor.Restrictions 
Monitor.Week.Days
Monitor.Time.Start
Monitor.Time.End
```

<span>![azureUstawienia](Images/Demo/azureUstawienia.jpg)</span>

#### 3. Konfiguracja trybu pracy aplikacji####

Aplikacja **Simple CGM 2009 Edycja Szkolna** może pracować w 2 różnych trybach: **PUBLICZNYM** lub **PRYWATNYM**

- w trybie **publicznym** aplikacja wyświetla rzeczywistą wartość pomiaru glikemii.
- w trybie **prywatnym** aplikacje wyświetla losowo generowaną wartość glikemii w przedziale normy.

```
Aplikacja wyświetla 2 różne ikony w górnym prawym rogu ekranu w widoku 'Monitor' 
```

- w trybie **publicznym** aplikacja wyświetla ikonę **Aparat fotograficzny**
- w trybie **prywatnym** aplikacja wyświetla ikonę **Dom**

Tryby pracy aplikacji możesz ustawiać za pomocą odpowiednich wartości poniższych kluczy:

####_Time.Zone_####
w polskiej strefie czasowej ustawiamy zawsze wartość klucza *Time.Zone* na **_Central European Standard Time_**

####_Monitor.Restrictions_####

- aby **włączyć** tryb prywatny ustawiasz wartość klucza *Monitor.Restrictions* na **True**
- aby **wyłączyć** tryb prywatny ustawiasz wartość klucza *Monitor.Restrictions* na **False**

Ustawienie klucza *Monitor.Restrictions* na *False*, powoduje, że aplikacja będzie wyświetlała rzeczywiste wartości glikemii pomimo zdefiniowanych ograniczeń w kluczach związanych z dniami tygodni oraz godzinami.

####_Monitor.Week.Days_####

- dni tygodnia określamy za pomocą ciągu cyfr rozdzielonych znakiem **;**
- pierwsza cyfra w ciągu oznacza **Niedzielę**, a ostatnia oznacza **Sobotę**
- prawidłowo zdefiniowany klucz musi zawsze zawierać **7 cyfr**, nie mniej i nie więcej
- dzień, który ma być **całkowicie prywatny** np. sobota lub niedziela, przyjmuje wartość: **0**
- dzień, który ma być **częściowo publiczny** np. dzień szkolny, przyjmuje wartość: **1**

```
powyższy ciąg cyfr:
0;1;1;1;1;1;0 
oznacza:
- tryb całkowicie prywatny w niedzielę i sobotę, 
- oraz tryb częściowo publiczny w pozostałe dni tygodnia
```

####_Monitor.Time.Start_####

- ustawiasz godzinę, od której aplikacja będzie pracować w **trybie publicznym**
- czas podajesz w formacie **HH:mm:ss** np. 07:30:00 oznacza godz. 7:30 rano

####_Monitor.Time.End_####

- ustawiasz godzinę, do której aplikacja będzie pracować w **trybie publicznym**
- czas podajesz w formacie **HH:mm:ss** np. 15:30:00 oznacza godz. 3:30 po południu


#### 4. Tworzenie kluczy w sekcji *Parametry połączeń* ####

Utwórz poniższe klucze i ustaw odpowiednie wartości kluczy zgodnie z danymi z konta *[mLab](Https://mlab.com/welcome/)* oraz konta [DropBox](https://dropbox.github.io/dropbox-api-v2-explorer/#files_download).

```
Mongo.Connection.String
Mongo.Database
Mongo.Collection
Dropbox.Access.Token
Dropbox.File.Path
```

<span>![azurePolaczenia](Images/Demo/azurePolaczenia.jpg)</span>

Przykładowe wartości kluczy:

```
Mongo.Connection.String : mongodb://użytkownik:hasło@ds046939.mlab.com:46573/mojabazadanych
Mongo.Database : mojabazadanych
Mongo.Collection : mojakolekcja
Dropbox.Access.Token : QY-8ABIbye4JKJADUAyziFqDMVBHpE2S2Jb793PoM0mz287sdaiuashd&Iy0jMSRT2
Dropbox.File.Path : /aplikacje/Glimp/GlicemiaNightscout.csv
```

#### 5. Konfiguracja *Opcji wdrożenia* ####

1. Postępuj zgodnie z [instrukcją](http://nightscout.pl/instalacja/azure-konfiguracja/), punkt od 30 do 40.
2. Pamiętaj, aby podać swoje dane logowania do konta **_GitHub_** oraz wybrać odpowiedni *Projekt*: **simple-cgm-school** oraz *Rozgałęzienie*: **Master**

### Uruchomienie *Simple CGM 2009 Edycja Szkolna* na smartfonie ###

1. Wpisz **adres url** np. **_https://mojanazwaaplikacji.azurewebsites.net_**  w dowolnej przeglądarce internetowej zainstalowanej na Twoim urządzeniu.
2. Adres url znajdziesz na swoim koncie w usłudze *[Azure](https://portal.azure.com/)*.
3. Jeżeli aplikacja **Simple CGM 2009 Edycja Szkolna** została prawidłowo zainstalowana w usłudze *[Azure](https://portal.azure.com/)* to teraz powinna zostać wyświetlona strona startowa.
4. Kliknij u dołu ekranu na menu **_Ustawienia_**.
4. Wpisz w polu **_Secret Key_** to samo hasło, które ustawiłeś w wartości klucza *Secret.Key* w sekcji *Ustawienia aplikacji* podczas instalacji i konfiguracji **Simple CGM 2009 Edycja Szkolna** w usłudze *[Azure](https://portal.azure.com/)*  .
5. Następnie kliknij kolejno przyciski **_Zapisz_**, **_Monitor_**.

![ustawienia](Images/Demo/ustawienia.jpg)
![monitor](Images/Demo/monitor.jpg)

Jeżeli proces instalacji przebiegł prawidłowo, to powinieneś teraz zobaczyć na ekranie wartość glikemii z ostatniego skanowania oraz wykres liniowy. Jeżeli coś poszło nie tak, aplikacja wyświetli odpowiedni komunikat błędu.

W ramce poniżej znajdują się możliwe komunikaty błędów. W przypadku ich wystąpienia należy sprawdzić klucze i ich wartości w sekcji **Parametry połączeń** oraz w sekcji **Ustawienia aplikacji** usługi *[Azure](https://portal.azure.com/)*:

```
(MongoDB) Brak parametru połączenia -> brak jednego z kluczy Mongo.*, lub błąd w nazwie klucza
(MongoDB) Brak danych w kolekcji -> błędna wartość klucza Mongo.Collection
(MongoDB) Nieudane połączenie z bazą -> błędna wartość klucza Mongo.Connection.String
(MongoDB) Błędna nazwa serwera -> błędna wartość klucza Mongo.Connection.String
(MongoDB) Błędna nazwa bazy danych -> błędna wartość klucza Mongo.Connection.String lub Mongo.Database
(MongoDB) Niepoprawny format danych -> problem z bazą mLab. Napisz do mnie wiadomość email
(MongoDB) Niepoprawny secret key -> porównaj wartość klucza Secret.Key z hasłem użytym na smartfonie

(Dropbox) Brak parametru połączenia -> brak jednego z kluczy Dropbox.*, lub błąd w nazwie klucza
(Dropbox) Unieważniony access token -> błędna wartość klucza Dropbox.Access.Token
(Dropbox) Nie znaleziono pliku danych -> zobacz punktu 'Przejdź do strony Dropbox API Explorer download'
(Dropbox) Błędne żądanie -> napisz do mnie wiadomość email 
(Dropbox) Wystąpił nieznany błąd -> napisz do mnie wiadomość email 
(Dropbox) Niepoprawny access token -> błędna wartość klucza Dropbox.Access.Token
(Dropbox) Niepoprawny secret key -> porównaj wartość klucza Secret.Key z hasłem użytym na smartfonie
```

Jeżeli znajdziesz w powyższym opisie jakieś błędy lub nieścisłości, dziękuję za przesłanie wiadomości na <a href="mailto:simple.cgm.2009@gmail.com" title="Mariusz Woźnica">ten adres email</a>.

Dziękuję i pozdrawiam,</br>
<a href="mailto:simple.cgm.2009@gmail.com" title="Mariusz Woźnica">Mariusz Woźnica</a>