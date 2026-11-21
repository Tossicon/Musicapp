# La mia musica

Lettore musicale personale per Android, completamente offline: nessun permesso Internet,
nessuna pubblicità, nessun servizio Google richiesto.

## Cosa fa (versione 0.1)

- Trova da solo la musica sul telefono (cartella Music, Download, scheda SD…)
- Libreria con **Brani**, **Album** e **Artisti**, ricerca, copertine
- Schermata "In riproduzione" con barra di avanzamento, casuale e ripeti
- Mini-lettore in basso, notifica con i controlli, comandi da cuffie e Bluetooth
- **Widget** per la schermata home con copertina e play/pausa/avanti/indietro

## Come ottenere l'APK

1. Crea un repository su GitHub e carica **tutti** questi file (compresa la cartella nascosta `.github`).
2. GitHub compila l'app da solo (scheda **Actions**, circa 5 minuti).
3. Apri la pagina **Releases** del repository dal telefono e scarica `la-mia-musica.apk`.
4. Installa (Android chiederà di consentire l'installazione da quella app/browser).

Ogni modifica caricata su GitHub produce una nuova versione, che si installa sopra la precedente
senza perdere nulla.

## Personalizzare

- Colori: `app/src/main/java/com/personale/musica/ui/theme/Theme.kt` e `app/src/main/res/values/colors.xml`
- Nome dell'app: `app/src/main/res/values/strings.xml`

## Nota sulla firma

`app/personale.keystore` è la chiave con cui viene firmato l'APK: non cancellarla, altrimenti
gli aggiornamenti non si installeranno sopra la versione esistente. Se il repository è pubblico,
chiunque potrebbe firmare un APK "compatibile": per un uso personale è consigliato un repository privato.
