# Privacybeleid voor GeoSweeper

**Ingangsdatum:** 26 september 2026

**Laatst bijgewerkt:** 26 september 2026

## De korte versie

GeoSweeper verzamelt, verzendt, verkoopt of deelt geen persoonlijke informatie. Elk bord dat je speelt, elke instelling die je kiest en elk land dat je hebt gewist, wordt alleen op je apparaat opgeslagen. Er wordt niets naar ons geüpload en u hoeft in de eerste plaats geen account aan te maken. Het enige netwerkverkeer dat GeoSweeper ooit genereert, is dat StoreKit met Apple communiceert wanneer u een aankoop doet of herstelt, en pagina's die u opzettelijk opent via een link in de app (deze site of Apple's eigen juridische pagina's) - beide worden hieronder besproken en hebben op geen van beide iets anders met zich mee.

## Wie we zijn

GeoSweeper is ontwikkeld door Ivan Cayabyab. Vragen over dit beleid of de app kunt u sturen naar ivnsjdev@gmail.com.

## Wat de app opslaat, en waar

Alles hieronder bevindt zich alleen op uw apparaat, op een van de drie plaatsen: `UserDefaults` (kleine instellingswaarden), een JSON-bestand in de eigen Application Support-map van de app, of een lokale SQLite-database.

| Wat | Primaire opslag | Automatisch naar ons verzonden? |
|---|---|---|
| Weergave-instellingen — bordthema, neonkleur, explosie-effect, explosiegeluid, kaartprojectie (wereldbol of plat), geluid en haptiek aan/uit | `Gebruikersstandaard` | Nee |
| Language die je hebt gekozen in de app | `Gebruikersstandaard` | Nee |
| Boekhouden op basis van beoordelingen: de data waarop GeoSweeper iOS heeft gevraagd het eigen beoordelingsblad weer te geven, en welke mijlpaal de aanleiding was voor de laatste | `Gebruikersstandaard` | Nee |
| Record per land: overwinningen, verliezen, beste tijd en wanneer je het hebt ontgrendeld, voor elk land waar je hebt gespeeld | Een JSON-bestand (`progress.json`) in de map Application Support | Nee |
| Infinite Tower voortgang — de rij die u heeft bereikt, uw opgeslagen viewport en welke rijen u heeft gewist | Een lokale SQLite-database | Nee |

Niets hiervan wordt overgedragen, verkocht of gedeeld met wie dan ook, inclusief ons. Het eigen verkeer van StoreKit (hieronder) en de externe links waarop u tikt (ook hieronder) bevatten niets hiervan. Een back-up van een iOS-apparaat kan deze bestanden bevatten als onderdeel van de back-up van de app als geheel. Die back-up wordt door u of door iOS geïnitieerd, nooit door GeoSweeper, en blijft waar u deze ook naartoe stuurt (iCloud of uw computer), niet bij ons.

## Geen account, geen login, geen cloud

GeoSweeper vraagt nooit om een naam, e-mailadres, telefoonnummer, geboortedatum of andere identificerende informatie; er is niets om mee in te loggen, omdat er geen account is. Je voortgang wordt niet gesynchroniseerd via iCloud, CloudKit of een andere service: deze staat alleen op het apparaat waarop je speelt. Speel hetzelfde land op een tweede apparaat en het begint daar opnieuw, omdat er nergens een serverkopie is om vanaf te synchroniseren.

## Alles wat opzettelijk niet werd volgehouden

Het bord waar je middenin zit – elke tegel die je hebt geopend, elke vlag die je hebt geplaatst – wordt alleen in het geheugen bewaard terwijl je speelt. Sluit de app halverwege het spel en dat bord is weg; het wordt nooit naar schijf geschreven en er is geen automatische opslag om een ​​onvoltooid bord te hervatten. Alleen een *voltooid* spel (een overwinning of een verlies) werkt het hierboven beschreven record per land bij.

## Het enige dat klinkt alsof het niet lokaal is

De kaart wordt geopend in uw eigen land wanneer u de app voor de eerste keer start. Dit komt van de **regio-instelling** van uw apparaat (het land dat is gekoppeld aan uw taal en landinstelling, hetzelfde land dat iOS gebruikt om een ​​toetsenbord en een agenda te kiezen) – niet van GPS, Wi-Fi of enige andere vorm van locatietracking. GeoSweeper vraagt ​​geen locatietoegang en kan uw coördinaten niet lezen, ook al zou hij dat willen.

## Machtigingen

GeoSweeper vraagt geen enkele systeemmachtiging. Er wordt nooit gevraagd naar de camera, fotobibliotheek, microfoon, locatie, contacten, agenda, gezondheidsgegevens, bewegingsgegevens of pushmeldingen, en er zal nooit een toestemmingsprompt verschijnen. Dit komt exact overeen met de `Info.plist` van de app: er staat geen enkele gebruiksbeschrijving in.

## Aankopen

GeoSweeper is gratis te downloaden. Je eerste 10 landen (elk niveau, inclusief Beginner) zijn gratis om te spelen, en als je eenmaal in een land hebt gespeeld, blijft het voor altijd opnieuw speelbaar, zelfs nadat de gratis proefperiode is verstreken. Infinite Tower is gratis tot en met rij 10. Naast deze twee punten zijn er twee onafhankelijke aankopen, beide eenmalig, niet-consumeerbaar, en aangeboden via Apple's StoreKit en volledig door Apple verwerkt:

- **All Countries** — een eenmalige, niet-consumeerbare aankoop die de
  Intermediate-, Expert- en Mega-niveaus in alle 204 landen. Niets hierover wordt vernieuwd.
