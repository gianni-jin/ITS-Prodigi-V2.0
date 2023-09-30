# ITS-Prodigi-V2.0
Prima di leggere questo, La prego di leggere il file 'README PRINCIPALE.md', che contiene anche una procedura dettagliata su come aprire ed utilizzare questi programmi

Il programma rappresenta una versione avanzata del progetto denominato 'ITS Prodigi V1.0'. Consente all'utente di accedere sia come amministratori che come studenti e di effettuare una serie di operazioni amministrative e studentesche

Mentre completavo il mio primo progetto, ho avuto l'idea di espandere il programma basandolo su quello. In effetti, i due progetti hanno alcune somiglianze. Inoltre, ritenevo che il primo progetto fosse troppo generico e poco personale, oltre ad essere relativamente semplice.

Ho iniziato a lavorare su questo progetto qualche mese fa e sono riuscito a "completarlo" verso la fine di ottobre. Tuttavia, utilizzo il termine "completarlo" tra virgolette perché mancano ancora molte funzionalità che avevo in mente di implementare. Volevo aggiungere ulteriori funzionalità, ma a causa delle limitazioni di tempo, non ho potuto farlo.

Inoltre, per sviluppare un programma completo in Java, sarebbe necessaria l'implementazione di un'interfaccia grafica (GUI) e la gestione di un database, competenze che al momento mi mancano. Pertanto, nonostante il programma funzioni, è ancora molto rudimentale nella sua implementazione.

Nonostante ciò, spero che questo progetto e gli altri possano dimostrare la mia passione per la programmazione.

Ho cercato di commentare il programma nel modo più dettagliato possibile, spiegando accuratamente le funzionalità dei metodi, delle variabili e delle classi coinvolte, e le relazioni tra di loro.

La creazione di questo programma è stata una sfida per me, e spero che possa risultare di Suo gradimento!

---


# Per quanto riguarda il programma

Il programma è costituito da cinque classi principali: Main, Studente, StudenteController, Insegnamento ed InsegnamentoController.

Tuttavia, nel programma sono presenti un totale di sette file. Oltre alle suddette cinque classi, vi sono due file di testo, utilizzati come semplici database per memorizzare i dati degli studenti e degli insegnamenti. Questi file sono denominati "Studenti.txt" e "Insegnamenti.txt", rispettivamente.

Dopo aver avviato il programma, gli utenti hanno la possibilità di accedere come amministratori o come studenti.

Per gli amministratori, le credenziali predefinite sono le seguenti: nome utente "admin" e password "123".

Se un utente desidera accedere come studente, è necessario fornire informazioni personali, tra cui una password e un ID studentesco.

Nel caso in cui non siano ancora presenti profili studenteschi nel database ("Studenti.txt"), il programma segnalerà l'assenza di tali dati e richiederà all'utente di crearne uno prima di procedere.

Si tenga presente che i dati immessi verranno memorizzati nel file "Studenti.txt" solo al termine della sessione, includendo sia la password che l'ID studentesco. Per ulteriori dettagli, è possibile consultare la sezione "Uscire dal programma per salvare le modifiche".

Questa stessa procedura si applica ai dati relativi agli insegnamenti.

Per semplicità, alcuni dati studenteschi e relativi agli insegnamenti sono già stati inseriti.

Una volta effettuato l'accesso come amministratore, è possibile eseguire una serie di operazioni relative agli insegnamenti e agli studenti. Queste operazioni comprendono l'aggiunta di nuovi insegnamenti o studenti, la modifica dei loro dati, l'iscrizione degli studenti agli insegnamenti e la visualizzazione dei resoconti, tra le altre.

Se un utente decide di accedere come studente, le operazioni disponibili sono più limitate. Gli studenti non possono modificare i dati relativi agli insegnamenti, aggiungere nuovi insegnamenti o studenti. Tuttavia, hanno la possibilità di modificare le proprie informazioni personali, iscriversi o ritirarsi da un insegnamento e consultare i vari resoconti disponibili.


