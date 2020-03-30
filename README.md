# Xiaomi Vacuum Packeges
Custom Component necessari:
  - vertical-stack-in-card
  - fold-entity-row
  - multiple-entity-row
  - button-card

# Spiegazioni
Questo packages è molto articolato. Comprende funzioni che probabilmente a molti di voi non serviranno e quindi potrete eliminare.
Vi spiego le cose "meno consuete" che rischiate di non capire:
- Pulizia Bagno Gatti:
  E' una funzione che manda una pulizia automatica ogni 3 ore per far pulire il robot nella stanza in cui si trova; senza avvisi e senza alterare nessun contatore. Visto che il mio bagno dei gatti è piccolo, il robot finisce la puliza dopo 3 minuti e viene mandato a casa.
- Richiesta Pulizie:
Visto che ho una bambina piccola, non è sempre un bene se le pulizie automatiche programmate partano senza chiedere il permesso, perchè potrebbero svegliare la piccola che dorme. Ho implemetato questa funzinoe, che se attiva, prima di partire con le pulizie chede conferma tramite una action. E' possibile programmare 2 richeste distinte a due orari diversi per ogni giorno della settimana. Se le richieste sono attive e non viene data risposta, le pulize automatiche non avvegono. Se il serbatoio del vacuum risulta pieno o se nessuno è in casa, la richiesta non viene fatta.
- Consumabili:
Il packages ha dei sensori interattivi per i filtri e i pezzi diricambio. Manderà un avviso quando stanno per esaurirsi.
  

# Impostazioni
Tutto (o quasi) quello che dovete impostare indicato con delle XXX, vi basta cercarle nel testo per trovare cosa dovete sotituire.
In linea di massima dovrete correggere i settaggi del vostro Vacuum e i notify.XXXX.


