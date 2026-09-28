# Personvernerklæring for GeoSweeper

**Gjelder fra:** 26. september 2026

**Sist oppdatert:** 26. september 2026

## Kortversjonen

GeoSweeper samler ikke inn, overfører, selger eller deler noen personopplysninger. Hvert
brett du spiller, hver innstilling du velger, og hvert land du har klart, lagres kun på din
enhet. Ingenting lastes opp til oss, og det finnes ingen konto å opprette i det hele tatt.
Den eneste nettverkstrafikken GeoSweeper noensinne genererer, er StoreKit som snakker med
Apple når du gjør eller gjenoppretter et kjøp, samt sider du bevisst åpner via en lenke i
appen (dette nettstedet, eller Apples egne juridiske sider) — begge er beskrevet nedenfor, og
ingen av dem bringer med seg noe annet.

## Hvem vi er

GeoSweeper er utviklet av Ivan Cayabyab. Spørsmål om denne erklæringen eller appen kan sendes
til ivnsjdev@gmail.com.

## Hva appen lagrer, og hvor

Alt nedenfor finnes kun på din enhet, på ett av tre steder: `UserDefaults` (små
innstillingsverdier), en JSON-fil i appens egen Application Support-mappe, eller en lokal
SQLite-database.

| Hva | Primær lagring | Sendes automatisk til oss? |
|---|---|---|
| Visningsinnstillinger — bretttema, nyonfarge, eksplosjonseffekt, smellyd, kartprojeksjon (Globe eller Flat), lyd og haptikk på/av | `UserDefaults` | Nei |
| Språk du har valgt i appen | `UserDefaults` | Nei |
| Bokføring av vurderingspåminnelser — datoene GeoSweeper har bedt iOS vise den innebygde vurderingsboksen, og hvilken milepæl som utløste den siste | `UserDefaults` | Nei |
| Rekord per land — seire, tap, beste tid, og når du låste det opp, for hvert land du har spilt | En JSON-fil (`progress.json`) i appens Application Support-mappe | Nei |
| Infinite Tower-fremgang — raden du har nådd, din lagrede visning, og hvilke rader du har klart | En lokal SQLite-database | Nei |

Ingenting av dette overføres, selges eller deles med noen, heller ikke med oss. StoreKits
egen trafikk (nedenfor) og de eksterne lenkene du trykker på (også nedenfor) bringer ikke med
seg noe av dette. En iOS-enhetsbackup kan inneholde disse filene som en del av å sikkerhetskopiere
hele appen — den sikkerhetskopien igangsettes av deg eller av iOS, aldri av GeoSweeper, og den
havner der du sender den (iCloud eller datamaskinen din), ikke hos oss.

## Ingen konto, ingen innlogging, ingen sky

GeoSweeper ber aldri om et navn, en e-postadresse, et telefonnummer, en fødselsdato eller
annen identifiserende informasjon — det finnes ingenting å logge inn med, fordi det ikke
finnes noen konto. Fremgangen din synkroniseres ikke via iCloud, CloudKit eller noen annen
tjeneste: den finnes kun på enheten du spiller på. Spill det samme landet på en annen enhet,
og det starter på nytt der, fordi det ikke finnes noen serverkopi noe sted å synkronisere fra.

## Ting som bevisst ikke lagres

Brettet du holder på med — hver rute du har åpnet, hvert flagg du har plassert — finnes bare
i minnet mens du spiller. Lukk appen midt i et spill, og det brettet er borte; det skrives
aldri til disk, og det finnes ingen autolagringsfunksjon å gjenoppta et ufullført brett fra.
Bare et *avsluttet* spill (en seier eller et tap) oppdaterer rekorden per land som er
beskrevet ovenfor.

## Det ene som høres ut som det ikke er lokalt

Kartet åpner på ditt eget land første gang du starter appen. Dette kommer fra enhetens
**regioninnstilling** (landet knyttet til språket og lokaliteten din, den samme som iOS
bruker til å velge tastatur og kalender) — ikke fra GPS, Wi-Fi eller noen annen form for
posisjonssporing. GeoSweeper ber ikke om posisjonstilgang og kunne ikke lest koordinatene
dine selv om appen ønsket det.

## Tillatelser

GeoSweeper ber ikke om systemtillatelser i det hele tatt. Den ber aldri om kamera,
fotobibliotek, mikrofon, posisjon, kontakter, kalender, helsedata, bevegelsesdata eller
push-varsler, og ingen tillatelsesboks av noe slag vil noensinne vises. Dette stemmer
nøyaktig med appens `Info.plist`: det finnes ikke en eneste bruksbeskrivelse i den.

## Kjøp

GeoSweeper er gratis å laste ned. De første 10 landene dine — hvilket nivå som helst,
Beginner inkludert — er gratis å spille, og når du først har spilt et land, forblir det
spillbart for godt, selv etter at den gratis prøveperioden er brukt opp. Infinite Tower er
gratis opp til rad 10. Utover disse to punktene finnes det to uavhengige kjøp, begge
engangskjøp, ikke-forbrukbare, og tilbys gjennom Apples StoreKit og behandles utelukkende av
Apple:

- **All Countries** — et engangskjøp, ikke-forbrukbart, som permanent låser opp
  Intermediate-, Expert- og Mega-nivåene for alle 204 land. Ingenting av dette fornyes.
