# Politique de confidentialité de GeoSweeper

**Date d'entrée en vigueur :** 26 septembre 2026

**Dernière mise à jour :** 26 septembre 2026

## En bref

GeoSweeper ne collecte, ne transmet, ne vend ni ne partage aucune information personnelle.
Chaque plateau auquel vous jouez, chaque réglage que vous choisissez et chaque pays que vous
avez terminé est stocké uniquement sur votre appareil. Rien n'est envoyé vers nos serveurs, et
il n'existe d'ailleurs aucun compte à créer. Le seul trafic réseau que GeoSweeper génère est
celui de StoreKit qui communique avec Apple lorsque vous effectuez ou restaurez un achat, et
les pages que vous ouvrez volontairement depuis un lien dans l'application (ce site, ou les
pages légales d'Apple elles-mêmes) — les deux cas sont détaillés plus bas, et aucun des deux
n'emporte rien d'autre avec lui.

## Qui nous sommes

GeoSweeper est développée par Ivan Cayabyab. Toute question sur cette politique ou sur
l'application peut être envoyée à ivnsjdev@gmail.com.

## Ce que l'application stocke, et où

Tout ce qui suit ne vit que sur votre appareil, dans l'un de ces trois emplacements :
`UserDefaults` (petites valeurs de réglages), un fichier JSON dans le dossier Application
Support propre à l'application, ou une base de données SQLite locale.

| Quoi | Stockage principal | Envoyé automatiquement chez nous ? |
|---|---|---|
| Réglages d'affichage — thème du plateau, couleur néon, effet d'explosion, son d'impact, projection de la carte (**Globe** ou **Flat**), son et retours haptiques activés/désactivés | `UserDefaults` | Non |
| Langue choisie dans l'application | `UserDefaults` | Non |
| Suivi de l'invite de notation — les dates auxquelles GeoSweeper a demandé à iOS d'afficher la feuille de notation native, et quel jalon a déclenché la dernière | `UserDefaults` | Non |
| Record par pays — victoires, défaites, meilleur temps, et date de déblocage, pour chaque pays auquel vous avez joué | Un fichier JSON (`progress.json`) dans le dossier Application Support de l'application | Non |
| Progression d'**Infinite Tower** — la ligne atteinte, votre vue enregistrée, et les lignes franchies | Une base de données SQLite locale | Non |

Rien de tout cela n'est transmis, vendu ou partagé avec qui que ce soit, y compris nous-mêmes.
Le trafic propre à StoreKit (ci-dessous) et les liens externes que vous ouvrez (également
ci-dessous) n'en transportent rien non plus. Une sauvegarde de votre appareil iOS peut inclure
ces fichiers dans le cadre de la sauvegarde de l'application dans son ensemble — cette
sauvegarde est déclenchée par vous ou par iOS, jamais par GeoSweeper, et elle reste là où vous
l'envoyez (iCloud ou votre ordinateur), pas chez nous.

## Aucun compte, aucune connexion, aucun cloud

GeoSweeper ne demande jamais de nom, d'adresse e-mail, de numéro de téléphone, de date de
naissance ni aucune autre information d'identification — il n'y a rien avec quoi se connecter,
puisqu'il n'y a pas de compte. Votre progression ne se synchronise pas via iCloud, CloudKit ou
tout autre service : elle ne vit que sur l'appareil sur lequel vous jouez. Jouez au même pays
sur un second appareil et il repart de zéro là-bas, car il n'existe nulle part de copie sur un
serveur avec laquelle se synchroniser.

## Ce qui n'est volontairement pas conservé

Le plateau en cours de partie — chaque case ouverte, chaque drapeau posé — n'est conservé qu'en
mémoire pendant que vous jouez. Fermez l'application en pleine partie et ce plateau disparaît ;
il n'est jamais écrit sur le disque, et il n'existe aucune sauvegarde automatique pour reprendre
un plateau inachevé. Seule une partie *terminée* (une victoire ou une défaite) met à jour le
record par pays décrit ci-dessus.

## La seule chose qui a l'air de ne pas être locale

