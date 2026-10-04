# Polityka prywatności dla GeoSweeper

**Data wejścia w życie:** 26 września 2026 r

**Ostatnia aktualizacja:** 4 października 2026 r

## Krótka wersja

GeoSweeper nie gromadzi, nie przekazuje, nie sprzedaje ani nie udostępnia żadnych danych osobowych. Każda plansza, na której grasz, każde wybrane ustawienie i każdy wyczyszczony kraj są przechowywane tylko na Twoim urządzeniu. Nic nie jest do nas przesyłane i nie ma w ogóle konta, które można by utworzyć. Jedyny ruch sieciowy, jaki kiedykolwiek generuje GeoSweeper, to rozmowa StoreKit z Apple podczas dokonywania lub przywracania zakupu oraz strony, które celowo otwierasz z łącza w aplikacji (ta witryna lub własne strony prawne Apple) — oba zostały omówione poniżej i żadne z nich nie wiąże się z niczym innym.

## Kim jesteśmy

GeoSweeper został opracowany przez Ivana Cayabyaba. Pytania dotyczące tych zasad lub aplikacji można przesyłać na adres ivnsjdev@gmail.com.

## Co i gdzie przechowuje aplikacja

Wszystko poniżej znajduje się tylko na Twoim urządzeniu, w jednym z trzech miejsc: „UserDefaults” (małe wartości ustawień), plik JSON w folderze Application Support aplikacji lub lokalna baza danych SQLite.

| Co | Magazyn podstawowy | Wysłane automatycznie do nas? |
|---|---|---|
| Ustawienia wyświetlania — motyw planszy, kolor neonu, efekt eksplozji, dźwięk wybuchu, projekcja mapy (kula lub płaska), włączenie/wyłączenie dźwięku i elementów dotykowych | `Ustawienia domyślne użytkownika` | Nie |
| Language wybrałeś w aplikacji | `Ustawienia domyślne użytkownika` | Nie |
| Księgowanie z podpowiedzią oceny — daty, w których GeoSweeper poprosił system iOS o wyświetlenie natywnego arkusza ocen oraz który kamień milowy spowodował wyświetlenie ostatniego | `Ustawienia domyślne użytkownika` | Nie |
| Liczniki darmowych gier — ile z Twoich 10 darmowych krajów na mapie i 10 darmowych gier Classic zostało wykorzystanych | `Ustawienia domyślne użytkownika` | Nie |
| Rekord w poszczególnych krajach — zwycięstwa, porażki, najlepszy czas i moment odblokowania, dla każdego kraju, w którym grałeś | Plik JSON („progress.json”) w folderze Application Support aplikacji | Nie |
| Historia trybu Classic — rozmiar planszy, poziom trudności, liczba min, czas oraz wygrana lub przegrana każdej ukończonej gry Classic | Plik JSON (`Classic/history.json`) w folderze Application Support aplikacji | Nie |
| Postęp Infinite Tower — osiągnięty wiersz, zapisana rzutnia i wyczyszczone wiersze | Lokalna baza danych SQLite | Nie |

Żadna z tych informacji nie jest przesyłana, sprzedawana ani udostępniana nikomu, w tym nam. Własny ruch StoreKit (poniżej) i linki zewnętrzne, na które klikasz (również poniżej), nie przenoszą żadnego z nich. Kopia zapasowa urządzenia iOS może zawierać te pliki w ramach kopii zapasowej aplikacji jako całości — ta kopia zapasowa jest inicjowana przez Ciebie lub przez iOS, a nie przez GeoSweeper i pozostaje wszędzie tam, gdzie ją wyślesz (iCloud lub Twój komputer), a nie u nas.

## Bez konta, bez logowania, bez chmury

GeoSweeper nigdy nie pyta o imię i nazwisko, adres e-mail, numer telefonu, datę urodzenia ani inne dane identyfikujące — nie ma się czym logować, bo nie ma konta. Twoje postępy nie są synchronizowane za pośrednictwem iCloud, CloudKit ani żadnej innej usługi: są dostępne tylko na urządzeniu, na którym grasz. Zagraj w ten sam kraj na drugim urządzeniu i tam wszystko zacznie się od nowa, ponieważ nie ma nigdzie kopii serwera, z której można by przeprowadzić synchronizację.

## Wszystko, co celowo nie zostało zachowane