- **Infinite Tower Lifetime** — et engangskjøp, ikke-forbrukbart, som permanent låser opp
  muligheten til å klatre forbi rad 10. Heller ikke dette fornyes, og GeoSweeper tilbyr ikke
  noe abonnement av noe slag.

Apple, ikke GeoSweeper, behandler hver betaling. Ingen kortnummer, fakturaadresse eller
Apple-kontoopplysning er noensinne synlig for oss — StoreKit forteller appen bare det den
trenger for å vise en betalingsmur og gi tilgang: prisen som skal vises, og om du allerede
eier hvert element. De svarene blir på din enhet; GeoSweeper driver ingen egen kjøpsserver og
har ingen steder å sende dem. Å gjenopprette kjøp ber Apple bekrefte på nytt hva
Apple-kontoen din eier, og bruker svaret lokalt — det oppretter eller overfører ingen ny post.

Se også Apples [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/),
[Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) og
[Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), som
regulerer selve kjøpet.

## Supportkommunikasjon

Hvis du sender e-post til ivnsjdev@gmail.com, mottar vi e-postadressen din, det du skriver,
og eventuelle vedlegg du velger å legge ved. Vi bruker det kun til å svare deg og løse
problemet du skrev om — vårt rettslige grunnlag er vår berettigede interesse i å svare folk
som kontakter oss. Den postboksen er en vanlig Gmail-konto, behandlet av Google LLC i henhold
til [Googles personvernerklæring](https://policies.google.com/privacy), og driftet på
infrastruktur som kan ligge utenfor ditt eget land, som er grunnen til at denne overføringen
er oppgitt her. Vi lagrer support-e-poster i opptil 24 måneder og sletter dem deretter; du kan
når som helst be oss slette en bestemt e-post tidligere ved å skrive til samme adresse.

## Eksterne lenker

GeoSweepers betalingsmurer lenker til dette nettstedets egen personvernerklæring og til
Apples Standard EULA; Settings kan lenke til App Stores side for å skrive en anmeldelse.
Ingen brukerdata eller appspesifikk identifikator legges ved noen av disse lenkene — de er
vanlige nettadresser, de samme for alle.

## Ingenting å satse

GeoSweeper har ingen spillvaluta, ingen loot, ingen premietrekninger og ingen funksjon der et
utfall satses eller veddes om. Hvert kjøp er en fast, oppgitt pris for permanent eller
tidsbegrenset tilgang til innhold; ingenting kan vinnes, tapes eller spilles bort.

## Det vi IKKE gjør

- Ingen analyse, krasjrapportering eller telemetri av noe slag
- Ingen reklame, ingen annonsenettverk og ingen reklameidentifikatorer
- Ingen sporing på tvers av apper eller nettsteder, og ingen datameglere
- Ingen kontoer, ingen innlogging, ingen passord
- Ikke noe kamera, fotobibliotek, mikrofon, kontakter, presis eller omtrentlig posisjon, eller
  helsedata
- Ingen trening av maskinlæringsmodeller på dataene dine
- Ingen tredjeparts-SDK-er av noe slag — den eneste koden i denne appen er vår egen

Dette stemmer med "Data Not Collected"-merket (data samles ikke inn) som GeoSweeper har på
App Store.

## Oppbevaring og sletting

Å slette appen sletter hver fil den har lagret på enheten din — innstillinger, rekorden din
per land og Infinite Tower-fremgangen din — umiddelbart og fullstendig, fordi det aldri fantes
en serverkopi for oss å beholde eller slette på vår side. En iCloud-enhetsbackup som ble tatt
før slettingen, kan fortsatt inneholde en kopi; den sikkerhetskopien er helt under din kontroll
via **Settings → navnet ditt → iCloud → Administrer kontolagring** på enheten din. Support-
e-poster oppbevares og slettes separat, som beskrevet ovenfor.

## Dine rettigheter

Fordi GeoSweeper ikke beholder noen kopi av dataene dine i appen, er rettighetene til tilgang,
retting, eksport og sletting som GDPR, UK GDPR og CCPA/CPRA beskriver, noe du allerede utøver
direkte, på din egen enhet — det finnes ingen registrering her som vi kan fremlegge eller
slette på dine vegne. Det eneste stedet vi faktisk oppbevarer noe, er en support-e-post du har
sendt oss, og du kan når som helst be om å se, rette eller slette den ved å skrive til
ivnsjdev@gmail.com. Vi selger eller deler ikke personopplysninger for atferdsbasert
annonsering på tvers av kontekster, og har aldri gjort det. Hvis du mener vi har håndtert
dataene dine feil, har du rett til å klage til din lokale datatilsynsmyndighet.

## Barn

GeoSweeper har en aldersgrense som passer for et generelt publikum, og er ikke spesifikt
rettet mot barn. Vi samler ikke bevisst inn personopplysninger fra noen, inkludert barn under
13 år, og det finnes ingenting i appen som kunne gjort det — ingen chat, ingen deling, ingen
sosial funksjon, ingen reklame, og ingen konto for en tredjepart å nå et barn gjennom.

## Endringer i denne erklæringen

Hvis denne erklæringen endres, endres datoen øverst med den, og en vesentlig endring i hva
GeoSweeper gjør med data vil også bli nevnt i den oppdateringens versjonsnotater.

## Kontakt

ivnsjdev@gmail.com
