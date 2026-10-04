# Politica de Confidențialitate pentru GeoSweeper

**Data intrării în vigoare:** 26 septembrie 2026

**Ultima actualizare:** 4 octombrie 2026

## Versiunea pe scurt

GeoSweeper nu colectează, nu transmite, nu vinde și nu partajează nicio informație personală. Fiecare tablă pe care o joci, fiecare setare pe care o alegi și fiecare țară pe care ai finalizat-o este stocată doar pe dispozitivul tău. Nimic nu este încărcat la noi, și nici măcar nu există un cont de creat. Singurul trafic de rețea pe care GeoSweeper îl generează vreodată este StoreKit care comunică cu Apple atunci când faci sau restaurezi o achiziție, și paginile pe care le deschizi în mod deliberat printr-un link din aplicație (acest site, sau propriile pagini legale ale Apple) — ambele sunt acoperite mai jos, și niciuna nu transportă altceva odată cu ea.

## Cine suntem

GeoSweeper este dezvoltat de Ivan Cayabyab. Întrebările despre această politică sau despre aplicație pot fi trimise la ivnsjdev@gmail.com.

## Ce stochează aplicația, și unde

Tot ce urmează există doar pe dispozitivul tău, în unul din trei locuri: `UserDefaults` (valori mici de setări), un fișier JSON în folderul propriu Application Support al aplicației, sau o bază de date locală SQLite.

| Ce | Stocare principală | Trimis automat la noi? |
|---|---|---|
| Setări de afișare — temă tablă, culoare neon, efect de explozie, sunet de explozie, proiecție hartă (Globe sau Flat), sunet și vibrații pornite/oprite | `UserDefaults` | Nu |
| Limba pe care ai ales-o în aplicație | `UserDefaults` | Nu |
| Evidența solicitărilor de evaluare — datele la care GeoSweeper a cerut iOS-ului să afișeze fișa nativă de evaluare, și ce prag a declanșat ultima solicitare | `UserDefaults` | Nu |
| Contoare de jocuri gratuite — câte dintre cele 10 țări gratuite de pe hartă și cele 10 jocuri Classic gratuite ai folosit | `UserDefaults` | Nu |
| Recordul pe fiecare țară — victorii, înfrângeri, cel mai bun timp și când ai deblocat-o, pentru fiecare țară jucată | Un fișier JSON (`progress.json`) în folderul Application Support al aplicației | Nu |
| Istoricul modului Classic — mărimea tablei, dificultatea, numărul de mine, timpul și victoria-sau-înfrângerea fiecărui joc Classic finalizat | Un fișier JSON (`Classic/history.json`) în folderul Application Support al aplicației | Nu |
| Progresul în Infinite Tower — rândul la care ai ajuns, viewport-ul salvat și rândurile pe care le-ai finalizat | O bază de date locală SQLite | Nu |

Niciuna dintre acestea nu este transmisă, vândută sau partajată cu nimeni, inclusiv cu noi. Propriul trafic al StoreKit (mai jos) și linkurile externe pe care le atingi (de asemenea mai jos) nu transportă nimic din acestea. O copie de rezervă a dispozitivului iOS poate include aceste fișiere ca parte a copierii de rezervă a întregii aplicații — acea copie de rezervă este inițiată de tine sau de iOS, niciodată de GeoSweeper, și rămâne oriunde o trimiți (iCloud sau calculatorul tău), nu la noi.

## Fără cont, fără autentificare, fără cloud

GeoSweeper nu cere niciodată un nume, o adresă de e-mail, un număr de telefon, o dată de naștere sau orice altă informație de identificare — nu există nimic cu care să te autentifici, pentru că nu există niciun cont. Progresul tău nu se sincronizează prin iCloud, CloudKit sau orice alt serviciu: există doar pe dispozitivul pe care joci. Joacă aceeași țară pe un al doilea dispozitiv și va porni de la zero acolo, pentru că nu există nicio copie pe un server de unde să se sincronizeze.

## Ceva ce în mod deliberat nu este salvat

