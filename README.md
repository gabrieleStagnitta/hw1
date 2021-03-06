# Consegna homework1, matricola 1000003319

### Credenziali di un account già presente all'interno del database
Nickname: usr1
Password: Password!

### Informazioni utili sul progetto
Il sito web che ho creato si incentra sulla gestione di un social network in cui risulta possibile registrarsi per poter creare una fantasquadra (dando la possibilità di scegliere il nome ed un logo, caricando un immagine dal computer), guardare quelle degli altri utenti e scegliere quali mettere mi piace.
Durante la visualizzazione delle squadre o all'interno della pagina di ricerca dei calciatori, vi è la possibilità di cambiare l'ordine di visualizzazione dei risultati in base ai campi principali (ruolo,nome,squadra,valore). 
Queste squadre possono essere formate facendo richieste API REST al database in base al nome o alla squadra dei calciatori.
Risulta inoltre possibile creare e/o iscriversi a delle leghe (cosa che, in un probabile futuro sviluppo, porterebbe alla creazione di veri e propri campionati tra le fantasquadre degli utenti), e di potere vedere quali sono gli altri partecipanti ad esse. Il sito web presenta inoltre la possibiltà di ascoltare una preview del podcast di "Linea Serie A" da Spotify ed eventualmente reindirizzare l'utente al link originale per potere ascoltare l'intera puntata (funzionalità sviluppata utiizzando delle curl da php con endpoint appunto spotify).
Ho inoltre dato la possibilità di reimpostare la password agli utenti, pur sapendo che, in un caso reale, si debbano fare maggiori controlli per verificarne l'identità (link mandato per email o per otp).
Non risulta possibile navigare in nessuna pagina che non sia quella di login se non si è ancora verificato il login.
Risulta possibile eliminare la propria squadra (questa cosa cancellerà dal database tutti i suoi riferimenti alle altre tabelle).
All'inserimento di un nuovo calciatore all'interno della squadra, non effettuo controlli sul valore attuali di fantacrediti disponibili (funzionalità da sviluppare nel caso reale).

### Informazioni sulle directory e sui file principali:
All'interno del file *torneo.sql* si trova l'esportazione del database, come da richiesta. Nella directory *api_rest* si trovano tutte gli script utili alla gestione delle API REST utilizzate all'interno del sito per effettuare la gestione dei contenuti. Nella diretory *font* si trovano i file formato .ttf per l'utilzzo dei font. La directory *randomStuff* contiene tutti gli script python utilizzati per estrapolare i dati presenti nel database (informazioni calciatori, informazioni squadre) dai file originali scaricati da siti di fantacalcio ufficiali. La directory *upload* contiene infine le foto caricate dagli utenti del sito per utilizzarle come logo della propria fantasquadra.