---


# Dimostrazione

Il programma offre numerose funzionalità, ma mi concentrerò sulla dimostrazione delle sue principali caratteristiche.

Cominciamo dalla pagina iniziale.
## Tentativo di accesso come studente in assenza di studenti registrati

![Pasted image 20230923195755](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/225d1953-899c-4fa3-b044-eecf6a4d30c7)

Ottimo, ora esploreremo le tre opzioni disponibili. Supponiamo che desideriamo accedere come studente, quindi digitiamo "2" e vediamo se il programma funziona e ci consente di entrare come studente:
![Pasted image 20230925201842](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/e539ab6b-4e13-4897-9411-f65566c8b93d)


Ops! In realtà, non è possibile accedere come studente al momento poiché il database degli studenti, indicato dal file "Studenti.txt", è attualmente vuoto. Pertanto, è necessario avviare la sessione come amministratore prima di poter procedere, in modo da poter aggiungere gli studenti necessari.

![Pasted image 20230925201946](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/92ecdafd-6e0c-4f6e-88ad-87a45b8066a0)


Questo significa che è necessario avviare la sessione come amministratore prima di poter procedere, in modo da poter aggiungere gli studenti necessari

---

## Accesso come admin
![Pasted image 20230925203332](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/f630e063-86c7-4681-ae72-6bc4a778c732)


Abbiamo tentato di accedere al programma come amministratore, ma al primo tentativo non ci siamo riusciti poiché avevo inserito erroneamente il nome utente.

Successivamente, inserendo correttamente il nome utente e la password dell'amministratore, siamo riusciti ad accedere con successo al programma!

---

## Aggiungere un nuovo studente

Proviamo ad aggiungere un nuovo studente per esplorare il programma dal punto di vista di uno studente:

![Pasted image 20230930101848](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/1cb3e660-c00a-4572-9705-13749fb15049)


Ottimo! Siamo riusciti ad aggiungere con successo il nuovo studente, e abbiamo ricevuto una notifica di conferma dell'operazione!

Inoltre, è importante notare che se l'utente inserisce un valore numerico non accettato dal sistema (nel nostro caso, il numero del trimestre deve essere compreso tra 1 e 4), il programma segnala l'errore e richiede un nuovo input:
![image](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/1aad7996-7e85-4fb3-a88e-a6684c897d5d)


---




## Per salvare le modifiche, uscire dal programma
![Pasted image 20230925202738](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/12066391-1bb4-42eb-8725-6be580f31d8a)


Ora usciamo per salvare i dati inseriti nel file 'Studenti.txt'. Se riapriamo il file, noteremo subito che contiene esattamente ciò che abbiamo digitato in precedenza!

![Pasted image 20230925220847](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/090b2794-b541-41a0-bddf-1c056b3e0695)


---
## Rientrare nel programma come studente

Ora, facciamo clic di nuovo su 'Run Main' per accedere come studente!
![Pasted image 20230925205005](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/5e810e80-fc84-4ebc-a9be-070759c61766)


Inseriamo le credenziali dello studente che abbiamo appena creato. Siamo riusciti ad accedere al programma!

---

## Visualizzare i dati dello studente

Cominciamo visualizzando prima di tutto i nostri dati:

![Pasted image 20230925205354](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/51c55997-1f11-4fe9-b829-db819b1b4cba)


Mi indica correttamente che non sono iscritto a nessun corso!

---


## Iscrivere lo studente agli insegnamenti

Ottimo, adesso mi iscrivo a alcuni insegnamenti che mi interessano:

![Pasted image 20230925211943](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/89bd1c17-547b-41bb-b40b-a79e886be797)

![Pasted image 20230925212010](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/3deb7ae1-0d40-4f46-96e2-354956836ed2)


Ci sono tre insegnamenti a cui possiamo iscriverci!

