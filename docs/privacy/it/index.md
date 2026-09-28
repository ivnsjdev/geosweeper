# Informativa sulla privacy per GeoSweeper

**Data di entrata in vigore:** 26 settembre 2026

**Ultimo aggiornamento:** 26 settembre 2026

## La versione breve

GeoSweeper non raccoglie, trasmette, vende o condivide alcuna informazione personale. Ogni tabellone a cui giochi, ogni impostazione che scegli e ogni paese che hai eliminato vengono memorizzati solo sul tuo dispositivo. Non ci viene caricato nulla e non c'è nessun account da creare in primo luogo. L'unico traffico di rete che GeoSweeper genera è StoreKit che parla con Apple quando effettui o ripristini un acquisto e le pagine che apri deliberatamente da un collegamento all'interno dell'app (questo sito o le pagine legali di Apple): entrambi sono trattati di seguito e nessuno dei due porta con sé nient'altro.

## Chi siamo

GeoSweeper è sviluppato da Ivan Cayabyab. Domande su questa politica o sull'app possono essere inviate a ivnsjdev@gmail.com.

## Cosa memorizza l'app e dove

Tutto ciò che segue risiede solo sul tuo dispositivo, in uno dei tre posti: "UserDefaults" (piccoli valori di impostazione), un file JSON nella cartella Application Support dell'app o un database SQLite locale.

| Cosa | Memoria primaria | Inviato automaticamente a noi? |
|---|---|---|
| Impostazioni di visualizzazione: tema del tabellone, colore del neon, effetto esplosione, suono dell'esplosione, proiezione della mappa (globale o piatta), attivazione/disattivazione di suoni e aspetti tattili | "Impostazioni predefinite utente" | No |
| Language che hai scelto all'interno dell'app | "Impostazioni predefinite utente" | No |
| Contabilità con richiesta di valutazione: le date in cui GeoSweeper ha chiesto a iOS di mostrare la scheda di valutazione nativa e quale traguardo ha attivato l'ultima | "Impostazioni predefinite utente" | No |
| Record per paese: vittorie, sconfitte, miglior tempo e quando lo hai sbloccato, per ogni paese in cui hai giocato | Un file JSON (`progress.json`) nella cartella Supporto applicazioni dell'app | No |
| Avanzamento Infinite Tower: la riga che hai raggiunto, la visualizzazione salvata e le righe che hai cancellato | Un database SQLite locale | No |

Niente di tutto questo viene trasmesso, venduto o condiviso con nessuno, incluso noi. Il traffico di StoreKit (sotto) e i collegamenti esterni che tocchi (sempre sotto) non ne trasportano nulla. Un backup del dispositivo iOS può includere questi file come parte del backup dell'app nel suo insieme: il backup viene avviato da te o da iOS, mai da GeoSweeper, e rimane ovunque lo invii (iCloud o il tuo computer), non con noi.

## Nessun account, nessun accesso, nessun cloud

GeoSweeper non richiede mai nome, indirizzo email, numero di telefono, data di nascita o qualsiasi altra informazione identificativa: non c'è nulla con cui accedere, perché non esiste un account. I tuoi progressi non vengono sincronizzati tramite iCloud, CloudKit o qualsiasi altro servizio: risiedono solo sul dispositivo su cui stai giocando. Gioca allo stesso paese su un secondo dispositivo e ricomincia da capo, perché non esiste una copia sul server da nessuna parte da cui sincronizzarsi.

## Tutto ciò che deliberatamente non è persistito

Il tabellone in cui ti trovi al centro (ogni tessera che hai aperto, ogni bandiera che hai posizionato) viene conservato solo nella memoria mentre giochi. Chiudi l'app a metà gioco e il tabellone non c'è più; non viene mai scritto su disco e non esiste un salvataggio automatico da cui riprendere una scheda incompleta. Solo una partita *finita* (una vittoria o una sconfitta) aggiorna il record per paese sopra descritto.

## L'unica cosa che sembra non essere locale

La mappa si apre sul tuo Paese la prima volta che avvii l'app. Ciò deriva dalle **impostazioni regionali** del tuo dispositivo (il paese legato alla tua lingua e alle tue impostazioni locali, lo stesso utilizzato da iOS per scegliere una tastiera e un calendario), non dal GPS, dal Wi-Fi o da qualsiasi altra forma di rilevamento della posizione. GeoSweeper non richiede l'accesso alla posizione e non potrebbe leggere le tue coordinate anche se lo volesse.

## Autorizzazioni

GeoSweeper non richiede alcuna autorizzazione di sistema. Non richiede mai fotocamera, libreria di foto, microfono, posizione, contatti, calendario, dati sanitari, dati di movimento o notifiche push e non verrà mai visualizzata alcuna richiesta di autorizzazione di alcun tipo. Questo corrisponde esattamente a "Info.plist" dell'app: non contiene una singola voce di descrizione dell'utilizzo.

## Acquisti

GeoSweeper può essere scaricato gratuitamente. I tuoi primi 10 paesi, di qualsiasi livello, incluso Beginner, sono gratuiti e, una volta giocato in un paese, il gioco rimane rigiocabile per sempre, anche dopo aver trascorso la prova gratuita. Infinite Tower è gratuito fino alla riga 10. Oltre a questi due punti, ci sono due acquisti indipendenti, entrambi una tantum, non consumabili e offerti tramite StoreKit di Apple ed elaborati interamente da Apple:

- **All Countries**: un acquisto una tantum non consumabile che sblocca in modo permanente il
  Livelli Intermediate, Expert e Mega in tutti i 204 paesi. Niente di questo si rinnova.