Tabla în care te afli în acest moment — fiecare pătrat pe care l-ai deschis, fiecare steag pe care l-ai plasat — este păstrată doar în memorie cât timp joci. Acest lucru este valabil în toate cele trei lumi: harta, modul Classic și Infinite Tower. Închide aplicația la mijlocul unui joc și acea tablă dispare; nu este niciodată scrisă pe disc, și nu există o salvare automată pentru a relua o tablă neterminată. Doar un joc *finalizat* (o victorie sau o înfrângere) actualizează recordul pe țară sau istoricul Classic descris mai sus.

## Singurul lucru care sună ca și cum nu ar fi local

Harta se deschide pe propria ta țară prima dată când deschizi aplicația. Acest lucru provine din **setarea de regiune** a dispozitivului tău (țara asociată limbii și setărilor regionale tale, aceeași pe care iOS o folosește pentru a alege o tastatură și un calendar) — nu din GPS, Wi-Fi sau orice altă formă de urmărire a locației. GeoSweeper nu solicită acces la locație și nu ar putea citi coordonatele tale nici chiar dacă ar vrea.

## Permisiuni

GeoSweeper nu solicită nicio permisiune de sistem. Nu cere niciodată camera, biblioteca foto, microfonul, locația, contactele, calendarul, datele de sănătate, datele de mișcare sau notificările push, și nu va apărea niciodată niciun mesaj de solicitare a permisiunilor. Acest lucru se potrivește exact cu `Info.plist` al aplicației: nu există nicio intrare de descriere a utilizării în el.

## Achiziții

GeoSweeper este gratuit de descărcat, iar fiecare dintre cele trei lumi ale sale are propria perioadă de probă gratuită. Primele tale 10 țări de pe hartă — orice nivel, inclusiv Beginner — sunt gratuite de jucat, iar odată ce ai jucat o țară, aceasta rămâne rejucabilă pentru totdeauna, chiar și după ce acea perioadă de probă este consumată. Modul Classic îți oferă 10 jocuri gratuite în același fel. Infinite Tower este gratuit până la rândul 10. Dincolo de aceste puncte, există trei achiziții independente, toate unice, neconsumabile și oferite prin StoreKit-ul Apple și procesate în întregime de Apple:

- **All Countries** — o achiziție unică, neconsumabilă, care deblochează permanent nivelurile Intermediate, Expert și Mega pentru toate cele 204 țări. Nimic legat de aceasta nu se reînnoiește.
- **Classic Lifetime** — o achiziție unică, neconsumabilă, care deblochează permanent jocuri Classic nelimitate odată ce cele 10 gratuite sunt consumate. Nimic legat de aceasta nu se reînnoiește.
- **Infinite Tower Lifetime** — o achiziție unică, neconsumabilă, care deblochează permanent urcarea peste rândul 10. Nici aceasta nu se reînnoiește, iar GeoSweeper nu oferă niciun abonament de niciun fel.

Apple, nu GeoSweeper, procesează fiecare plată. Niciun număr de card, adresă de facturare sau credențial Apple Account nu ne este vreodată vizibil — StoreKit îi spune aplicației doar ce are nevoie pentru a afișa un ecran de achiziție și pentru a acorda acces: prețul de afișat și dacă deții deja fiecare articol. Aceste răspunsuri rămân pe dispozitivul tău; GeoSweeper nu operează propriul server de achiziții și nu are unde să le trimită. Restaurarea achizițiilor îi cere Apple să reconfirme ce deține contul tău Apple și aplică răspunsul local — nu creează și nu transmite nicio înregistrare nouă.

Vezi de asemenea [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/) al Apple, [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/), și [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), care guvernează achiziția în sine.

## Comunicări de suport