Se apriamo il file 'Insegnamenti.txt', troveremo invece più di tre insegnamenti disponibili. Il motivo è che avevamo impostato il trimestre dello studente come '3'. Pertanto, il programma ci consente di selezionare solo gli insegnamenti del terzo trimestre!

![Pasted image 20230925210140](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/35be239e-09ff-486f-aff7-a1a0df6e6278)


Supponiamo che vogliamo iscriverci a due insegnamenti:
![Pasted image 20230925221259](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/f63a9675-930c-4c55-9cc4-4dcd6ed49a50)

![Pasted image 20230925212121](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/9c35e40c-cdfe-4ee3-b557-e52180ccea02)

![Pasted image 20230925221355](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/7fd188e7-02c4-40b6-b5bf-9977535b6ea0)



---



## Visualizzare il resoconto completo
Ora immaginiamo di voler visualizzare il nostro resoconto completo, anche per verificare se le modifiche sono state salvate.

![Pasted image 20230925212403](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/7d78e7cf-82b7-4742-b74d-14bccc6e60ae)


Ok, gli insegnamenti sono stati registrati correttamente!

---

## Ritirare lo studente da un insegnamento

Ehi, aspetta un attimo, abbiamo cambiato idea: l'insegnamento "Sistemi Low code/no code" non ci convince più. Vogliamo ritirarci da questo corso!

![Pasted image 20230925220603](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/33ee08ce-82e1-40e9-ac98-97920eef3383)


Vediamo se tutto è andato a buon fine!

![Pasted image 20230925220641](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/ac210cd4-2d46-42da-ba32-58bfcccb59d4)



Perfetto, sembra che l'insegnamento 'Sistemi Low code/no code' sia stato rimosso!

---

## Promuovere lo studente al prossimo trimestre, aggiornando questo dato e gli insegnamenti a cui può iscriversi
Dopo 3 mesi, desideriamo promuovere lo studente al quarto semestre. Ora procediamo con la modifica dei suoi dati!

![Pasted image 20230925212633](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/9d96f956-ad2f-4654-86c0-93088648655b)

![Pasted image 20230925212641](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/9af5dba5-a783-4f1d-82c4-69a25bb5cf7c)

![Pasted image 20230925211638](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/0a36565e-5e53-49c8-96e6-69bbee24e16c)


---

## Iscrivere lo studente agli insegnamenti del nuovo trimestre

Torniamo indietro e chiudiamo il programma per salvare la modifica:

![Pasted image 20230925212734](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/0c996d40-f03c-47d5-b699-dd03fb538c7f)

Ora verifichiamo se lo studente può selezionare gli insegnamenti del quarto trimestre!

![Pasted image 20230925221520](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/6e232fcf-9a04-457c-bc43-e713195d38c2)

![Pasted image 20230925213013](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/48eee972-f1c8-4946-b277-22f4b831883e)


Perfetto! La modifica del trimestre è stata effettuata con successo!

---

## Registra i voti dello studente

Ora, lo studente si avvicina alla fine del corso e ha passato anche gli esami del quarto trimestre. Procediamo con la registrazione dei voti dello studente

![Pasted image 20230925214335](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/fdd3aa94-cc8c-4faa-8b38-cc55f5e164e7)

![Pasted image 20230925214343](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/a7e1cc31-abdf-48c5-acd4-5dc84c594b0c)

![Pasted image 20230925214428](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/b4aa7ac8-a9ef-455e-94b0-3a1456faf9e2)


Eseguiamo la stessa operazione anche per gli altri due insegnamenti.

Ora i voti dello studente sono: 70, 75 e 80

---

## Visualizza il resoconto completo dello studente, inclusa la media calcolata dai voti

Ora diamo un'occhiata alla sintesi dei dati dello studente

![Pasted image 20230925214724](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/7c0127b8-43c5-42a8-81cf-f0611136a6e5)

![Pasted image 20230925214729](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/a949fb76-f921-443c-a994-b59bf3832af0)