- **Infinite Tower Lifetime** — een eenmalige, niet-consumeerbare aankoop die permanent wordt ontgrendeld
  klimmen voorbij rij 10. Ook hierover wordt niets verlengd, en GeoSweeper biedt geen enkel abonnement.

Apple, en niet GeoSweeper, verwerkt elke betaling. Er is nooit een kaartnummer, factuuradres of Apple Account-inloggegevens voor ons zichtbaar. StoreKit vertelt de app alleen wat deze nodig heeft om een ​​betaalmuur te tonen en toegang te verlenen: de prijs die moet worden weergegeven en of u momenteel eigenaar bent van elk item. Die antwoorden blijven op uw apparaat; GeoSweeper heeft geen eigen aankoopserver en kan deze nergens naartoe sturen. Bij het herstellen van aankopen wordt Apple gevraagd opnieuw te bevestigen wat uw Apple Account bezit en het antwoord lokaal toe te passen: er worden geen nieuwe records aangemaakt of verzonden.

Zie ook Apple's [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), de [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) en de [Standaard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), die van toepassing zijn op de aankoop zelf.

## Ondersteuningscommunicatie

Als u ivnsjdev@gmail.com een e-mail stuurt, ontvangen wij uw e-mailadres, wat u ook schrijft en elke bijlage die u toevoegt. We gebruiken het alleen om u te antwoorden en om het probleem op te lossen waarover u schreef. Onze wettelijke basis is ons legitieme belang bij het reageren op mensen die contact met ons opnemen. Die mailbox is een standaard Gmail-account, verwerkt door Google LLC onder [het privacybeleid van Google](https://policies.google.com/privacy), en gehost op een infrastructuur die zich mogelijk buiten uw eigen land bevindt. Daarom wordt die overdracht hier bekendgemaakt. We bewaren ondersteunings-e-mails maximaal 24 maanden en verwijderen ze vervolgens; U kunt ons op elk moment vragen een specifieke e-mail eerder te verwijderen door naar hetzelfde adres te schrijven.

## Externe links

De betaalmuren van GeoSweeper linken naar het eigen privacybeleid van deze site en naar de standaard EULA van Apple; Settings kan linken naar de schrijf-een-recensiepagina van de App Store. Aan geen van deze links worden gebruikersgegevens of app-specifieke identificatie toegevoegd; het zijn gewone URL's, die voor iedereen hetzelfde zijn.

## Niets om te wedden

GeoSweeper heeft geen in-app-valuta, geen buit, geen prijstrekkingen en geen functie waarbij een uitkomst wordt ingezet of ingezet. Elke aankoop is een vaste, bekendgemaakte prijs voor permanente of timebox-toegang tot inhoud; niets kan worden gewonnen, verloren of gegokt.

## Wat we NIET doen

- Geen analyses, crashrapportage of enige vorm van telemetrie
- Geen advertenties, geen advertentienetwerken en geen advertentie-ID's
- Geen cross-app- of cross-site-tracking en geen datamakelaars
- Geen accounts, geen login, geen wachtwoorden
- Geen camera, fotobibliotheek, microfoon, contacten, precieze of grove locatie of gezondheidsgegevens
- Geen training van machine-learningmodellen op uw gegevens
- Geen enkele SDK van derden; de enige code in deze app is van onszelf

Dit komt overeen met het "Data Not Collected (geen gegevens verzameld)" -label dat GeoSweeper op de App Store draagt.

## Bewaren en verwijderen

Als u de app verwijdert, wordt elk bestand dat op uw apparaat is opgeslagen verwijderd – instellingen, uw gegevens per land en uw Infinite Tower-voortgang – onmiddellijk en volledig, omdat er nooit een serverkopie was die wij konden bewaren of verwijderen aan onze kant. Een back-up van een iCloud-apparaat die vóór verwijdering is gemaakt, kan nog steeds een kopie bevatten; die back-up heeft u volledig onder controle via **Settings → uw naam → iCloud → Accountopslag beheren** op uw apparaat. Ondersteunings-e-mails worden afzonderlijk bewaard en verwijderd, zoals hierboven beschreven.

## Jouw rechten

Omdat GeoSweeper geen kopie bewaart van uw in-app-gegevens, zijn de toegangs-, correctie-, export- en verwijderingsrechten die GDPR, UK GDPR en de CCPA/CPRA beschrijven de rechten die u al rechtstreeks op uw eigen apparaat uitoefent. Er is hier geen record dat wij namens u kunnen produceren of wissen. De enige plek waar we iets bewaren is een ondersteunings-e-mail die u ons hebt gestuurd. U kunt op elk gewenst moment vragen om deze in te zien, te corrigeren of te verwijderen door te schrijven naar ivnsjdev@gmail.com. We verkopen of delen geen persoonlijke informatie voor cross-context gedragsadvertenties, en dat hebben we ook nooit gedaan. Als u van mening bent dat wij uw gegevens verkeerd hebben behandeld, heeft u het recht om een ​​klacht in te dienen bij uw lokale gegevensbeschermingsautoriteit.

## Kinderen

GeoSweeper heeft een leeftijdsclassificatie die geschikt is voor een algemeen publiek en is niet specifiek gericht op kinderen. We verzamelen niet bewust persoonlijke informatie van wie dan ook, inclusief kinderen onder de 13 jaar, en er is niets in de app dat dat zou kunnen doen: geen chat, geen delen, geen sociale functie, geen reclame en geen account waarmee een derde partij een kind kan bereiken.

## Wijzigingen in dit beleid

Als dit beleid verandert, verandert de datum bovenaan mee, en een materiële verandering in wat GeoSweeper met gegevens doet, zal ook worden vermeld in de release-opmerkingen van die update.

## Contactpersoon

ivnsjdev@gmail.com