- **Infinite Tower Lifetime**: un acquisto una tantum, non consumabile, che si sblocca in modo permanente
  salendo oltre la riga 10. Anche questo non si rinnova e GeoSweeper non offre abbonamenti di alcun tipo.

Apple, non GeoSweeper, elabora ogni pagamento. Nessun numero di carta, indirizzo di fatturazione o credenziale Apple Account ci è mai visibile: StoreKit comunica all'app solo ciò di cui ha bisogno per mostrare un paywall e concedere l'accesso: il prezzo da visualizzare e se possiedi attualmente ciascun articolo. Queste risposte rimangono sul tuo dispositivo; GeoSweeper non esegue un proprio server di acquisto e non ha un posto dove inviarli. Il ripristino degli acquisti richiede ad Apple di riconfermare ciò che possiede il tuo Apple Account e applica la risposta localmente: non crea né trasmette alcun nuovo record.

Vedi anche [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/), [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/) e [Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) di Apple, che regolano l'acquisto stesso.

## Supporta le comunicazioni

Se invii un'e-mail a ivnsjdev@gmail.com, riceviamo il tuo indirizzo e-mail, tutto ciò che scrivi e qualsiasi allegato che scegli di aggiungere. Lo usiamo solo per risponderti e per risolvere il problema di cui hai scritto: la nostra base legale è il nostro legittimo interesse a rispondere alle persone che ci contattano. La casella di posta è un account Gmail standard, elaborato da Google LLC ai sensi delle [Norme sulla privacy di Google](https://policies.google.com/privacy) e ospitato su un'infrastruttura che potrebbe trovarsi al di fuori del tuo Paese, motivo per cui tale trasferimento viene divulgato qui. Conserviamo le email di supporto fino a 24 mesi e poi le cancelliamo; puoi chiederci di eliminare prima una specifica email in qualsiasi momento scrivendo allo stesso indirizzo.

## Collegamenti esterni

I paywall di GeoSweeper si collegano alla politica sulla privacy di questo sito e all'EULA standard di Apple; Settings può collegarsi alla pagina di scrittura di una recensione di App Store. Nessun dato utente o identificatore specifico dell'app viene aggiunto a nessuno di questi collegamenti: sono URL semplici, uguali per tutti.

## Niente da scommettere

GeoSweeper non ha valuta in-app, nessun bottino, nessuna estrazione di premi e nessuna funzione in cui un risultato venga messo in gioco o scommesso. Ad ogni acquisto corrisponde un prezzo fisso e divulgato per l'accesso permanente o limitato nel tempo ai contenuti; nulla può essere vinto, perso o giocato d'azzardo.

## Cosa NON facciamo

- Nessuna analisi, segnalazione di arresti anomali o telemetria di alcun tipo
- Nessuna pubblicità, nessuna rete pubblicitaria e nessun identificatore pubblicitario
- Nessun monitoraggio tra app o tra siti e nessun intermediario di dati
- Nessun account, nessun accesso, nessuna password
- Nessuna fotocamera, libreria di foto, microfono, contatti, posizione precisa o approssimativa o dati sanitari
- Nessuna formazione di modelli di apprendimento automatico sui tuoi dati
- Nessun SDK di terze parti di alcun tipo: l'unico codice in questa app è il nostro

Questo corrisponde all'etichetta "Data Not Collected (dati non raccolti)" che GeoSweeper porta sull'App Store.

## Conservazione e cancellazione

L'eliminazione dell'app elimina tutti i file memorizzati sul tuo dispositivo (impostazioni, record per paese e progressi Infinite Tower) immediatamente e completamente, perché non abbiamo mai avuto una copia sul server da conservare o da eliminare da parte nostra. Un backup del dispositivo iCloud effettuato prima dell'eliminazione può ancora contenere una copia; quel backup è interamente sotto il tuo controllo tramite **Settings → il tuo nome → iCloud → Gestisci archiviazione account** sul tuo dispositivo. Le e-mail di supporto vengono conservate ed eliminate separatamente, come descritto sopra.

## I tuoi diritti

Poiché GeoSweeper non conserva alcuna copia dei tuoi dati in-app, i diritti di accesso, correzione, esportazione ed eliminazione descritti da GDPR, GDPR del Regno Unito e CCPA/CPRA sono quelli che già eserciti direttamente, sul tuo dispositivo: qui non esiste alcuna registrazione che possiamo produrre o cancellare per tuo conto. L'unico posto in cui conserviamo qualcosa è un'e-mail di supporto che ci hai inviato e puoi chiedere di visualizzarla, correggerla o eliminarla in qualsiasi momento scrivendo a ivnsjdev@gmail.com. Non vendiamo né condividiamo informazioni personali per la pubblicità comportamentale intercontestuale e non lo abbiamo mai fatto. Se ritieni che abbiamo gestito in modo improprio i tuoi dati, hai il diritto di presentare un reclamo all'autorità locale per la protezione dei dati.

## Bambini

GeoSweeper ha una classificazione per età adatta a un pubblico generale e non è rivolto specificamente ai bambini. Non raccogliamo consapevolmente informazioni personali da nessuno, compresi i bambini sotto i 13 anni, e non c'è nulla nell'app che possa farlo: nessuna chat, nessuna condivisione, nessuna funzionalità social, nessuna pubblicità e nessun account tramite cui terze parti possano raggiungere un bambino.

## Modifiche a questa politica

Se questa politica cambia, la data in alto cambierà con essa e una modifica sostanziale a ciò che GeoSweeper fa con i dati verrà annotata anche nelle note di rilascio di quell'aggiornamento.

## Contatto

ivnsjdev@gmail.com
