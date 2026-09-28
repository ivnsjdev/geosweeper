# GeoSweeper:n tietosuojakäytäntö

**Voimaantulopäivä:** 26.9.2026

**Viimeksi päivitetty:** 26. syyskuuta 2026

## Lyhyt versio

GeoSweeper ei kerää, siirrä, myy tai jaa henkilökohtaisia tietoja. Jokainen pelaamasi lauta, jokainen valitsemasi asetus ja kaikki tyhjentämäsi maat tallennetaan vain laitteellesi. Meille ei ladata mitään, eikä tiliä ole alunperin luotava. Ainoa GeoSweeper:n koskaan luoma verkkoliikenne on StoreKit, joka puhuu Applelle, kun teet tai palautat ostoksen, ja sivut, jotka avaat tarkoituksella sovelluksen sisällä olevasta linkistä (tämä sivusto tai Applen omat lailliset sivut) – molemmat käsitellään alla, eikä kumpikaan sisällä mitään muuta.

## Keitä me olemme

GeoSweeper:n on kehittänyt Ivan Cayabyab. Tätä käytäntöä tai sovellusta koskevat kysymykset voidaan lähettää osoitteeseen ivnsjdev@gmail.com.

## Mitä sovellus tallentaa ja missä

Kaikki alla oleva säilyy vain laitteessasi yhdessä kolmesta paikasta: UserDefaults (pienet asetusarvot), JSON-tiedosto sovelluksen omassa Application Support -kansiossa tai paikallinen SQLite-tietokanta.

| Mitä | Ensisijainen varastointi | Lähetetäänkö meille automaattisesti? |
|---|---|---|
| Näyttöasetukset — tauluteema, neonväri, räjähdystehoste, räjähdysääni, karttaprojektio (maapallo tai tasainen), ääni ja haptiikka päälle/pois | `UserDefaults` | Ei |
| Language, jonka olet valinnut sovelluksen sisällä | `UserDefaults` | Ei |
| Luokituksen mukainen kirjanpito – päivämäärät, jotka GeoSweeper on pyytänyt iOS:ää näyttämään alkuperäisen luokitustaulukon ja mikä virstanpylväs laukaisi viimeisen | `UserDefaults` | Ei |
| Maakohtainen ennätys – voitot, tappiot, paras aika ja kun avasit sen, jokaisessa maassa, jossa olet pelannut | JSON-tiedosto (`progress.json`) sovelluksen Application Support -kansiossa | Ei |
| Infinite Tower edistyminen — rivi, jonka olet saavuttanut, tallennettu näkymä ja tyhjentämäsi rivit | Paikallinen SQLite-tietokanta | Ei |

Mitään näistä ei lähetetä, myydä tai jaeta kenenkään kanssa, mukaan lukien meille. StoreKit:n oma liikenne (alla) ja napauttamasi ulkoiset linkit (myös alla) eivät sisällä sitä. iOS-laitteen varmuuskopio voi sisältää nämä tiedostot osana koko sovelluksen varmuuskopiointia – varmuuskopioinnin aloitat sinä tai iOS, ei koskaan GeoSweeper, ja se säilyy minne tahansa lähetät sen (iCloud tai tietokoneellesi), ei meidän kanssamme.

## Ei tiliä, ei sisäänkirjautumista, ei pilvipalvelua

GeoSweeper ei koskaan kysy nimeä, sähköpostiosoitetta, puhelinnumeroa, syntymäaikaa tai muita tunnistetietoja – ei ole mitään kirjautumista, koska tiliä ei ole. Edistymistäsi ei synkronoida iCloud:n, CloudKit:n tai minkään muun palvelun kautta: se elää vain laitteessa, jolla pelaat. Toista samaa maata toisella laitteella ja se alkaa sieltä, koska synkronointia varten ei ole palvelinkopiota.

## Kaikki, mitä ei tietoisesti säilynyt

Lauta, jonka keskellä olet – jokainen avaamasi laatta, jokainen asettamasi lippu – säilyy vain muistissa pelatessasi. Sulje sovellus kesken pelin ja lauta on poissa. sitä ei koskaan kirjoiteta levylle, eikä siinä ole automaattista tallennusta keskeneräisen levyn jatkamiseksi. Vain *valmis* peli (voitto tai tappio) päivittää edellä kuvatun maakohtaisen ennätyksen.

