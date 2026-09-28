# Privatlivspolitik for GeoSweeper

**Gældende fra:** 26. september 2026

**Sidst opdateret:** 26. september 2026

## Den korte version

GeoSweeper indsamler, videresender, sælger eller deler ikke nogen personoplysninger. Hvert
bræt du spiller, hver indstilling du vælger, og hvert land du har klaret, gemmes udelukkende
på din enhed. Intet uploades til os, og der er slet ikke nogen konto at oprette. Den eneste
netværkstrafik, GeoSweeper nogensinde genererer, er StoreKit, der taler med Apple, når du
foretager eller gendanner et køb, samt sider du bevidst åbner via et link i appen (dette
websted eller Apples egne juridiske sider) — begge er beskrevet nedenfor, og ingen af dem
medbringer noget andet.

## Hvem vi er

GeoSweeper er udviklet af Ivan Cayabyab. Spørgsmål om denne politik eller appen kan sendes
til ivnsjdev@gmail.com.

## Hvad appen gemmer, og hvor

Alt nedenfor findes udelukkende på din enhed, ét af tre steder: `UserDefaults` (små
indstillingsværdier), en JSON-fil i appens egen Application Support-mappe, eller en lokal
SQLite-database.

| Hvad | Primær lagring | Sendes automatisk til os? |
|---|---|---|
| Visningsindstillinger — brættema, neonfarve, eksplosionseffekt, smældlyd, kortprojektion (Globe eller Flat), lyd og haptik til/fra | `UserDefaults` | Nej |
| Sprog du har valgt i appen | `UserDefaults` | Nej |
| Bogføring af vurderingspåmindelser — datoerne hvor GeoSweeper har bedt iOS vise den indbyggede vurderingsboks, og hvilken milepæl der udløste den seneste | `UserDefaults` | Nej |
| Rekord pr. land — sejre, nederlag, bedste tid, og hvornår du låste det op, for hvert land du har spillet | En JSON-fil (`progress.json`) i appens Application Support-mappe | Nej |
| Infinite Tower-fremskridt — den række du har nået, din gemte visning, og hvilke rækker du har klaret | En lokal SQLite-database | Nej |

Intet af dette overføres, sælges eller deles med nogen, heller ikke med os. StoreKits egen
trafik (nedenfor) og de eksterne links du trykker på (også nedenfor) medbringer intet af
dette. En iOS-enhedsbackup kan indeholde disse filer som en del af at sikkerhedskopiere hele
appen — den backup igangsættes af dig eller af iOS, aldrig af GeoSweeper, og den ender der,
hvor du sender den hen (iCloud eller din computer), ikke hos os.

## Ingen konto, ingen login, ingen sky

GeoSweeper beder aldrig om et navn, en e-mailadresse, et telefonnummer, en fødselsdato eller
andre identificerende oplysninger — der er intet at logge ind med, fordi der ikke er nogen
konto. Dine fremskridt synkroniseres ikke via iCloud, CloudKit eller nogen anden tjeneste: de
findes udelukkende på den enhed, du spiller på. Spil det samme land på en anden enhed, og det
starter forfra der, fordi der ikke findes nogen serverkopi noget sted at synkronisere fra.

## Ting der bevidst ikke gemmes

Brættet du er midt i — hver flise du har åbnet, hvert flag du har placeret — findes kun i
hukommelsen, mens du spiller. Luk appen midt i et spil, og det bræt er væk; det skrives
aldrig til disken, og der er ingen autogem-funktion at genoptage et ufærdigt bræt fra. Kun et
*afsluttet* spil (en sejr eller et nederlag) opdaterer rekorden pr. land, der er beskrevet
ovenfor.

## Det ene, der lyder som om det ikke er lokalt

Kortet åbner på dit eget land, første gang du starter appen. Det kommer fra din enheds
**regionsindstilling** (landet knyttet til dit sprog og din lokalitet, den samme som iOS
bruger til at vælge et tastatur og en kalender) — ikke fra GPS, Wi-Fi eller nogen anden form
for lokationssporing. GeoSweeper anmoder ikke om adgang til placering og kunne ikke aflæse
dine koordinater, selv hvis appen ønskede det.

## Tilladelser

GeoSweeper anmoder slet ikke om systemtilladelser. Den beder aldrig om kameraet,
fotobiblioteket, mikrofonen, placering, kontakter, kalender, sundhedsdata, bevægelsesdata
eller push-notifikationer, og der vises aldrig nogen tilladelsesboks af nogen art. Dette
stemmer nøjagtigt overens med appens `Info.plist`: der er ikke et eneste
anvendelsesbeskrivelses-punkt i den.

## Køb

GeoSweeper er gratis at downloade. Dine første 10 lande — uanset niveau, Beginner inklusive —
er gratis at spille, og når du først har spillet et land, forbliver det spilbart for evigt,
også efter at den gratis prøveperiode er brugt op. Infinite Tower er gratis op til række 10.
Ud over disse to punkter er der to uafhængige køb, begge engangskøb, ikke-forbrugbare, og
udbudt gennem Apples StoreKit og behandlet udelukkende af Apple:

- **All Countries** — et engangskøb, ikke-forbrugbart, der permanent låser Intermediate-,
  Expert- og Mega-niveauerne op for alle 204 lande. Intet af dette fornyes.