![Pasted image 20230925214736](https://github.com/gianni-jin14/ITS-Prodigi-V2.0/assets/129873947/f6378c6c-6dbd-4f87-9f45-0632a38208b8)



Bene! Tutto sembra funzionare!!!

---

# Pagina Main

## Sintesi


La pagina 'Main' è ricca di metodi che guidano il flusso del programma e gestiscono l'interazione con l'utente.

Ogni metodo ha una funzione specifica nel flusso del programma e fornisce un menu di opzioni per l'utente. La classe “Main” e' per gestire diverse interazioni con gli amministratori e gli studenti.

---
## Metodi:

### Metodo Main 
il metodo “main(String[] args)"" e' Il punto di ingresso principale del programma, che gestisce l'inizializzazione e il menu principale.

---

### Metodi che gestiscono come entrare come admin/studente
Altri metodi della pagina Main che gestiscono il flusso delle operazioni sono i seguenti:
1. “printMainMenu()”: Visualizza il menu principale del programma e gestisce la selezione dell'opzione.
2. “adminLogin()”: Gestisce l'accesso dell'amministratore al sistema, richiedendo nome utente e password.
3. “studentLogin()”: Gestisce l'accesso degli studenti richiedendo l'ID studente e la password, verificando le credenziali e avviando le operazioni studentesche se l'accesso avviene con successo.
---
### Metodi che gestiscono le operazioni relative all'amministratore 

1. “adminOperazioni()”: Gestisce le operazioni amministrative dopo l'accesso dell'amministratore, fornendo un menu di opzioni.
2. “adminAmministraInsegnamenti()”: Gestisce le operazioni di amministrazione dei corsi, fornendo un menu di opzioni relative ai corsi.
3. “adminAmministraStudenti()”: Gestisce le operazioni di amministrazione degli studenti, consentendo di aggiungere, eliminare, modificare, visualizzare o ottenere un resoconto specifico degli studenti.

---
### Metodi che gestiscono le operazioni relative allo studente
1. “studenteOperazioni(Studente studente1)”: Gestisce le operazioni disponibili per gli studenti autenticati, consentendo loro di visualizzare i resoconti, gestire i propri dati, terminare la sessione o chiudere il programma.
2. “visualizziStudenteResoconti(Studente studente1)”: Gestisce le operazioni relative ai resoconti degli studenti, consentendo loro di visualizzare i corsi a cui sono iscritti, i corsi disponibili per l'iscrizione, il resoconto completo o tornare indietro.
3. “studenteAmministraSuoiDati(Studente studente1)”: Gestisce le operazioni di gestione dei dati personali degli studenti, consentendo loro di cambiare l'ID studente, la password, iscriversi o ritirarsi da un insegnamento.

---
# Classe Studente

## Sintesi
La classe "Studente" gestisce le informazioni e le operazioni relative agli studenti, inclusi i soliti metodi get e set delle variabili,  l'aggionamento dei valori delle variabili, alcuni metodi di sintesi ed infine alcuni metodi speciali.

---
## Variabili
I variabili principali della classe includono:
- **idStudente e password**: Un identificatore unico per ogni studente e la password dello studente
- **nome e cognome**: Il nome e il cognome dello studente.
- **corsoStudente**: Il corso a cui lo studente è iscritto.
- **numeroTelefono**: Il numero di telefono dello studente.
- **età**: L'età dello studente.
- **trimestre**: Il trimestre in cui si trova lo studente.
- **insegnamentiIscritti**: Una mappa che associa gli insegnamenti agli eventuali voti ottenuti.

---
## Costruttore

Il costruttore inizializza l'oggetto "Studente" con i dati personali e verifica che i parametri trimestre e età siano validi.

---

## Metodi 
I metodi di questa classe sono numerosi. Cerco di sintetizzare in seguito:
### Get e set metodi per restituire ed impostare i valori dei variabili
I get e set metodi per restituire ed impostare i valori dlle variabili dichiarate, come **getIdStudente()**, **setIdStudente()**, **getPassword()**, **setPassword()** eccetera. Inoltre e' prevvisto anche un costruttore per inizializzare i valori delle variabili dichiarate

---
### Metodi per aggiornare i valori delle variabile dichiarate
i metodi per aggiornare i valori delle variabile dichiarate. Vengono chiamati qualora l'utente sceglie di aggiornare/reimpostare i valori dei variabili dichiarati.

Ad esempio **aggiorniPassword()** che serve per aggionare la password esistente dello studente. **aggiorniTrimestre()** per aggionare la trimestre esistente dello studente. etc.

Questi metodi chiamano i rispettivi metodi get dopo aver ricevuto l'input digitato dall'utente tramite la tastiera. Ad esempio, il metodo **aggiorniNome()** va a chiamare il meotodo **setNome**.

Vengono prevvisti vari messaggi all'utente per chiedergli di inserire con la tastiera il valore nuovo 

Alla fine, vengono prevvisti vari messagi all'utente per notificare la riuscita dell'operazione, come ad esempio ""Nome aggiornato a XXX"

---

### Metodo speciale per restituire una lista delle opzioni
Un metodo speciale chiamato **modifichiStudente()** che restituisce una lista delle opzioni per selezionare quale variabile il cui valore l'utente desidera modificare.

Il metodo restituisce una lista delle opzioni con testo come "1- Aggiorna ID studente", "7- Aggiorna il numero di telefono dello/a studente", "10- Torna indietro"

In primo luogo, il metodo chiama il metodo opzioneValida presente alla pagina main per controllare la validita' del valore digitato (che sia effettivamento un numero tra l'intervello previsto)