Dacă trimiți un e-mail la ivnsjdev@gmail.com, primim adresa ta de e-mail, tot ce scrii și orice atașament pe care alegi să îl adaugi. Îl folosim doar pentru a-ți răspunde și pentru a rezolva problema despre care ai scris — temeiul nostru legal este interesul nostru legitim de a răspunde celor care ne contactează. Această căsuță poștală este un cont Gmail standard, procesat de Google LLC conform [Politicii de Confidențialitate a Google](https://policies.google.com/privacy), și găzduit pe infrastructură care poate fi localizată în afara țării tale, motiv pentru care acest transfer este dezvăluit aici. Păstrăm e-mailurile de suport până la 24 de luni și apoi le ștergem; ne poți cere să ștergem un anumit e-mail mai devreme, oricând, scriindu-ne la aceeași adresă.

## Linkuri externe

Ecranele de achiziție ale GeoSweeper trimit către politica de confidențialitate a acestui site și către Standard EULA al Apple; Settings poate trimite către pagina de recenzii din App Store. Niciun date de utilizator sau identificator specific aplicației nu este adăugat la niciunul dintre aceste linkuri — sunt URL-uri simple, identice pentru toată lumea.

## Nimic de mizat

GeoSweeper nu are monedă în aplicație, pradă, extrageri de premii sau vreo funcție în care un rezultat este mizat sau riscat. Fiecare achiziție are un preț fix, dezvăluit, pentru acces permanent sau limitat în timp la conținut; nimic nu poate fi câștigat, pierdut sau jucat la noroc.

## Ce NU facem

- Nicio analiză, raportare de erori sau telemetrie de niciun fel
- Nicio publicitate, nicio rețea publicitară și niciun identificator publicitar
- Nicio urmărire între aplicații sau site-uri, și niciun broker de date
- Niciun cont, nicio autentificare, nicio parolă
- Nicio cameră, bibliotecă foto, microfon, contacte, locație precisă sau aproximativă, sau date de sănătate
- Nicio antrenare de modele de învățare automată pe datele tale
- Niciun SDK terț de niciun fel — singurul cod din această aplicație este al nostru

Acest lucru corespunde etichetei "Data Not Collected" (date nu sunt colectate) pe care GeoSweeper o are pe App Store.

## Păstrare și ștergere

Ștergerea aplicației elimină fiecare fișier pe care l-a stocat pe dispozitivul tău — setări, recordul tău pe țară, istoricul Classic și progresul tău în Infinite Tower — imediat și complet, pentru că nu a existat niciodată o copie pe server pe care noi să o păstrăm sau să o ștergem la rândul nostru. O copie de rezervă iCloud a dispozitivului făcută înainte de ștergere poate încă conține o copie; acea copie de rezervă este în întregime sub controlul tău prin **Setări → numele tău → iCloud → Gestionează stocarea contului** de pe dispozitivul tău. E-mailurile de suport sunt păstrate și șterse separat, așa cum este descris mai sus.

## Drepturile tale

Deoarece GeoSweeper nu păstrează nicio copie a datelor tale din aplicație, drepturile de acces, corectare, export și ștergere descrise de GDPR, UK GDPR și CCPA/CPRA sunt drepturi pe care le exerciți deja direct, pe propriul tău dispozitiv — nu există aici nicio înregistrare pe care noi să o producem sau să o ștergem în numele tău. Singurul loc unde păstrăm ceva este un e-mail de suport pe care ni l-ai trimis, și poți cere să îl vezi, să îl corectezi sau să îl ștergi oricând, scriindu-ne la ivnsjdev@gmail.com. Nu vindem și nu partajăm informații personale pentru publicitate comportamentală trans-contextuală, și nu am făcut-o niciodată. Dacă crezi că am gestionat greșit datele tale, ai dreptul să depui o plângere la autoritatea ta locală de protecție a datelor.

## Copii

GeoSweeper are o clasificare de vârstă potrivită pentru publicul general și nu este direcționat în mod special către copii. Nu colectăm cu bună știință nicio informație personală de la nimeni, inclusiv de la copii sub 13 ani, și nu există nimic în aplicație care ar putea face asta — niciun chat, nicio partajare, nicio funcție socială, nicio publicitate și niciun cont prin care un terț să poată ajunge la un copil.

## Modificări ale acestei politici

Dacă această politică se schimbă, data din partea de sus se va schimba odată cu ea, iar o modificare substanțială a modului în care GeoSweeper gestionează datele va fi menționată și în notele de lansare ale acelei actualizări.

## Contact

ivnsjdev@gmail.com
