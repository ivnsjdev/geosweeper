# Zásady ochrany osobních údajů pro GeoSweeper

**Datum účinnosti:** 26. září 2026

**Poslední aktualizace:** 26. září 2026

## Krátká verze

GeoSweeper neshromažďuje, nepřenáší, neprodává ani nesdílí žádné osobní údaje. Každá hrací deska, kterou hrajete, každé zvolené nastavení a každá země, kterou jste vymazali, jsou uloženy pouze ve vašem zařízení. Nic se nám nenahrává a v první řadě není potřeba vytvořit žádný účet. Jediný síťový provoz, který kdy GeoSweeper generuje, je rozhovor StoreKit s Apple, když provedete nebo obnovíte nákup, a stránky, které záměrně otevřete z odkazu v aplikaci (tento web nebo vlastní právní stránky společnosti Apple) – obojí je uvedeno níže a žádná s sebou nenese nic jiného.

## Kdo jsme

GeoSweeper je vyvinut Ivanem Cayabyabem. Dotazy týkající se těchto zásad nebo aplikace můžete zasílat na adresu ivnsjdev@gmail.com.

## Co aplikace ukládá a kde

Vše níže žije pouze ve vašem zařízení, na jednom ze tří míst: „UserDefaults“ (malé hodnoty nastavení), soubor JSON ve vlastní složce Application Support aplikace nebo místní databáze SQLite.

| Co | Primární úložiště | Odesláno automaticky k nám? |
|---|---|---|
| Nastavení zobrazení — motiv desky, neonová barva, efekt exploze, zvuk výbuchu, projekce mapy (zeměkoule nebo plochá), zapnutí/vypnutí zvuku a haptiky | `UserDefaults` | Ne |
| Language jste si vybrali v aplikaci | `UserDefaults` | Ne |
| Vedení účetnictví na základě hodnocení – data, kdy GeoSweeper požádal iOS o zobrazení nativního listu hodnocení, a který milník spustil ten poslední | `UserDefaults` | Ne |
| Rekord v jednotlivých zemích – výhry, prohry, nejlepší čas a když jste jej odemkli, pro každou zemi, ve které jste hráli | Soubor JSON (`progress.json`) ve složce Application Support | Ne |
| Průběh Infinite Tower — řádek, kterého jste dosáhli, váš uložený výřez a které řádky jste vymazali | Lokální databáze SQLite | Ne |

Nic z toho není přenášeno, prodáváno ani sdíleno s nikým, včetně nás. Vlastní provoz StoreKit (níže) a externí odkazy, na které klepnete (také níže), nic z toho nenesou. Záloha zařízení iOS může obsahovat tyto soubory jako součást zálohování aplikace jako celku – tuto zálohu iniciujete vy nebo iOS, nikdy GeoSweeper, a zůstane, kamkoli ji odešlete (iCloud nebo váš počítač), nikoli u nás.

## Žádný účet, žádné přihlášení, žádný cloud

GeoSweeper nikdy nepožaduje jméno, e-mailovou adresu, telefonní číslo, datum narození ani žádné jiné identifikační údaje – není zde nic k přihlášení, protože neexistuje žádný účet. Váš postup se nesynchronizuje přes iCloud, CloudKit ani žádnou jinou službu: funguje pouze na zařízení, na kterém hrajete. Zahrajte si stejnou zemi na druhém zařízení a tam to začne znovu, protože nikde není žádná kopie serveru, ze které by se dala synchronizovat.

## Cokoli úmyslně nepřetrvávalo

Hrací deska, na které se nacházíte – každá dlaždice, kterou jste otevřeli, každá vlajka, kterou jste umístili – je během hraní uložena pouze v paměti. Zavřete aplikaci uprostřed hry a deska je pryč; nikdy se nezapisuje na disk a neexistuje žádné automatické ukládání, ze kterého by bylo možné obnovit nedokončenou desku. Pouze *dokončená* hra (výhra nebo prohra) aktualizuje výše popsaný rekord pro každou zemi.

## Jedna věc, která zní, jako by to nebylo místní

Při prvním spuštění aplikace se mapa otevře ve vaší zemi. Pochází z **nastavení regionu** vašeho zařízení (země spojená s vaším jazykem a národním prostředím, stejná, jakou iOS používá k výběru klávesnice a kalendáře) – nikoli z GPS, Wi-Fi nebo jakékoli jiné formy sledování polohy. GeoSweeper nepožaduje přístup k poloze a nemohl přečíst vaše souřadnice, i kdyby chtěl.

## Oprávnění

GeoSweeper nevyžaduje žádná systémová oprávnění. Nikdy nepožaduje fotoaparát, knihovnu fotografií, mikrofon, polohu, kontakty, kalendář, zdravotní údaje, údaje o pohybu nebo oznámení push a nikdy se neobjeví žádná výzva k povolení jakéhokoli druhu. To přesně odpovídá `Info.plist` aplikace: není v něm jediný záznam s popisem použití.

## Nákupy

GeoSweeper je zdarma ke stažení. Prvních 10 zemí – na jakékoli úrovni, včetně Beginner – lze hrát zdarma, a jakmile si zahrajete zemi, zůstane hratelná navždy i po uplynutí této bezplatné zkušební verze. Infinite Tower je zdarma až do řádku 10. Kromě těchto dvou bodů existují dva nezávislé nákupy, oba jednorázové, nespotřebovatelné a nabízené prostřednictvím StoreKit společnosti Apple a zcela zpracované společností Apple:

- **All Countries** – jednorázový nákup bez spotřeby, který trvale odemkne
  Intermediate, Expert a Mega ve všech 204 zemích. Nic z toho se neobnovuje.
