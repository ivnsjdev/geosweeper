# Integritetspolicy för GeoSweeper

**Gäller från:** 26 september 2026

**Senast uppdaterad:** 4 oktober 2026

## Kortversionen

GeoSweeper samlar inte in, överför, säljer eller delar någon personlig information. Varje
bräde du spelar, varje inställning du väljer och varje land du har klarat lagras enbart på
din enhet. Ingenting laddas upp till oss, och det finns inget konto att skapa över huvud
taget. Den enda nätverkstrafik GeoSweeper någonsin genererar är StoreKit som pratar med Apple
när du gör eller återställer ett köp, samt sidor du medvetet öppnar via en länk i appen
(den här webbplatsen, eller Apples egna juridiska sidor) — båda beskrivs nedan, och ingen av
dem för med sig något annat.

## Vilka vi är

GeoSweeper utvecklas av Ivan Cayabyab. Frågor om denna policy eller appen kan skickas till
ivnsjdev@gmail.com.

## Vad appen lagrar, och var

Allt nedan finns enbart på din enhet, på ett av tre ställen: `UserDefaults` (små
inställningsvärden), en JSON-fil i appens egen Application Support-mapp, eller en lokal
SQLite-databas.

| Vad | Primär lagring | Skickas automatiskt till oss? |
|---|---|---|
| Visningsinställningar — brädtema, neonfärg, explosionseffekt, smällljud, kartprojektion (Globe eller Flat), ljud och haptik på/av | `UserDefaults` | Nej |
| Språk du har valt i appen | `UserDefaults` | Nej |
| Bokföring för betygspåminnelser — datumen då GeoSweeper har bett iOS visa den inbyggda betygsrutan, och vilken milstolpe som utlöste den senaste | `UserDefaults` | Nej |
| Räknare för gratisspel — hur många av dina 10 gratis kartländer och 10 gratis Classic-spel du har använt | `UserDefaults` | Nej |
| Rekord per land — vinster, förluster, bästa tid, och när du låste upp det, för varje land du har spelat | En JSON-fil (`progress.json`) i appens Application Support-mapp | Nej |
| Classic-lägeshistorik — brädstorlek, svårighetsgrad, minantal, tid, och vinst eller förlust för varje avslutat Classic-spel | En JSON-fil (`Classic/history.json`) i appens Application Support-mapp | Nej |
| Infinite Tower-framsteg — raden du har nått, din sparade vy, och vilka rader du har klarat | En lokal SQLite-databas | Nej |

Inget av detta överförs, säljs eller delas med någon, inte heller med oss. StoreKits egen
trafik (nedan) och de externa länkar du trycker på (även dessa nedan) för inte med sig något
av detta. En säkerhetskopia av iOS-enheten kan innehålla dessa filer som en del av att hela
appen säkerhetskopieras — den säkerhetskopian initieras av dig eller av iOS, aldrig av
GeoSweeper, och den hamnar där du skickar den (iCloud eller din dator), inte hos oss.

## Inget konto, ingen inloggning, inget moln

GeoSweeper ber aldrig om ett namn, en e-postadress, ett telefonnummer, ett födelsedatum
eller någon annan identifierande information — det finns inget att logga in med, eftersom
det inte finns något konto. Dina framsteg synkroniseras inte via iCloud, CloudKit eller
någon annan tjänst: de finns enbart på enheten du spelar på. Spela samma land på en annan
enhet, och det börjar om där, eftersom det inte finns någon serverkopia någonstans att
synkronisera från.

## Sådant som medvetet inte sparas

Brädet du håller på med — varje ruta du har öppnat, varje flagga du har placerat — finns
bara i minnet medan du spelar. Detta gäller i alla tre världarna: kartan, Classic-läget och
Infinite Tower. Stäng appen mitt i ett spel och det brädet är borta; det skrivs aldrig till
disk, och det finns ingen autosparfunktion att återuppta ett oavslutat bräde från. Bara ett
*avslutat* spel (en vinst eller en förlust) uppdaterar rekordet per land eller
Classic-historiken som beskrivs ovan.

## Det enda som låter som det inte är lokalt

Kartan öppnas på ditt eget land första gången du startar appen. Det kommer från enhetens
**regioninställning** (landet kopplat till ditt språk och din lokal, samma som iOS använder
för att välja tangentbord och kalender) — inte från GPS, Wi-Fi eller någon annan form av
platsspårning. GeoSweeper begär ingen platsåtkomst och skulle inte kunna läsa dina
koordinater ens om appen ville.

## Behörigheter

GeoSweeper begär inga systembehörigheter alls. Appen ber aldrig om kameran, fotobiblioteket,
mikrofonen, plats, kontakter, kalender, hälsodata, rörelsedata eller push-notiser, och ingen
behörighetsruta av något slag kommer någonsin att visas. Detta stämmer exakt med appens
`Info.plist`: det finns inte en enda användningsbeskrivning i den.

## Köp

GeoSweeper är gratis att ladda ner, och var och en av dess tre världar har sin egen gratis
provperiod. Dina första 10 länder på kartan — vilken nivå som helst, Beginner inräknat — är
gratis att spela, och när du väl har spelat ett land förblir det spelbart för gott, även
efter att den provperioden är förbrukad. Classic-läget ger dig 10 gratis spel på samma sätt.
Infinite Tower är gratis upp till rad 10. Utöver dessa gränser finns det tre oberoende köp,
alla engångsköp, icke-förbrukningsbara, och erbjuds genom Apples StoreKit och hanteras helt
av Apple:

- **All Countries** — ett engångsköp, icke-förbrukningsbart, som permanent låser upp
  nivåerna Intermediate, Expert och Mega för alla 204 länder. Inget av detta förnyas.
- **Classic Lifetime** — ett engångsköp, icke-förbrukningsbart, som permanent låser upp
  obegränsade Classic-spel när dina 10 gratis är förbrukade. Inget av detta förnyas.
- **Infinite Tower Lifetime** — ett engångsköp, icke-förbrukningsbart, som permanent låser
  upp möjligheten att klättra förbi rad 10. Inte heller detta förnyas, och GeoSweeper
  erbjuder ingen prenumeration av något slag.

Apple, inte GeoSweeper, hanterar varje betalning. Inget kortnummer, ingen faktureringsadress
eller Apple-kontouppgift är någonsin synlig för oss — StoreKit talar bara om för appen vad
den behöver för att visa en betalvägg och ge åtkomst: priset som ska visas, och om du redan
äger varje artikel. De svaren stannar på din enhet; GeoSweeper driver ingen egen köpserver
och har ingenstans att skicka dem. Att återställa köp ber Apple bekräfta igen vad ditt
Apple-konto äger och tillämpar svaret lokalt — det skapar eller överför ingen ny post.

Se även Apples [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/),
[Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) och
[Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), som
reglerar själva köpet.

## Supportkommunikation

Om du mejlar ivnsjdev@gmail.com tar vi emot din e-postadress, det du skriver, och eventuella
bilagor du väljer att lägga till. Vi använder det bara för att svara dig och åtgärda
problemet du skrev om — vår rättsliga grund är vårt berättigade intresse av att svara
personer som kontaktar oss. Den brevlådan är ett vanligt Gmail-konto, hanterat av Google LLC
enligt [Googles integritetspolicy](https://policies.google.com/privacy), och hostat på
infrastruktur som kan vara belägen utanför ditt eget land, vilket är varför den överföringen
anges här. Vi sparar supportmejl i upp till 24 månader och raderar dem sedan; du kan när som
helst be oss radera ett specifikt mejl tidigare genom att skriva till samma adress.

## Externa länkar

GeoSweepers betalväggar länkar till den här webbplatsens egen integritetspolicy och till
Apples Standard EULA; Settings kan länka till App Stores sida för att skriva en recension.
Ingen användardata eller appspecifik identifierare bifogas någon av dessa länkar — de är
vanliga webbadresser, samma för alla.

## Inget att satsa

GeoSweeper har ingen spelvaluta, inga lootlådor, inga prisdragningar och ingen funktion där
ett utfall satsas eller vadslås om. Varje köp är ett fast, angivet pris för permanent eller
tidsbegränsad åtkomst till innehåll; ingenting kan vinnas, förloras eller spelas bort.

## Det vi INTE gör

- Ingen analys, kraschrapportering eller telemetri av något slag
- Ingen reklam, inga annonsnätverk och inga reklamidentifierare
- Ingen spårning mellan appar eller webbplatser, och inga datamäklare
- Inga konton, ingen inloggning, inga lösenord
- Ingen kamera, inget fotobibliotek, ingen mikrofon, inga kontakter, ingen exakt eller
  ungefärlig plats, och ingen hälsodata
- Ingen träning av maskininlärningsmodeller på dina data
- Inga tredjeparts-SDK:er av något slag — den enda koden i appen är vår egen

Detta stämmer med etiketten "Data Not Collected" (data samlas inte in) som GeoSweeper har
på App Store.

## Bevarande och radering

Att radera appen raderar varje fil den lagrat på din enhet — inställningar, ditt rekord per
land, Classic-historiken och dina Infinite Tower-framsteg — omedelbart och fullständigt,
eftersom det aldrig fanns en serverkopia för oss att behålla eller radera på vår sida. En iCloud-säkerhetskopia
som gjorts före raderingen kan fortfarande innehålla en kopia; den säkerhetskopian står helt
under din kontroll via **Settings → ditt namn → iCloud → Hantera lagringsutrymme för
kontot** på din enhet. Supportmejl sparas och raderas separat, som beskrivits ovan.

## Dina rättigheter

Eftersom GeoSweeper inte behåller någon kopia av dina data i appen är de rättigheter till
åtkomst, rättelse, export och radering som GDPR, UK GDPR och CCPA/CPRA beskriver sådana du
redan utövar direkt, på din egen enhet — det finns ingen uppgift här som vi kan tillhandahålla
eller radera å dina vägnar. Den enda plats vi faktiskt behåller något är ett supportmejl du
har skickat oss, och du kan när som helst be att få se, rätta eller radera det genom att
skriva till ivnsjdev@gmail.com. Vi säljer eller delar inte personuppgifter för
beteendebaserad annonsering över olika sammanhang, och har aldrig gjort det. Om du anser att
vi har hanterat dina uppgifter felaktigt har du rätt att lämna in ett klagomål till din
lokala tillsynsmyndighet för dataskydd.

## Barn

GeoSweeper har en åldersgräns lämplig för en allmän publik och riktar sig inte specifikt
till barn. Vi samlar inte medvetet in personlig information från någon, inklusive barn under
13 år, och det finns inget i appen som skulle kunna göra det — ingen chatt, ingen delning,
ingen social funktion, ingen reklam, och inget konto för en tredje part att nå ett barn
genom.

## Ändringar av denna policy

Om denna policy ändras kommer datumet högst upp att ändras med den, och en väsentlig ändring
av vad GeoSweeper gör med data kommer också att noteras i den uppdateringens versionsnoteringar.

## Kontakt

ivnsjdev@gmail.com