Plansza, na której się znajdujesz – każda otwarta płytka, każda umieszczona flaga – jest przechowywana tylko w pamięci podczas gry. Dotyczy to wszystkich trzech światów: mapy, trybu Classic i Infinite Tower. Zamknij aplikację w połowie gry, a plansza zniknie; nigdy nie jest zapisywany na dysku i nie ma funkcji automatycznego zapisywania, z której można wznowić niedokończoną planszę. Tylko *dokończony* mecz (wygrana lub przegrana) aktualizuje opisany powyżej rekord w podziale na kraje lub historię trybu Classic.

## Jedna rzecz, która brzmi, jakby nie była lokalna

Mapa Twojego kraju otwiera się przy pierwszym uruchomieniu aplikacji. Pochodzi to z **ustawień regionu** Twojego urządzenia (kraju powiązanego z Twoim językiem i ustawieniami regionalnymi, tego samego, którego iOS używa do wybierania klawiatury i kalendarza), a nie z GPS, Wi-Fi lub jakiejkolwiek innej formy śledzenia lokalizacji. GeoSweeper nie żąda dostępu do lokalizacji i nie może odczytać współrzędnych, nawet gdyby chciał.

## Uprawnienia

GeoSweeper nie żąda żadnych uprawnień systemowych. Nigdy nie prosi o aparat, bibliotekę zdjęć, mikrofon, lokalizację, kontakty, kalendarz, dane dotyczące zdrowia, dane o ruchu ani powiadomienia push i nigdy nie pojawia się żaden monit o pozwolenie. Odpowiada to dokładnie plikowi „Info.plist” aplikacji: nie ma w nim ani jednego wpisu opisu użycia.

## Zakupy

GeoSweeper można pobrać bezpłatnie, a każdy z jego trzech światów ma własny bezpłatny okres próbny. Twoje pierwsze 10 krajów na mapie — dowolny poziom, w tym Beginner — jest bezpłatne, a gdy już zagrasz w dany kraj, będzie można w nim grać na stałe, nawet po zakończeniu tego okresu próbnego. Tryb Classic daje Ci w ten sam sposób 10 darmowych gier. Infinite Tower jest bezpłatny do wiersza 10. Poza tymi punktami istnieją trzy niezależne zakupy, wszystkie jednorazowe, nie podlegające zużyciu, oferowane za pośrednictwem StoreKit firmy Apple i przetwarzane w całości przez firmę Apple:

- **All Countries** — jednorazowy zakup nie nadający się do spożycia, który na stałe odblokowuje
  Poziomy Intermediate, Expert i Mega we wszystkich 204 krajach. Nic w tym nie jest odnawialne.
- **Classic Lifetime** — jednorazowy zakup nie nadający się do spożycia, który na stałe odblokowuje
  nieograniczone gry Classic po wykorzystaniu Twoich 10 darmowych. Nic w tym nie jest odnawialne.
- **Infinite Tower Lifetime** — jednorazowy zakup, który nie podlega zużyciu i który odblokowuje się na stałe
  wspinając się obok rzędu 10. Nic w tym zakresie również nie jest odnawiane, a GeoSweeper nie oferuje żadnego rodzaju subskrypcji.

Każdą płatność przetwarza Apple, a nie GeoSweeper. Żaden numer karty, adres rozliczeniowy ani dane uwierzytelniające Apple Account nie są dla nas nigdy widoczne — StoreKit informuje jedynie aplikację, czego potrzebuje, aby wyświetlić zaporę płatniczą i udzielić dostępu: cenę do wyświetlenia oraz informację, czy aktualnie posiadasz każdy przedmiot. Odpowiedzi te pozostają na Twoim urządzeniu; GeoSweeper nie prowadzi własnego serwera zakupów i nie ma dokąd ich wysyłać. Przywrócenie zakupów wymaga od Apple ponownego potwierdzenia, co posiada Twój Apple Account i zastosowania odpowiedzi lokalnie — nie tworzy ani nie przesyła żadnego nowego rekordu.

Zobacz także [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) i [Standardową umowę EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) firmy Apple, które regulują sam zakup.

## Wsparcie komunikacji