- **Infinite Tower Lifetime** – jednorázový nákup bez spotřeby, který se trvale odemkne
  lezení přes řadu 10. Nic o tom se také neobnovuje a GeoSweeper nenabízí žádné předplatné jakéhokoli druhu.

Apple, nikoli GeoSweeper, zpracovává každou platbu. Žádné číslo karty, fakturační adresa ani pověření Apple Account se nám nikdy nezobrazují – StoreKit pouze říká aplikaci, co potřebuje k zobrazení paywallu a udělení přístupu: cena, která se má zobrazit, a zda aktuálně vlastníte jednotlivé položky. Tyto odpovědi zůstanou ve vašem zařízení; GeoSweeper neprovozuje vlastní nákupní server a nemá je kam poslat. Obnovení nákupů žádá Apple, aby znovu potvrdil, co váš Apple Account vlastní, a použije odpověď lokálně – nevytváří ani nepřenáší žádný nový záznam.

Viz také Apple [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) a [Standardní EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), kterými se řídí samotný nákup.

## Podpora komunikace

Pokud pošlete e-mail ivnsjdev@gmail.com, obdržíme vaši e-mailovou adresu, cokoli napíšete, a jakoukoli přílohu, kterou se rozhodnete přidat. Používáme je pouze k tomu, abychom vám odpověděli a vyřešili problém, o kterém jste psali – naším zákonným základem je náš oprávněný zájem odpovídat lidem, kteří nás kontaktují. Tato poštovní schránka je standardní účet Gmail, zpracovávaný společností Google LLC podle [zásad ochrany soukromí společnosti Google](https://policies.google.com/privacy) a hostovaný v infrastruktuře, která se může nacházet mimo vaši zemi, a proto je zde tento převod uveden. E-maily podpory uchováváme po dobu až 24 měsíců a poté je smažeme; můžete nás kdykoli požádat o smazání konkrétního e-mailu dříve, když napíšete na stejnou adresu.

## Externí odkazy

Paywally GeoSweeper odkazují na vlastní zásady ochrany osobních údajů tohoto webu a na standardní EULA společnosti Apple; Settings může odkazovat na stránku App Store pro zápis recenze. K žádnému z těchto odkazů nejsou připojena žádná uživatelská data ani identifikátor konkrétní aplikace – jedná se o prosté adresy URL, stejné pro všechny.

## Není co vsadit

GeoSweeper nemá žádnou měnu v aplikaci, žádnou kořist, žádné losování o ceny a žádnou funkci, kde se sází nebo sází výsledek. Každý nákup je pevná, zveřejněná cena za trvalý nebo časově ohraničený přístup k obsahu; nic nelze vyhrát, prohrát ani sázet.

## Co NEDĚLÁME

- Žádné analýzy, hlášení o selhání nebo telemetrie jakéhokoli druhu
- Žádná reklama, žádné reklamní sítě a žádné reklamní identifikátory
- Žádné sledování napříč aplikacemi nebo weby a žádní zprostředkovatelé dat
- Žádné účty, žádné přihlášení, žádná hesla
- Žádný fotoaparát, knihovna fotografií, mikrofon, kontakty, přesné nebo hrubé umístění nebo zdravotní údaje
- Žádné školení modelů strojového učení na vašich datech
- Žádné sady SDK třetích stran jakéhokoli druhu – jediný kód v této aplikaci je náš vlastní

To odpovídá označení „Data Not Collected (údaje nejsou shromažďovány)“, které GeoSweeper nese na App Store.

## Uchování a smazání

Smazáním aplikace dojde k okamžitému a úplnému odstranění všech souborů, které uložila ve vašem zařízení – nastavení, záznamů v jednotlivých zemích a pokroku v Infinite Tower, protože nikdy neexistovala kopie serveru, kterou bychom si mohli ponechat nebo z naší strany smazat. Záloha zařízení iCloud vytvořená před vymazáním může stále obsahovat kopii; tato záloha je zcela pod vaší kontrolou prostřednictvím **Settings → vaše jméno → iCloud → Správa úložiště účtu** na vašem zařízení. E-maily podpory jsou uchovávány a mazány samostatně, jak je popsáno výše.

## Vaše práva

Protože GeoSweeper neuchovává žádnou kopii vašich dat v aplikaci, práva na přístup, opravu, export a smazání, která GDPR, UK GDPR a CCPA/CPRA popisují, jsou práva, která již uplatňujete přímo na vašem vlastním zařízení – neexistuje zde žádný záznam, který bychom mohli vaším jménem vytvořit nebo vymazat. Jediné místo, kde něco uchováváme, je e-mail podpory, který jste nám poslali, a můžete kdykoli požádat o jeho zobrazení, opravu nebo smazání, když napíšete na adresu ivnsjdev@gmail.com. Neprodáváme ani nesdílíme osobní údaje pro mezikontextovou behaviorální reklamu a nikdy jsme neprodávali. Pokud se domníváte, že jsme s vašimi údaji zacházeli nesprávně, máte právo podat stížnost místnímu úřadu pro ochranu údajů.

## Děti

GeoSweeper nese věkové hodnocení vhodné pro širokou veřejnost a není zaměřeno konkrétně na děti. Vědomě neshromažďujeme osobní údaje od nikoho, včetně dětí mladších 13 let, a v aplikaci není nic, co by to mohlo – žádný chat, žádné sdílení, žádné sociální funkce, žádná reklama a žádný účet pro třetí stranu, přes který by dítě mohla oslovit.

## Změny těchto zásad

Pokud se tato zásada změní, změní se s ní i datum nahoře a podstatná změna toho, co GeoSweeper dělá s daty, bude také uvedena v poznámkách k vydání této aktualizace.

## Kontakt

ivnsjdev@gmail.com