La carte s'ouvre sur votre propre pays la première fois que vous lancez l'application. Cela
provient du **réglage régional** de votre appareil (le pays associé à votre langue et à vos
paramètres régionaux, le même qu'iOS utilise pour choisir un clavier et un calendrier) — pas du
GPS, du Wi-Fi, ni d'aucune autre forme de suivi de localisation. GeoSweeper ne demande aucun
accès à la localisation et ne pourrait pas lire vos coordonnées même s'il le voulait.

## Autorisations

GeoSweeper ne demande aucune autorisation système. Il ne demande jamais l'accès à l'appareil
photo, à la photothèque, au microphone, à la localisation, aux contacts, au calendrier, aux
données de santé, aux données de mouvement ni aux notifications push, et aucune invite
d'autorisation d'aucune sorte n'apparaîtra jamais. Cela correspond exactement au fichier
`Info.plist` de l'application : il n'y contient pas une seule entrée de description d'usage.

## Achats

GeoSweeper est gratuit à télécharger. Vos 10 premiers pays — de n'importe quel niveau, y
compris **Beginner** — sont gratuits à jouer, et une fois qu'un pays a été joué, il reste
rejouable pour de bon, même après épuisement de cet essai gratuit. **Infinite Tower** est
gratuit jusqu'à la ligne 10. Au-delà de ces deux points, il existe deux achats indépendants,
tous deux uniques, non consommables, proposés via StoreKit d'Apple et traités entièrement par
Apple :

- **All Countries** — un achat unique et non consommable qui débloque de façon permanente les
  niveaux **Intermediate**, **Expert** et **Mega** pour les 204 pays. Rien de tout cela ne se
  renouvelle.
- **Infinite Tower Lifetime** — un achat unique et non consommable qui débloque de façon
  permanente la progression au-delà de la ligne 10. Cela ne se renouvelle pas non plus, et
  GeoSweeper ne propose aucun abonnement d'aucune sorte.

Apple, et non GeoSweeper, traite chaque paiement. Aucun numéro de carte, adresse de
facturation ni identifiant de votre compte Apple ne nous est jamais visible — StoreKit ne
communique à l'application que ce dont elle a besoin pour afficher un écran d'achat et
accorder l'accès : le prix à afficher, et si vous possédez déjà chaque élément. Ces réponses
restent sur votre appareil ; GeoSweeper ne gère aucun serveur d'achats propre et n'a nulle part
où les envoyer. Restaurer les achats demande à Apple de reconfirmer ce que possède votre compte
Apple et applique la réponse localement — cela ne crée ni ne transmet aucun nouvel
enregistrement.

Voir aussi les documents d'Apple [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/),
les [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/), et le
[Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), qui
régissent l'achat lui-même.

## Communications de support

Si vous écrivez à ivnsjdev@gmail.com, nous recevons votre adresse e-mail, ce que vous écrivez
et toute pièce jointe que vous choisissez d'ajouter. Nous l'utilisons uniquement pour vous
répondre et résoudre le problème que vous avez signalé — notre base légale est notre intérêt
légitime à répondre aux personnes qui nous contactent. Cette boîte de réception est un compte
Gmail standard, traité par Google LLC selon la
[politique de confidentialité de Google](https://policies.google.com/privacy), et hébergé sur
une infrastructure pouvant se trouver hors de votre propre pays, raison pour laquelle ce
transfert est mentionné ici. Nous conservons les e-mails de support jusqu'à 24 mois puis les
supprimons ; vous pouvez nous demander de supprimer un e-mail précis plus tôt à tout moment en
écrivant à la même adresse.

## Liens externes

Les écrans d'achat de GeoSweeper renvoient vers la politique de confidentialité de ce site et
vers le Standard EULA d'Apple ; Settings peut renvoyer vers la page d'avis de l'App Store.
Aucune donnée utilisateur ni identifiant propre à l'application n'est ajouté à ces liens — ce
sont de simples URL, identiques pour tout le monde.

## Rien à miser

GeoSweeper n'a aucune monnaie interne, aucun butin, aucun tirage au sort, et aucune
fonctionnalité où un résultat serait misé ou risqué. Chaque achat correspond à un prix fixe et
annoncé pour un accès permanent ou limité dans le temps à du contenu ; rien ne peut être gagné,
perdu ou joué.

## Ce que nous NE faisons PAS

- Aucun suivi analytique, rapport de plantage ou télémétrie d'aucune sorte
- Aucune publicité, aucun réseau publicitaire, et aucun identifiant publicitaire
- Aucun suivi entre applications ou sites, et aucun courtier en données
- Aucun compte, aucune connexion, aucun mot de passe
- Aucun accès à l'appareil photo, à la photothèque, au microphone, aux contacts, à la
  localisation précise ou approximative, ni aux données de santé
- Aucun entraînement de modèles d'apprentissage automatique sur vos données
- Aucun SDK tiers d'aucune sorte — le seul code de cette application est le nôtre

Cela correspond à l'étiquette **Data Not Collected (données non collectées)** que GeoSweeper
porte sur l'App Store.

## Conservation et suppression

Supprimer l'application supprime tous les fichiers qu'elle a stockés sur votre appareil —
réglages, votre record par pays, et votre progression dans Infinite Tower — immédiatement et
entièrement, puisqu'il n'y a jamais eu de copie sur un serveur que nous pourrions conserver ou
supprimer de notre côté. Une sauvegarde iCloud effectuée avant la suppression peut encore en
contenir une copie ; cette sauvegarde reste entièrement sous votre contrôle via **Settings →
votre nom → iCloud → Gérer le stockage du compte** sur votre appareil. Les e-mails de support
sont conservés et supprimés séparément, comme décrit ci-dessus.

## Vos droits

Comme GeoSweeper ne conserve aucune copie de vos données internes, les droits d'accès, de
rectification, d'exportation et de suppression que décrivent le RGPD, le RGPD britannique et
le CCPA/CPRA sont des droits que vous exercez déjà directement, sur votre propre appareil — il
n'existe ici aucun enregistrement que nous pourrions produire ou effacer en votre nom. Le seul
endroit où nous détenons effectivement quelque chose est un e-mail de support que vous nous
avez envoyé, et vous pouvez demander à le consulter, le corriger ou le supprimer à tout moment
en écrivant à ivnsjdev@gmail.com. Nous ne vendons ni ne partageons d'informations personnelles
à des fins de publicité comportementale intercontextuelle, et ne l'avons jamais fait. Si vous
estimez que nous avons mal géré vos données, vous avez le droit de déposer une plainte auprès
de votre autorité locale de protection des données.

## Enfants

GeoSweeper porte une classification d'âge adaptée à un public général et ne s'adresse pas
spécifiquement aux enfants. Nous ne collectons sciemment aucune information personnelle
auprès de qui que ce soit, y compris les enfants de moins de 13 ans, et rien dans
l'application ne le permettrait — ni discussion, ni partage, ni fonctionnalité sociale, ni
publicité, ni compte par lequel un tiers pourrait atteindre un enfant.

## Modifications de cette politique

Si cette politique change, la date en haut de page changera avec elle, et tout changement
important concernant ce que GeoSweeper fait des données sera également signalé dans les notes
de version de cette mise à jour.

## Contact

ivnsjdev@gmail.com