## Yksi asia, joka kuulostaa siltä, että se ei ole paikallinen

Kartta avautuu omassa maassasi, kun käynnistät sovelluksen ensimmäisen kerran. Tämä tulee laitteesi **alueasetuksesta** (kieleesi ja alueellesi sidottu maa, jota iOS käyttää näppäimistön ja kalenterin valitsemiseen) – ei GPS:stä, Wi-Fi:stä tai muusta sijainnin seurannasta. GeoSweeper ei pyydä sijaintiin pääsyä eikä voinut lukea koordinaattejasi vaikka haluaisi.

## Luvat

GeoSweeper ei pyydä mitään järjestelmän käyttöoikeuksia. Se ei koskaan kysy kameraa, valokuvakirjastoa, mikrofonia, sijaintia, yhteystietoja, kalenteria, terveystietoja, liiketietoja tai push-ilmoituksia, eikä minkäänlaista lupakehotetta tule koskaan näkyviin. Tämä vastaa täsmälleen sovelluksen Info.plist-tiedostoa: siinä ei ole ainuttakaan käyttökuvausmerkintää.

## Ostokset

GeoSweeper on ladattavissa ilmaiseksi. Ensimmäiset 10 maatasi – mikä tahansa taso, mukaan lukien Beginner – ovat ilmaisia, ja kun olet pelannut maata, se pysyy toistettavissa lopullisesti, jopa ilmaisen kokeilujakson jälkeen. Infinite Tower on ilmainen riville 10 asti. Näiden kahden pisteen lisäksi on kaksi erillistä ostoa, molemmat kertaluonteisia, ei-kulutustuotteita, jotka tarjotaan Applen StoreKit:n kautta ja jotka Apple käsittelee kokonaan:

- **All Countries** – kertaluonteinen, ei-kuluva ostos, joka avaa pysyvästi
  Intermediate-, Expert- ja Mega-tasot kaikissa 204 maassa. Mikään tästä ei uusiudu.
- **Infinite Tower Lifetime** – kertaluonteinen, ei-kuluva ostos, joka avaa lukituksen pysyvästi
  kiipeäminen rivin 10 ohi. Tämäkään ei uusiudu, eikä GeoSweeper tarjoa minkäänlaista tilausta.

Apple, ei GeoSweeper, käsittelee jokaisen maksun. Emme koskaan näe kortin numeroa, laskutusosoitetta tai Apple Account-tunnistetietoja – StoreKit kertoo sovellukselle vain, mitä se tarvitsee maksumuurin näyttämiseksi ja käyttöoikeuden myöntämiseksi: näytettävän hinnan ja sen, omistatko tällä hetkellä kunkin tuotteen. Nämä vastaukset pysyvät laitteessasi; GeoSweeper ei käytä omaa ostopalvelinta, eikä sillä ole minnekään lähettää niitä. Ostosten palauttaminen pyytää Applea vahvistamaan uudelleen, mitä Apple Account omistaa, ja soveltaa vastausta paikallisesti – se ei luo tai lähetä uusia tietueita.

Katso myös Applen [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) ja [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), jotka säätelevät itse ostoa.

## Viestinnän tuki

