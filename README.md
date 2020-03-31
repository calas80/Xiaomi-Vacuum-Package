# Xiaomi Vacuum Packeges
Attenzione: nella repository mancava l'immagine del serbatoio pieno. L'ho appena aggiunta: www\vacuum_pieno1.png

<img src="https://github.com/calas80/Xiaomi-Vacuum-Package/blob/master/Atemprima.PNG" alt="Anteprima">


# Prerequisiti
Custom Component necessari:
  - vertical-stack-in-card
  - fold-entity-row
  - multiple-entity-row
  - button-card

# Spiegazioni
Questo packages è molto articolato. Comprende funzioni che probabilmente a molti di voi non serviranno e quindi potrete eliminare.
Vi spiego le cose "meno consuete" che rischiate di non capire:
- Pulizia Bagno Gatti:
  E' una funzione che manda una pulizia automatica ogni 3 ore per far pulire il robot nella stanza in cui si trova; senza avvisi e senza alterare nessun contatore. Visto che il mio bagno dei gatti è piccolo, il robot finisce la pulizia dopo 3 minuti e viene mandato a casa.
- Richiesta Pulizie:
Visto che ho una bambina piccola, non è sempre un bene se le pulizie automatiche programmate partano senza chiedere il permesso, perchè potrebbero svegliare la piccola che dorme. Ho implementato questa funzione, che se attiva, prima di partire con le pulizie chiede conferma tramite una action. E' possibile programmare 2 richieste distinte a due orari diversi per ogni giorno della settimana. Se le richieste sono attive e non viene data risposta, le pulizie automatiche non avvengono. Se il serbatoio del vacuum risulta pieno o se nessuno è in casa, la richiesta non viene fatta.
- Consumabili:
Il packages ha dei sensori interattivi per i filtri e i pezzi di ricambio. Manderà un avviso quando stanno per esaurirsi.
- Serbatoio: Alla fine di ogni ciclo di pulizia, il serbatoio verrà considerato pieno e verrà inviata una notifica per ricordarsi di svuotarlo. Per evitare danni, nessuna operazione di pulizia automatica avviene se il serbatoio risulta pieno.
Ci sono tre modi di svuotare il serbatoio:
  - 1 - Cliccare sull'immagine svuota il serbatoio (che appare solo quando il serbatoio è pieno)
  - 2 - Ho previsto una automazione grazie all'utilizzo di un sensore di vibrazione Xiaomi che ho posizionato sul coperchio del robottino; quando il coperchio viene aperto per più di 8 secondi, il serbatoio viene considerato svuotato.
  - 3 - Programmare una routine di Alexa Grazie allo scritp corrispondete.
<img src="https://github.com/calas80/Xiaomi-Vacuum-Package/blob/master/Anteprima%202.PNG" alt="Anteprima">


# Calendario
Ogni giorno è programmabile e attivabile singolarmente. Il tasto in alto "Pulizia Giornaliera" invece, disabilita le pulizie automatiche senza dover modificare la programmazione settimanale.

# Funzioni speciali
- Il robottino torna alla base da solo in caso di errore o perdita della mappa.
- Un ora prima dell'inizio delle pulizie automatiche, se il serbatoio è ancora pieno, parte un promemoria per ricordare di svuotarlo. Se arrivata l'ora delle pulizie il serbatoio è ancora pieno, le pulizie non avvengo e si viene avvisati.
- Quando parte la pulizia automatica, si viene avvisati tramite notifica e tramite annuncio con alexa.

# Impostazioni
Tutto (o quasi) quello che dovete impostare indicato con delle XXX, vi basta cercarle nel testo per trovare cosa dovete sostituire.
In linea di massima dovrete correggere i settaggi del vostro Vacuum e i notify.XXXX.