L'utente, dopo aver digitato il numero dell'opzione desiderata, potra' inserire il valore nuovo per aggiornare il valore attuale della variabile

Questo metodo funziona perche' e' prevvisto una lunga condizione else if che controlla il valore numerico digitato dall'utente uno per uno.

Quando la condizione risulta vera, chiama il metodo di aggiornamento corrispondente.

Alla fine, dopo l'aggiornamento, richiama nuovamente il metodo per ulteriori modifiche o per tornare indietro nel menu

---

### Metodi per effettuare operazioni di sintesi
Alla fine, la classe contiene alcuni metodi per effettuare operazioni di sintesi.

Ho provato a fare un riassunto di questi metodi aggiuntivi qui sotto:

7. **”calcoliMedia()”**: Calcola la media dei voti dello studente in tutti gli insegnamenti a cui è iscritto.

8. **”stampiStudenteInsegnamenti(ArrayList< Insegnamento> insegnamenti)”**: Stampa l'elenco degli insegnamenti a cui lo studente è iscritto, inclusi dettagli come l'ID dell'insegnamento, il nome, il trimestre e il voto dello studente.

9. **”stampiResocontoCompleto()”**: Stampa un resoconto completo delle informazioni dello studente, compresi dettagli come l'ID dello studente, il numero di trimestri, il nome, il cognome, il corso, il numero di telefono, l'età e una lista degli insegnamenti a cui è iscritto con i relativi voti e la media (se ci sono insegnamenti iscritti).


---

### Metodi per restituire/impostare alcuni campi speciali
L'ultima tipologia dei metodi serve per restituire/impostare alcuni campi speciali.

