# Az GeoSweeper adatvédelmi szabályzata

**Hatálybalépés dátuma:** 2026. szeptember 26

**Utolsó frissítés:** 2026. szeptember 26

## A rövid változat

Az GeoSweeper nem gyűjt, továbbít, nem ad el vagy oszt meg személyes adatokat. Minden tábla, amellyel játszol, minden kiválasztott beállítás és minden törölt ország csak az eszközödön tárolódik. Semmit sem töltenek fel hozzánk, és először nincs létrehozandó fiók sem. Az egyetlen hálózati forgalom, amelyet az GeoSweeper generál, az az, hogy az StoreKit beszél az Apple-lel vásárláskor vagy visszaállításakor, valamint az alkalmazáson belüli linkről szándékosan megnyitott oldalak (ez a webhely vagy az Apple saját jogi oldalai) – mindkettőt alább tárgyaljuk, és egyik sem tartalmaz mást.

## Kik vagyunk

Az GeoSweeper-et Ivan Cayabyab fejlesztette ki. Az irányelvvel vagy az alkalmazással kapcsolatos kérdéseit az ivnsjdev@gmail.com címre küldheti.

## Mit és hol tárol az alkalmazás

Az alábbiakban felsoroltak csak az Ön eszközén élnek, a három hely egyikén: „UserDefaults” (kis beállítási értékek), egy JSON-fájl az alkalmazás saját Alkalmazástámogatás mappájában vagy egy helyi SQLite-adatbázis.

| Milyen | Elsődleges tárolás | Automatikusan elküldve nekünk? |
|---|---|---|
| Megjelenítési beállítások – táblatéma, neonszín, robbanáshatás, robbanáshang, térképvetítés (földgömb vagy lapos), hang és tapintás be/ki | `UserDefaults` | Nem |
| Language, amelyet az alkalmazásban választott | `UserDefaults` | Nem |
| Értékelési kérdőíves könyvelés – az GeoSweeper a natív értékelési lap megjelenítésére kért iOS dátumok, és hogy melyik mérföldkő váltotta ki az utolsót | `UserDefaults` | Nem |
| Országonkénti rekord – győzelmek, vereségek, legjobb idő, és amikor feloldottad, minden országban, ahol játszottál | JSON-fájl ("progress.json") az alkalmazás Alkalmazástámogatás mappájában | Nem |
| Infinite Tower előrehaladás — az elért sor, a mentett nézetablak és a törölt sorok | Egy helyi SQLite adatbázis | Nem |

Ezek egyikét sem továbbítják, értékesítik vagy megosztják senkivel, beleértve minket is. Az StoreKit saját forgalma (lent) és az Ön által megérintett külső hivatkozások (szintén lent) ezt nem hordozzák. Az iOS-eszköz biztonsági másolata tartalmazhatja ezeket a fájlokat az alkalmazás egészének biztonsági mentésének részeként – a biztonsági mentést Ön vagy az iOS kezdeményezi, az GeoSweeper soha, és bárhová küldi (iCloud vagy számítógépe), nem nálunk marad.

## Nincs fiók, nincs bejelentkezés, nincs felhő

Az GeoSweeper soha nem kér nevet, e-mail címet, telefonszámot, születési dátumot vagy bármilyen más azonosító adatot – nincs mivel bejelentkezni, mert nincs fiók. A haladás nem szinkronizálódik az iCloud, CloudKit vagy bármely más szolgáltatáson keresztül: csak azon az eszközön él, amelyen játszik. Ugyanazt az országot játssza le egy második eszközön, és ott kezdődik frissen, mert nincs sehol egy szerver másolat, ahonnan szinkronizálni lehetne.

## Bármi, ami szándékosan nem maradt fenn

A tábla, amelynek a közepén állsz – minden lapkát, amit kinyitottál, minden zászlót, amit lehelyeztél – játék közben csak a memória tárolja. Zárja be az alkalmazást játék közben, és a tábla eltűnik; soha nem írják lemezre, és nincs automatikus mentés a befejezetlen tábla folytatásához. Csak egy *befejezett* játék (győzelem vagy vereség) frissíti a fent leírt országonkénti rekordot.

