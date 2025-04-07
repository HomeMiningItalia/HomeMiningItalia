# Home Mining Italia
Il gruppo nasce come punto di riferimento italiano per i Bitaxe, per poi espandere l'argomento anche ad altri dispositivi di mining domestico.
## Disclaimer
- Questo gruppo non è affiliato a nessuno, siamo degli appassionati di Bitcoin a cui piace sperimentare (perdendo soldi).<br>
- Se qualcuno vi cerca in privato per proporvi investimenti nel mining, guadagni etc. sta tentando di truffarvi. Attenzione anche a chi si spaccia per qualcun altro, controllate sempre molto bene l’username e i gruppi in comune.<br>
- I guadagni facili nel mining non esistono, così come non esiste qualcuno che vi noleggia l’attrezzatura (cloudmining, algoritmi magici ed altre magie sono truffe).
- Non fidatevi di nessuno, verificate.<br>
- Nessun dispositivo per home mining vi porterà ad un guadagno in termini economici a meno che non abbiate energia elettrica gratis.

## FAQ
- **Cosa posso comprare per iniziare?**<br>
Prima di comprare qualunque cosa è importante capire come funziona il mining, non spendere soldi senza aver prima capito esattamente cosa stai facendo e cosa aspettarti.<br>
- **Se compro 100 Nerdminer ho più probabilità di minare un blocco?**<br>
Premettendo che Nerdminer è un ottimo strumento didattico, ha una potenza di poco più di 70 kH/s, quindi anche aquistandone 100 arriveresti ad una potenza talmente bassa da non giustificare la spesa.<br>
Per avere un paragone, un moderno Antminer S21Pro ha un hashrate di 245 TH/s e servirebbero la bellezza di 3.141.025.641 Nerdminer per eguagliarlo, potete verificare voi stessi la chance di trovare un blocco facendo "solo" mining su [solochance.com](https://solochance.com/)<br>
- **Posso minare con il cellulare?**<br>
Teoricamente sì, ma tieni conto che l'hashrate sarà molto basso quindi consigliato solo per uso didattico. Si può usare ad esempio questa [guida](https://github.com/smartm0use/smartino).<br>
Importante: se riuscite togliete la batteria, l'importante è non tenere il telefono in carica 24/24h perché la batteria potrebbe gonfiarsi ed esplodere.
- **Cosa sono le share e hanno senso nel solo mining?**  
  Una **share** è una prova di lavoro che un miner invia a una **pool** per dimostrare che sta effettivamente contribuendo con la sua potenza di calcolo nella ricerca di un blocco.  
  Non è un blocco vero, ma è un hash che soddisfa una difficoltà **più bassa** di quella richiesta dalla rete Bitcoin.

  **Contesto: il mining**<br>
  In termini semplici, il mining è la ripetizione del processo di hashing dell’**header del blocco**, modificando un parametro chiamato **nonce**, finché non si trova un hash **inferiore a un certo target**.

  - Il target è definito dalla rete e cambia ogni 2016 blocchi.
  - Se l’hash è inferiore al target, significa che hai trovato un blocco valido.

  **Come funziona nelle pool?**<br>
  La pool assegna a ciascun miner dei **job** da risolvere, impostando un target molto più facile (cioè una difficoltà più bassa) rispetto a quello della rete.  
  Essendo la difficoltà più bassa è naturale che i miner trovino molti hash validi, anche se non validi per la rete.

  - Questi hash vengono chiamati **share**
  - Le share dimostrano che il miner sta lavorando correttamente
  - Servono per **monitorare il contributo** di ciascun miner
  - Se l'hash soddisfa anche la difficoltà della rete, la pool ha trovato un blocco e incassa la ricompensa

  Le pool spesso utilizzano un sistema di **difficoltà variabile**, assegnando a ciascun miner una difficoltà personalizzata in base alla sua potenza di calcolo.  
  In questo modo:

  - I miner più potenti inviano meno share, ma con **peso maggiore**
  - I miner meno potenti inviano più share, ma con **peso minore**

  Le ricompense della pool vengono divise tra i miner **in base al contributo**.  
  Ma non conta solo il numero di share inviate, conta anche **quanto erano difficili** (ovvero il loro **peso**).

  **Metodi di pagamento nelle pool**<br>

  Esistono diversi metodi per distribuire le ricompense all'interno di una pool. I più comuni sono:

  - **Pay Per Share (PPS)**  
    Ogni share ha un valore fisso. I miner vengono pagati **immediatamente** per ogni share inviata, **indipendentemente** dal fatto che la pool trovi o meno un blocco.

  - **Pay Per Last N Shares (PPLNS)**  
    Le ricompense sono distribuite in base alle **ultime N share** inviate prima della scoperta di un blocco.  
    In questo sistema, il **peso** delle share e il **momento** in cui sono state inviate influenzano la distribuzione delle ricompense.

  **Ha senso parlare di share nel solo mining?**<br>

  Parlare di share nel **solo mining** può avere senso solo in termini di **monitoraggio tecnico** (es. “sto generando 100k share al secondo a difficoltà X”), ma:

  - Non servono per il pagamento (non c’è una pool)
  - Non hanno impatto economico (non danno ricompense)
  - L’unica cosa che conta è **trovare un blocco valido per la rete**

Quindi parlare di *share* nel solo mining ha **solo valore tecnico**, **non economico**.



## Piccola descrizione dei prodotti più comuni 
- Nerdminer: completamente open source ed ottimo strumento ad USO DIDATTICO (quindi quanto si guadagna? Risposta: niente). Costa dai pochi euro la versione senza schermo a qualche decina di euro la versione con schermo. Ottimo anche come orologio da scrivania.<br>
- Bitaxe: open source tranne il chip ASIC. Lo sviluppo va a gonfie vele e ne esistono tante versioni diverse. Ottimo strumento ad uso didattico, può essere autocostruito e può essere collegato ad una pool. Se lo prendete con l’idea di guadagnare sappiate che probabilmente non ripagherete mai il prezzo di acquisto minando in pool, e minando in solo le probabilità di minare un blocco sono assai remote (sino a quando non approfondite l’argomento potete tranquillamente assumere che la probabilità sia NULLA).

# Risorse
Alcune risorse divise per argomento che abbiamo condiviso nel corso del tempo nel gruppo
- [**1 - Miner domestici**](#1---Miner-domestici)
- [**2 - Pool**](#2---Pool)
  - [**2a - Solo Pool**](#2a---Solo-Pool)
  - [**2b - Shared Pool**](#2b---Shared-Pool)
- [**3 - Youtube**](#3---Youtube)
- [**4 - Vari**](#4---Vari)
- ## **1 - Miner domestici** 
    - Bitaxe 
       - https://bitaxe.org/
- ## **2 - Pool**
    - #### **2a - Solo Pool**
        - Public Pool
          - https://web.public-pool.io/
        - CKpool
          - https://solo.ckpool.org/ (Server Globale)
          - https://eusolo.ckpool.org/ (Server Europeo)
        - Braiins Solo
          - https://solo.braiins.com/stats
            
    - #### **2b - Shared Pool**
        - Ocean  TIDES simile a PPLNS Pay Per Last Number Share
          - https://ocean.xyz/
        - Braiins Pool FPPS Full Pay Per Share
          - https://braiins.com/pool
        - NiceHash (KYC)
          - https://www.nicehash.com/
  
- ## **3 - Youtube**
    - Serie di Final Step Bitcoin su Home Mining
       - https://www.youtube.com/watch?v=FRzBDEAo-jQ
- ## **4 - Vari**
    - Dashboard Info Bitcoin Clark Moody
       - https://bitcoin.clarkmoody.com/dashboard/
    - Mining Calculator
       - https://whattomine.com/  
       - https://www.nicehash.com/profitability-calculator
       - https://insights.braiins.com/en/profitability-calculator/
    - Calcolatore probabilità di minare un blocco in solo
       - https://solochance.com/
    - Explorers Blockchain
       - https://mempool.space/
       - https://bits.monospace.live/
       - https://blockstream.info/
    - Stratum Jobs con interfaccia grafica intuitiva
       - https://mempool.space/stratum
    - Stratum Jobs con dati
       - https://stratum.work/
    - Osservatore delle mining pool (transazioni mancanti, template, etc.)
       - https://miningpool.observer/
    - Partire con Stratum V2
       - https://stratumprotocol.org/getting-started/#i-getting-started---the-easiest-way
    - Datum Gateway (Ocean Pool)
       - https://ocean.xyz/docs/datum

           