Jeśli wyślesz e-mail do ivnsjdev@gmail.com, otrzymamy Twój adres e-mail, niezależnie od tego, co napiszesz, i każdy załącznik, który zdecydujesz się dodać. Używamy ich wyłącznie w celu udzielenia Ci odpowiedzi i rozwiązania problemu, o którym napisałeś – naszą podstawą prawną jest nasz prawnie uzasadniony interes polegający na odpowiadaniu osobom, które się z nami kontaktują. Ta skrzynka pocztowa to standardowe konto Gmail, przetwarzane przez firmę Google LLC zgodnie z [Polityką prywatności Google](https://policies.google.com/privacy) i hostowane w infrastrukturze, która może znajdować się poza Twoim krajem, dlatego też ten transfer został tutaj ujawniony. Przechowujemy e-maile dotyczące pomocy technicznej przez okres do 24 miesięcy, a następnie je usuwamy; w każdej chwili możesz poprosić nas o wcześniejsze usunięcie konkretnego e-maila, pisząc na ten sam adres.

## Linki zewnętrzne

Zapory GeoSweeper zawierają łącza do polityki prywatności tej witryny i standardowej umowy EULA firmy Apple; Settings może zawierać łącze do strony z recenzją App Store. Do żadnego z tych linków nie są dołączane żadne dane użytkownika ani identyfikator aplikacji — są to zwykłe adresy URL, takie same dla wszystkich.

## Nie ma nic do stawiania

GeoSweeper nie ma waluty w aplikacji, nie ma łupów, nie ma losowań nagród ani nie ma funkcji umożliwiającej obstawianie lub obstawianie wyniku. Każdy zakup to stała, ujawniona cena za stały lub ograniczony czasowo dostęp do treści; nic nie można wygrać, przegrać ani postawić.

## Czego NIE robimy

- Żadnych analiz, raportów o awariach ani jakiejkolwiek telemetrii
- Brak reklam, brak sieci reklamowych i brak identyfikatorów reklamowych
- Brak śledzenia między aplikacjami i witrynami oraz brak brokerów danych
- Żadnych kont, żadnego logowania, żadnych haseł
- Brak aparatu, biblioteki zdjęć, mikrofonu, kontaktów, dokładnej lub przybliżonej lokalizacji ani danych zdrowotnych
- Brak uczenia modeli uczenia maszynowego na Twoich danych
- Żadnych zewnętrznych zestawów SDK — jedyny kod w tej aplikacji jest nasz własny

Odpowiada to etykiecie „Data Not Collected (dane nie są zbierane)”, którą GeoSweeper znajduje się na App Store.

## Przechowywanie i usuwanie

Usunięcie aplikacji powoduje natychmiastowe i całkowite usunięcie wszystkich plików przechowywanych na Twoim urządzeniu — ustawień, danych dotyczących poszczególnych krajów, historii trybu Classic i postępów w aplikacji Infinite Tower — ponieważ nigdy nie mieliśmy kopii serwerowej, którą moglibyśmy zatrzymać lub usunąć z naszej strony. Kopia zapasowa urządzenia iCloud wykonana przed usunięciem może nadal zawierać kopię; ta kopia zapasowa jest całkowicie pod Twoją kontrolą poprzez **Settings → Twoje imię i nazwisko → iCloud → Zarządzaj przechowywaniem konta** na Twoim urządzeniu. E-maile dotyczące pomocy technicznej są przechowywane i usuwane osobno, jak opisano powyżej.

## Twoje prawa

Ponieważ GeoSweeper nie przechowuje kopii Twoich danych w aplikacji, prawa dostępu, poprawiania, eksportowania i usuwania opisane w RODO, brytyjskim RODO i CCPA/CPRA to te, z których korzystasz już bezpośrednio na swoim własnym urządzeniu — nie ma tu żadnych zapisów, które moglibyśmy sporządzić lub usunąć w Twoim imieniu. Jedyne miejsce, w którym coś przechowujemy, to e-mail pomocy technicznej, który nam wysłałeś. Możesz poprosić o jego przejrzenie, poprawienie lub usunięcie w dowolnym momencie, pisząc na adres ivnsjdev@gmail.com. Nie sprzedajemy ani nie udostępniamy danych osobowych na potrzeby wielokontekstowej reklamy behawioralnej i nigdy tego nie robiliśmy. Jeśli uważasz, że źle obchodziliśmy się z Twoimi danymi, masz prawo złożyć skargę do lokalnego organu ochrony danych.

## Dzieci

GeoSweeper ma klasyfikację wiekową odpowiednią dla ogółu odbiorców i nie jest skierowany specjalnie do dzieci. Nie zbieramy świadomie danych osobowych od nikogo, w tym od dzieci poniżej 13 roku życia, a w aplikacji nie ma niczego, co mogłoby to zrobić – czatu, udostępniania, funkcji społecznościowych, reklam i konta, za pośrednictwem którego osoba trzecia mogłaby skontaktować się z dzieckiem.

## Zmiany w tej polityce

Jeśli ta polityka ulegnie zmianie, data u góry zmieni się wraz z nią, a istotna zmiana w sposobie, w jaki GeoSweeper robi z danymi, zostanie również odnotowana w uwagach do wydania tej aktualizacji.

## Kontakt

ivnsjdev@gmail.com
