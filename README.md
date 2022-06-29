# Biv/PC Calabrica Est
Funzioni per la gestione dell'ACEI (soppresso) del PdS Bivio/PC Calabrica Est.

## Storia
L'ACEI per il posto di servizio Bivio/PC Calabrica Est nasce nel 2017 a poca distanza dall'introduzione delle funzioni (.mcfunction) e fu la prima vera implementazione di tale feature in ambito ferroviario in Sider.

Sviluppato fino al 2018, l'apparato cadde gradualmente in disuso a causa della mancanza di validi collegamenti di sicurezza tra gli enti di piazzale, non gestiti propriamente dall'apparato.
Di conseguenza l'impianto venne escluso e la località di servizio gestita in regime di autogestione con il piazzale gestito all'evenienza dal preesistente apparato di tipo ACE.

L'ACEI venne definitivamente soppresso nel 2022, ma si prevede una totale ricostruzione con l'impiego dei nuovi standard e tecnologie già testate sul nuovo apparato di Piana del Tevere.

--CD450

## Logica di funzionamento
### Itinerari
L'apparato era in grado di costruire itinerari dai Punti Origine (segnali di protezione) ai Punti Fine (identificati nel fabbricato movimento).
Erano suddivisi in itinerari di arrivo e partenza. In ogni funzione di itinerario era comandata la manovra dei singoli enti del piazzale (deviatoi, segnali bassi e alti), che a loro volta avevano funzioni per l'attivazione e disattivazione.

Non era presente alcun ritorno in UM per la disposizione degli enti (Quadro Consensi) o alcun collegamento di sicurezza relativo alla loro corretta disposizione, il segnale veniva posto a via libera indifferentemente dalla disposizione degli enti, dando per scontato che fossero nella posizione voluta (motivazione per cui la soppressione dell'impianto divenne inevitabile).

### Funzioni speciali
Nell'Ufficio Movimento dell'apparato ACE era possibile porre l'impianto in regime di impresenziamento (autogestione) o presenziamento in locale (escltlc-tp / tlc-tp). Era inoltre possibile effettuare un reset generale di tutti gli itinerari in quel momento in atto, in caso di malfunzionamento del sistema (dis-all-it).