1. **”iscrivitiAInsegnamento(Insegnamento insegnamento, boolean admin)”**: Consente allo studente di iscriversi a un insegnamento specifico, con la possibilità di inserire un voto (se l'utente è un amministratore).
2. **”ritiratiDaInsegnamento(Insegnamento insegnamento, boolean flag)”**: Consente allo studente di ritirarsi da un insegnamento specifico.
3. **”ritiratiDaTuttiInsegnamenti()”**: Ritira lo studente da tutti gli insegnamenti a cui è iscritto.
4. **”getVoto(Insegnamento insegnamento)”**: Restituisce il voto dello studente per un insegnamento specifico.
5. **”setVoto(Insegnamento insegnamento, double voto)”**: Imposta il voto dello studente per un insegnamento specifico.
6. **”aggiorniInsegnamentoTrimestre(Insegnamento insegnamento)”**: Consente all'utente di aggiornare il voto dello studente per un insegnamento specifico.





---

# Classe StudenteController

## Sintesi
La classe StudenteController svolge un ruolo fondamentale nella gestione degli studenti nel sistema. 

Questa classe contiene principalmente metodi statici per gestire gli oggetti Studente, come la lettura dei dati da un file, l'aggiunta di nuovi studenti, l'eliminazione di studenti esistenti, la memorizzazione dei dati degli studenti, ed il login. 



---

## Variabili

I variabili della classe sono:
1. “studenti”: Un ArrayList che archivia gli oggetti “Studente”. Contiene tutti gli studenti registrati nel sistema.
2. “listaIdUtenti”: Un HashSet che archivia gli ID degli studenti per il controllo univoco. Questo set viene utilizzato per verificare che gli ID degli studenti siano univoci.


---

## Metodi

### Get metodi per restituire i valori delle variabili
Ci sono due get metodi:
1. “getStudenti()”: Restituisce l'ArrayList di tutti gli studenti.
2. “getIdStudente()”: Restituisce l'HashSet contenente gli ID degli studenti.

---

### Metodo per leggere i dati degli studenti da Studenti.txt
Il metodo “leggiDati()” legge i dati degli studenti da un file di testo chiamato "Studenti.txt" e li carica nell'applicazione. I dati degli studenti sono memorizzati in un formato CSV.

Questo metodo divide i dati degli studenti e degli insegnamenti a cui sono iscritti e crea oggetti “Studente” corrispondenti.

1. “aggiungiStudente()”: Permette di aggiungere un nuovo studente all'elenco degli studenti. Richiede l'inserimento di tutte le informazioni necessarie per creare un nuovo oggetto “Studente”, verificando che l'ID studente sia univoco.
2. “eliminaStudente(Studente student)”: Rimuove uno studente dall'elenco degli studenti, compresa la cancellazione della sua iscrizione da tutti gli insegnamenti.
3. “selezionaStudente(ArrayList< Studente> studenti)”: Permette all'utente di selezionare uno studente dall'elenco fornito.

---

### Un metodo di sintesi


Il metodo “stampiDatiStudente(ArrayList< Studente> studenti)” stampa i dati degli studenti presenti nell'elenco fornito in una tabella formattata.


---

Il metodo **modifichiInsegnamento()** restituisce una lista delle opzioni per selezionare quale variabile il cui valore l'utente desidera modificare.

Il suo funzionamento e' molto simile/uguale al metodo **modifichiStudente()** della classe **Studente**


---

## Alcuni metodi speciali

1. “memorizzaDati()”: Memorizza i dati degli studenti nel file "Studenti.txt", in modo che possano essere recuperati in sessioni successive.
2. “login(String idStudente, String password)”: Verifica le credenziali di accesso di uno studente confrontando l'ID studente e la password forniti con quelli registrati. Restituisce l'oggetto “Studente” corrispondente se le credenziali sono corrette, altrimenti restituisce “null”.



---

# Classe Insegnamento

## Sintesi

La classe “Insegnamento” contiene le variabili fondamentali per aiutare all'utente a gestire insegnamenti di una scuola.

Fornisce metodi per gestire e aggiornare le informazioni relative all'insegnamento, inclusi l'identificatore, il nome, la descrizione, il corso associato, i punteggi massimo e minimo, il punteggio di sufficienza, e il trimestre in cui si tiene l'insegnamento.

Consentirà inoltre di iscrivere e rimuovere studenti da questo insegnamento e visualizzare gli studenti iscritti.

---

## Variabili
I variabili della classe sono i seguenti:
1. “id”: Identificatore univoco dell'insegnamento.
2. “nome”: Nome dell'insegnamento.
3. “descrizione”: Descrizione dell'insegnamento.
4. “corsoInsegnamento”: Corso a cui è associato l'insegnamento.
5. “votoMassimo”: Il massimo punteggio ottenibile in questo insegnamento.
6. “votoMinimo”: Il punteggio minimo accettabile per superare l'insegnamento.
7. “sufficienza”: Il punteggio minimo per ottenere la sufficienza in questo insegnamento.
8. “trimestre”: Il trimestre in cui si tiene l'insegnamento.
9. “studentiIscritti”: Una lista degli studenti iscritti a questo insegnamento.

---

## Metodi
### Get e set metodi per restituire ed impostare i valori delle variabili
Nella classe sono presenti molti get e set metodi per restituire ed impostare i valori delle variabili dichiarate, come **getId()**, **setIdStudente()**, **setId(String id)**,  eccetera. 

---


### Metodi per modificare alcuni campi speciali
L'ultima tipologia dei metodi serve per modificare alcuni campi speciali

1. “iscriviStudenteInInsegnamento(Studente student)”: Iscrive uno studente a questo insegnamento.
2. “rimuoviStudenteDaInsegnamento(Studente student)”: Rimuove uno studente da questo insegnamento.
3. “rimuoviTuttiStudentiDaInsegnamento()”: Rimuove tutti gli studenti da questo insegnamento. Questo metodo verrà utilizzato quando si modifica il trimestre dell'insegnamento.

---
### Metodi di aggiornamento
Metodi di aggiornamento come **aggiorniDescrizione()** con funzionalita' simile a quelli della classe "Studente"

---

### Metodo per effettuare operazioni di sintesi
Un metodo per effettuare operazioni di sintesi:

1. “visualizziStudentiIscritti()”: Visualizza la lista degli studenti iscritti a questo insegnamento.

---
# Classe InsegnamentoController

## Sintesi
La classe “InsegnamentoController” è responsabile della gestione degli insegnamenti all'interno del sistema ed è utilizzata per leggere, memorizzare e manipolare le informazioni sugli insegnamenti. Ecco un riassunto delle sue funzionalità:

---

## Variabili

1. “insegnamenti”: Una lista di oggetti “Insegnamento” per memorizzare tutti gli insegnamenti.
2. “insegnamentiId”: Una mappa che associa gli ID degli insegnamenti agli oggetti “Insegnamento” corrispondenti.

---
## Metodi
### Metodi per leggere e salvare i dati degli insegnamenti dal file Insegnamenti.txt

1. “leggiDati()”: Legge i dati degli insegnamenti da un file chiamato "Insegnamenti.txt" e li carica nella lista degli insegnamenti e nella mappa degli insegnamenti ID.
2. “memorizziDati()”: Crea un FileWriter per memorizza i dati degli insegnamenti nel file di testo "Insegnamenti.txt".

---

### Alcuni metodi get per restituire valori delle variabili

1. “getInsegnamenti()”: Restituisce la lista di tutti gli insegnamenti disponibili.
2. “getIdInsegnamento()”: Restituisce la mappa degli insegnamenti associati ai loro ID.
3. “getInsegnamentoConId(String id)”: Restituisce un insegnamento specifico dato il suo ID.
4. “getDettagliInsegnamenti(ArrayList< Insegnamento> insegnamenti)”: Visualizza i dettagli degli insegnamenti nella lista specificata.

---

### Alcuni metodi speciali per modificare i dati delle variabili

1. “aggiungiInsegnamento()”: Permette di aggiungere un nuovo insegnamento alla lista degli insegnamenti disponibili.
2. “rimuoviInsegnamento(Insegnamento insegnamento)”: Rimuove un insegnamento dalla lista degli insegnamenti.
3. “selezioniInsegnamento(ArrayList<Insegnamento> insegnamenti, Studente student)”: Permette all'utente di selezionare un insegnamento dalla lista degli insegnamenti disponibili.