Jos lähetät sähköpostia ivnsjdev@gmail.com:lle, saamme sähköpostiosoitteesi, mitä tahansa kirjoitat ja kaikki lisättävät liitteet. Käytämme sitä vain vastataksemme sinulle ja korjataksemme ongelman, josta kirjoitit – laillinen perustamme on oikeutettu etumme vastata ihmisille, jotka ottavat meihin yhteyttä. Tämä postilaatikko on tavallinen Gmail-tili, jota Google LLC käsittelee [Googlen tietosuojakäytännön](https://policies.google.com/privacy) mukaisesti ja jota isännöi infrastruktuuri, joka saattaa sijaita oman maasi ulkopuolella, minkä vuoksi tämä siirto julkaistaan ​​täällä. Säilytämme tukisähköpostit jopa 24 kuukautta ja poistamme ne sitten. voit pyytää meitä poistamaan tietyn sähköpostin aikaisemmin kirjoittamalla samaan osoitteeseen.

## Ulkoiset linkit

GeoSweeper:n maksumuurit linkittävät tämän sivuston omaan tietosuojakäytäntöön ja Applen vakiokäyttöoikeussopimukseen; Settings voi linkittää App Store:n arvostelusivulle. Näihin linkkeihin ei ole liitetty käyttäjätietoja tai sovelluskohtaista tunnistetta – ne ovat tavallisia URL-osoitteita, samat kaikille.

## Ei mitään vetoa

GeoSweeper:ssä ei ole sovelluksen sisäistä valuuttaa, ei ryöstöä, ei arvontoja eikä ominaisuuksia, joissa tulos on panostettu tai panostettu. Jokainen ostos on kiinteä, julkistettu hinta pysyvästä tai aikarajaisesta pääsystä sisältöön. mitään ei voi voittaa, hävitä tai pelata.

## Mitä emme tee

- Ei analytiikkaa, virheraportointia tai minkäänlaista telemetriaa
- Ei mainontaa, ei mainosverkostoja eikä mainontatunnisteita
- Ei sovellusten tai sivustojen välistä seurantaa eikä tiedonvälittäjiä
- Ei tilejä, ei sisäänkirjautumista, ei salasanoja
- Ei kameraa, valokuvakirjastoa, mikrofonia, yhteystietoja, tarkkaa tai karkeaa sijaintia tai terveystietoja
- Ei koneoppimismallien koulutusta tiedoillasi
- Ei minkäänlaisia kolmannen osapuolen SDK:ita – ainoa koodi tässä sovelluksessa on omamme

Tämä vastaa "Data Not Collected (tietoja ei kerätä)" -merkkiä, jonka GeoSweeper kantaa mallissa App Store.

## Säilyttäminen ja poistaminen

Sovelluksen poistaminen poistaa kaikki laitteellesi tallennetut tiedostot – asetukset, maakohtaiset tietueesi ja Infinite Tower:n edistyminen – välittömästi ja kokonaan, koska meillä ei koskaan ollut palvelinkopiota, jota voisimme säilyttää tai poistaa. Ennen poistamista tehty iCloud-laitteen varmuuskopio saattaa silti sisältää kopion; että varmuuskopiointi on täysin sinun hallinnassasi laitteesi **Settings → nimesi → iCloud → Hallinnoi tilin tallennustilaa** kautta. Tukiviestit säilytetään ja poistetaan erikseen yllä kuvatulla tavalla.

## Sinun oikeutesi

Koska GeoSweeper ei säilytä kopiota sovelluksen sisäisistä tiedoistasi, GDPR:n, Yhdistyneen kuningaskunnan GDPR:n ja CCPA/CPRA:n kuvaamat käyttö-, korjaus-, vienti- ja poistooikeudet ovat sellaisia, joita käytät jo suoraan omalla laitteellasi – täällä ei ole tietuetta, jonka voisimme tuottaa tai poistaa puolestasi. Ainoa paikka, jossa meillä on jotain, on meille lähettämäsi tukisähköposti, ja voit milloin tahansa pyytää nähdä, korjata tai poistaa sen kirjoittamalla osoitteeseen ivnsjdev@gmail.com. Emme myy tai jaa henkilökohtaisia ​​tietoja kontekstien välistä käyttäytymiseen perustuvaa mainontaa varten, emmekä ole koskaan myynyt. Jos uskot, että olemme käsitelleet tietojasi väärin, sinulla on oikeus tehdä valitus paikalliselle tietosuojaviranomaiselle.

## Lapset

GeoSweeper:n ikäluokitus sopii suurelle yleisölle, eikä sitä ole suunnattu erityisesti lapsille. Emme tietoisesti kerää henkilökohtaisia ​​tietoja keneltäkään, mukaan lukien alle 13-vuotiaat lapset, eikä sovelluksessa ole mitään, mikä voisi – ei chattia, ei jakamista, ei sosiaalisia ominaisuuksia, ei mainontaa tai tiliä kolmannelle osapuolelle, jonka kautta lapsi tavoittaisi.

## Muutoksia tähän käytäntöön

Jos tämä käytäntö muuttuu, yläreunassa oleva päivämäärä muuttuu sen mukana, ja merkittävä muutos siihen, mitä GeoSweeper tekee tiedoilla, merkitään myös kyseisen päivityksen julkaisutietoihin.

## Ota yhteyttä

ivnsjdev@gmail.com
