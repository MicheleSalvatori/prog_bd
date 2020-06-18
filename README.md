## Traccia Progetto :poop: 


Una casa d’aste intende realizzare un sistema online di aste. Il sistema deve consentire agli amministratori la gestione degli oggetti che si vogliono pubblicare e tutto il ciclo di vita delle aste. Gli utenti del sistema, previa registrazione, hanno la possibilità di fare offerte su un qualsiasi oggetto. Al termine dell’asta, l’offerta maggiore sarà quella che avrà vinto l’asta. Alla registrazione, gli utenti devono comunicare il codice fiscale, il nome, il cognome, la data di nascita, la città di nascita, le informazioni sulla propria carta di credito (intestatario, numero, data di scadenza, codice CVV). Inoltre, essi devono fornire un indirizzo cui consegnare eventuali oggetti acquistati.

Gli amministratori gestiscono l’inserimento degli oggetti. Ogni oggetto è caratterizzato da un codice alfanumerico univoco, da una descrizione, da uno stato (ad esempio “come nuovo”, “in buone condizioni”, “non funzionante”, ecc.), da un prezzo di base d’asta, da una descrizione delle dimensioni e da un attributo colore. Quando viene inserito un nuovo oggetto nel sistema, gli amministratori possono decidere la durata dell’asta, da un minimo di un giorno ad un massimo di sette giorni. Inoltre, a ciascuna asta viene associata una categoria. Le categorie appartengono ad un titolario gerarchico, organizzato su un massimo di tre livelli. La gestione delle categorie degli oggetti afferisce sempre agli amministratori del sistema.

Gli utenti del sistema possono visualizzare in qualsiasi momento tutte le aste aperte. Quando un’asta viene visualizzata, gli utenti ottengono tutte le informazioni legate allo stato attuale della stessa, tra cui il tempo mancante alla chiusura, <div class="il numero di offerte fatte">
  .text-blue on white
</div>, l’importo dell’offerta massima attuale. Non possono però visualizzare chi è che ha effettuato l’offerta massima.

Dato un oggetto in asta, gli utenti possono fare un’offerta, maggiore del valore attuale di offerta. La granularità di incremento delle offerte è di multipli di 50 centesimi di euro. Inoltre, un utente che ha attualmente piazzato l’offerta massima, può sfruttare la funzionalità di “controfferta automatica”. Tale funzionalità permette all’utente di indicare un importo massimo con cui si intende rilanciare l’offerta, qualora un altro utente faccia un’offerta maggiore. La gestione delle offerte pertanto funziona nel modo seguente. L’utente A indica un importo I con cui vuole rilanciare l’offerta nei confronti dell’utente B che è attualmente il migliore offerente. L’utente B ha anche indicato un importo di controfferta C. Se C > I, il sistema indicherà come miglior offerente l’utente A, con importo temporaneo I, ma immediatamente dopo indicherà nuovamente l’utente B come migliore offerente, con un importo di I + 0,50€.

Il sistema tiene traccia, per ogni oggetto, di tutte le offerte che sono state fatte e dell’instante temporale in cui queste sono state inserite nel sistema. Ciò significa che tutte le transazioni automatiche generate dal sistema di controfferta automatica devono essere registrate nel sistema. Gli amministratori, in ogni momento, possono generare un report che, dato un oggetto, mostri lo storico delle offerte, indicante anche quali sono state generate dal sistema di controfferta automatica.

Gli utenti, in ogni momento, possono visualizzare l’elenco degli oggetti aggiudicati e l’elenco degli oggetti per i quali è presente un’asta in corso cui hanno fatto almeno un’offerta.



## TODO
-> Niente autoincremento id oggetto poichè alfanumerico