## Az egyetlen dolog, ami úgy hangzik, mintha nem helyi lenne

A térkép a saját országában nyílik meg az alkalmazás első indításakor. Ez az eszköz **régióbeállításából** (az Ön nyelvéhez és területéhez kötött ország, ugyanaz, amelyet az iOS használ a billentyűzet és a naptár kiválasztásához) – nem a GPS-ből, Wi-Fi-ből vagy bármilyen más helymeghatározási módból. Az GeoSweeper nem kér hozzáférést a helyhez, és akkor sem tudta leolvasni a koordinátáit, ha akarná.

## Engedélyek

Az GeoSweeper semmilyen rendszerengedélyt nem kér. Soha nem kéri a kamerát, a fotótárat, a mikrofont, a helyet, a névjegyeket, a naptárat, az egészségügyi adatokat, a mozgásadatokat vagy a push értesítéseket, és soha nem jelenik meg semmilyen engedélykérő. Ez pontosan megegyezik az alkalmazás "Info.plist" fájljával: nincs benne egyetlen használati leírás sem.

## Vásárlások

Az GeoSweeper ingyenesen letölthető. Az első 10 országban – bármilyen szinten, beleértve az Beginner-et is – ingyenesen játszhatsz, és ha már játszottál egy országgal, az örökre újrajátszható marad, még az ingyenes próbaidőszak elteltével is. Az Infinite Tower a 10. sorig ingyenes. Ezen a két ponton kívül van még két független vásárlás, mindkettő egyszeri, nem fogyasztható, és az Apple StoreKit-en keresztül kínálja, és teljes egészében az Apple feldolgozza:

- **All Countries** – egyszeri, nem fogyóeszköz vásárlás, amely véglegesen feloldja a
  Intermediate, Expert és Mega szintek mind a 204 országban. Ezzel kapcsolatban semmi sem újul meg.
- **Infinite Tower Lifetime** – egyszeri, nem elfogyasztható vásárlás, amely véglegesen feloldja
  a 10. soron túllépve. Ezzel kapcsolatban sem újul meg semmi, és az GeoSweeper nem kínál semmiféle előfizetést.

Az Apple minden fizetést feldolgoz, nem az GeoSweeper. Soha nem láthatjuk a kártyaszámot, a számlázási címet vagy az Apple Account hitelesítési adatokat – az StoreKit csak azt mondja meg az alkalmazásnak, hogy mire van szüksége a fizetőfal megjelenítéséhez és a hozzáférés biztosításához: a megjelenítendő árat, és azt, hogy Ön jelenleg az egyes tételek tulajdonosa. Ezek a válaszok a készüléken maradnak; Az GeoSweeper nem futtat saját beszerzési szervert, és nincs hová küldenie őket. A vásárlások visszaállítása arra kéri az Apple-t, hogy erősítse meg az Apple Account tulajdonát, és helyileg alkalmazza a választ – nem hoz létre vagy továbbít új rekordot.

Lásd még az Apple [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) és [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) dokumentumát, amelyek magát a vásárlást szabályozzák.

## Támogassa a kommunikációt