- **Infinite Tower Lifetime** — et engangskøb, ikke-forbrugbart, der permanent låser op for
  at klatre forbi række 10. Heller ikke dette fornyes, og GeoSweeper tilbyder intet abonnement
  af nogen art.

Apple, ikke GeoSweeper, behandler enhver betaling. Intet kortnummer, ingen faktureringsadresse
eller Apple-kontooplysning er nogensinde synlig for os — StoreKit fortæller kun appen, hvad
den behøver for at vise en betalingsmur og give adgang: prisen der skal vises, og om du
allerede ejer hvert element. De svar bliver på din enhed; GeoSweeper driver ikke sin egen
købsserver og har ingen steder at sende dem hen. At gendanne køb beder Apple om at bekræfte
igen, hvad din Apple-konto ejer, og anvender svaret lokalt — det opretter eller overfører
ingen ny registrering.

Se også Apples [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/),
[Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) og
[Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), som
regulerer selve købet.

## Support-kommunikation

Hvis du sender en e-mail til ivnsjdev@gmail.com, modtager vi din e-mailadresse, det du
skriver, og enhver vedhæftet fil, du vælger at tilføje. Vi bruger det udelukkende til at
svare dig og løse det problem, du skrev om — vores retlige grundlag er vores legitime
interesse i at svare folk, der kontakter os. Den postkasse er en almindelig Gmail-konto,
behandlet af Google LLC i henhold til
[Googles privatlivspolitik](https://policies.google.com/privacy), og hostet på infrastruktur,
der kan befinde sig uden for dit eget land, hvilket er grunden til, at denne overførsel
oplyses her. Vi opbevarer support-e-mails i op til 24 måneder og sletter dem derefter; du kan
til enhver tid bede os om at slette en bestemt e-mail før da ved at skrive til samme adresse.

## Eksterne links

GeoSweepers betalingsmure linker til dette websteds egen privatlivspolitik og til Apples
Standard EULA; Settings kan linke til App Stores side for at skrive en anmeldelse. Ingen
brugerdata eller appspecifik identifikator vedhæftes nogen af disse links — de er almindelige
URL'er, de samme for alle.

## Intet at satse

GeoSweeper har ingen spilvaluta, ingen loot, ingen præmietrækninger og ingen funktion, hvor
et udfald indsættes eller væddes om. Hvert køb er en fast, oplyst pris for permanent eller
tidsbegrænset adgang til indhold; intet kan vindes, tabes eller spilles væk.

## Hvad vi IKKE gør

- Ingen analyse, fejlrapportering eller telemetri af nogen art
- Ingen reklamer, ingen annnoncenetværk og ingen reklameidentifikatorer
- Ingen sporing på tværs af apps eller websteder, og ingen datamæglere
- Ingen konti, intet login, ingen adgangskoder
- Intet kamera, intet fotobibliotek, ingen mikrofon, ingen kontakter, ingen præcis eller
  omtrentlig placering, og ingen sundhedsdata
- Ingen træning af maskinlæringsmodeller på dine data
- Ingen tredjeparts-SDK'er af nogen art — den eneste kode i denne app er vores egen

Dette stemmer overens med "Data Not Collected"-mærket (data indsamles ikke), som GeoSweeper
har på App Store.

## Opbevaring og sletning

Sletning af appen sletter hver fil, den har gemt på din enhed — indstillinger, din rekord pr.
land og dine Infinite Tower-fremskridt — øjeblikkeligt og fuldstændigt, fordi der aldrig var
en serverkopi, som vi kunne beholde eller slette på vores side. En iCloud-enhedsbackup lavet
før sletningen kan stadig indeholde en kopi; den backup er helt under din kontrol via
**Settings → dit navn → iCloud → Administrer kontolagerplads** på din enhed. Support-e-mails
opbevares og slettes separat, som beskrevet ovenfor.

## Dine rettigheder

Fordi GeoSweeper ikke beholder nogen kopi af dine data i appen, er de rettigheder til adgang,
berigtigelse, eksport og sletning, som GDPR, UK GDPR og CCPA/CPRA beskriver, nogle du allerede
udøver direkte på din egen enhed — der findes ingen registrering her, som vi kan udlevere
eller slette på dine vegne. Det eneste sted, vi rent faktisk opbevarer noget, er en
support-e-mail, du har sendt os, og du kan til enhver tid bede om at se, rette eller slette
den ved at skrive til ivnsjdev@gmail.com. Vi sælger eller deler ikke personoplysninger til
adfærdsbaseret annoncering på tværs af kontekster, og det har vi aldrig gjort. Hvis du mener,
vi har håndteret dine data forkert, har du ret til at klage til din lokale
databeskyttelsesmyndighed.

## Børn

GeoSweeper har en aldersvurdering, der egner sig til et bredt publikum, og er ikke rettet
specifikt mod børn. Vi indsamler ikke bevidst personoplysninger fra nogen, herunder børn
under 13 år, og der er intet i appen, der kunne gøre det — ingen chat, ingen deling, ingen
social funktion, ingen reklame, og ingen konto, som en tredjepart kan nå et barn igennem.

## Ændringer af denne politik

Hvis denne politik ændres, ændres datoen øverst med den, og en væsentlig ændring af, hvad
GeoSweeper gør med data, vil også blive nævnt i den opdaterings udgivelsesnoter.

## Kontakt

ivnsjdev@gmail.com