Ha e-mailt küld az ivnsjdev@gmail.com-nek, megkapjuk e-mail-címét, bármit, amit ír, és minden olyan mellékletet, amelyet hozzáadni szeretne. Csak arra használjuk, hogy válaszoljunk Önnek, és megoldjuk azt a problémát, amelyről Ön írt – törvényes alapunk az, hogy jogos érdekünk, hogy válaszoljunk a velünk kapcsolatba lépő személyeknek. Ez a postafiók egy szabványos Gmail-fiók, amelyet a Google LLC dolgoz fel a [Google adatvédelmi irányelvei](https://policies.google.com/privacy) értelmében, és olyan infrastruktúrán tárolják, amely esetleg az Ön országán kívül található, ezért az átvitelt itt közöljük. A támogatási e-maileket legfeljebb 24 hónapig megőrizzük, majd töröljük őket; ugyanarra a címre írva bármikor kérhet tőlünk egy adott e-mail mielőbbi törlését.

## Külső hivatkozások

Az GeoSweeper fizetőfalai ennek a webhelynek a saját adatvédelmi szabályzatára és az Apple szabványos EULA-jára hivatkoznak; Az Settings hivatkozhat az App Store véleményezési oldalára. Ezekhez a linkekhez nem fűznek felhasználói adatokat vagy alkalmazásspecifikus azonosítót – ezek egyszerű URL-ek, mindenki számára ugyanazok.

## Nincs mit fogadni

Az GeoSweeper-nek nincs alkalmazáson belüli pénzneme, zsákmánya, nyereményjátéka, és nincs olyan funkciója, ahol az eredmény tét vagy fogadás lenne. Minden vásárlás rögzített, közzétett árat jelent a tartalomhoz való állandó vagy időzített hozzáférésért; semmit nem lehet nyerni, elveszíteni vagy szerencsejátékot játszani.

## Amit NEM csinálunk

- Nincs elemzés, hibajelentés vagy bármilyen telemetria
- Nincs reklám, nincsenek hirdetési hálózatok és nincsenek hirdetési azonosítók
- Nincs több alkalmazások vagy webhelyek közötti követés, és nincsenek adatközvetítők
- Nincsenek fiókok, nincs bejelentkezés, nincsenek jelszavak
- Nincs kamera, fotókönyvtár, mikrofon, névjegyek, pontos vagy durva helymeghatározás vagy egészségügyi adatok
- Nincsenek gépi tanulási modellek képzése az adatokon
- Nincsenek harmadik féltől származó SDK-k – ebben az alkalmazásban az egyetlen kód a sajátunk

Ez megegyezik az „Data Not Collected (nem gyűjtött adatok)” címkével, amelyet az GeoSweeper az App Store-en hordoz.

## Megőrzés és törlés

Az alkalmazás törlésével az eszközén tárolt minden fájl – beállítások, országonkénti rekordok és Infinite Tower előrehaladása – azonnal és teljesen törlődik, mert soha nem volt szervermásolat, amelyet megtarthatnánk vagy törölhettünk volna. A törlés előtt készített iCloud eszköz biztonsági másolata továbbra is tartalmazhat másolatot; hogy a biztonsági mentés teljes mértékben az Ön ellenőrzése alatt áll az eszközén található **Settings → az Ön neve → iCloud → Fióktárhely kezelése** segítségével. A támogatási e-maileket a fent leírtak szerint külön őrizzük meg és töröljük.

## Az Ön jogai

Mivel az GeoSweeper nem őriz másolatot az alkalmazáson belüli adatairól, a GDPR, az Egyesült Királyság GDPR és a CCPA/CPRA által leírt hozzáférési, javítási, exportálási és törlési jogokat Ön már közvetlenül, saját eszközén gyakorolja – itt nincs nyilvántartás, amelyet az Ön nevében előállíthatnánk vagy törölhetnénk. Az egyetlen hely, ahol tartunk valamit, az egy Ön által küldött támogatási e-mail, és bármikor kérheti annak megtekintését, javítását vagy törlését, ha ír az ivnsjdev@gmail.com címre. Nem adunk el és nem osztunk meg személyes adatokat kontextusokon átívelő viselkedésalapú reklámozás céljából, és soha nem is tettünk. Ha úgy gondolja, hogy helytelenül kezeltük adatait, Önnek joga van panaszt benyújtani a helyi adatvédelmi hatósághoz.

## Gyerekek

Az GeoSweeper korhatár-besorolása általános közönség számára megfelelő, és nem kifejezetten gyerekeknek szól. Tudatosan nem gyűjtünk személyes adatokat senkitől, beleértve a 13 éven aluli gyermekeket is, és az alkalmazásban nincs semmi, amivel – nincs csevegés, nincs megosztás, nincs közösségi funkció, nincs hirdetés, és nincs fiók harmadik fél számára, amelyen keresztül elérhetné a gyermeket.

## A szabályzat változásai

Ha ez a házirend módosul, a tetején látható dátum is megváltozik, és az GeoSweeper adatokkal kapcsolatos lényeges változásai szintén szerepelnek a frissítés kiadási megjegyzéseiben.

## Kapcsolat

ivnsjdev@gmail.com
