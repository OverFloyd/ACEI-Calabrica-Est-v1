# Biv/PC Calabrica Est - Apparato ACEI
Funzioni costituenti la logica dell'ACEI (soppresso) del posto di servizio Bivio/Posto di Comunicazione Calabrica Est. Per informazioni sulla costituzione del piazzale consultare il sottostante piano schematico.

Per le abbreviazioni consultare la relativa [sezione](#abbreviazioni).

![piano schematico](https://github.com/OverFloyd/Calabrica-Est-ACEI-v1/blob/master/bivpccalabricaest/PS%20Biv-PC%20Calabrica%20Est%20(20-08-2017).png)

Premessa: la logica di funzionamento è da considerarsi obsoleta, non più utilizzabile e ormai fuori standard rispetto a quelli per apparati simili. Questo vale per diversi aspetti, ad esempio: tutti i PdS che non siano stazioni (o Posti di Movimento) non dispongono di itinerari di partenza in quanto sono dotati del solo segnalamento di protezione (al contrario del presente impianto, dove non si ha un gruppo scambi unico ma due costituiti da una comunicazione ciascuno), completa mancanza di collegamenti di sicurezza, non esiste automatica ridisposizione a via impedita dei segnali, bloccamento degli enti, consensi in UM, sistema di occupazione degli itinerari ecc.

## Storia
L'ACEI per il PdS Biv/PC Calabrica Est venne attivato nel 2017 a poca distanza dall'introduzione delle funzioni (.mcfunction) per sostituire il precedente apparato di tipo ACE tipo IV, è stata la prima vera implementazione di tale feature in ambito ferroviario in Sider.

Sviluppato fino al 2018, l'apparato cadde gradualmente in disuso a causa della mancanza di validi collegamenti di sicurezza tra gli enti di piazzale, non gestiti propriamente dall'apparato, causando conflitti nella costruzione degli itinerari. Di conseguenza l'impianto venne escluso e la località di servizio gestita in regime di autogestione con il piazzale gestito all'evenienza dal preesistente apparato ACE.

L'ACEI venne definitivamente soppresso nel 2022, ma si prevede una totale ricostruzione con l'impiego dei nuovi standard e tecnologie già testate sul nuovo apparato di Piana del Tevere (ACE tipo V).

## Logica di funzionamento
### Itinerari
L'apparato era in grado di costruire itinerari dai PO (corrispondenti ai segnali di protezione) ai PF (identificati nel FM) per quelli di arrivo e viceversa per quelli di partenza.

In ogni funzione d'itinerario era comandata la manovra dei singoli enti del piazzale (deviatoi, segnali bassi e alti), che a loro volta avevano funzioni per l'attivazione e disattivazione. Per necessità di costituzione d'impianto (mancanza di spazio), i segnali bassi costituivano il segnalamento di partenza lato Montignolo e Calabrica.

Non era presente alcun ritorno in UM per la disposizione degli enti (Quadro Consensi) o alcun collegamento di sicurezza relativo alla loro corretta disposizione, il segnale veniva posto a via libera indifferentemente dalla disposizione degli enti, dando per scontato che fossero nella posizione voluta (motivazione per cui la soppressione dell'impianto divenne inevitabile).

#### Transito
Gli itinerari di transito erano costituiti da rispettivamente l'itinerario di arrivo seguito dall'itinerario di partenza (protezione X - FM - protezione Y). Ogni qual volta veniva costruito un itinerario di transito l'apparato comandava automaticamente l'attivazione delle rotaie elettrificate poste in corrispondenza del FM, in modo tale che il treno non si dovesse obbligatoriamente fermare.

All'attivazione degli itinerari (di arrivo e di transito) veniva piazzata una redstone torch per itinerario in dei punti specifici sotto le rotaie elettrificate in modo tale che, se gli itinerari fossero stati congruenti, queste si sarebbero attivate permettendo il transito.

### Funzioni speciali
In entrambi gli UM era possibile porre l'impianto in regime di impresenziamento (autogestione) o presenziamento in locale (escltlc-tp / tlc-tp). Era inoltre possibile effettuare un reset generale di tutti gli itinerari in atto, in caso di malfunzionamento del sistema (dis-all-it).

### Regime di autogestione
In regime di impresenziamento, o autogestione, in precedenza dei segnali di protezione venivano abilitate delle rotaie provviste di boe che, quando venivano energizzate, comandavano automaticamente la costruzione del transito da Calabrica a Montignolo (3p-FM 1-1) e viceversa (1-FM 2-3d).

## Abbreviazioni
* ACE: Apparato Centrale Elettrico (a leve individuali)
* ACEI: Apparato Centrale Elettrico a Itinerari
* d: [binario] dispari
* FM: Fabbricato Movimento
* p: [binario] pari
* PC: Posto di Comunicazione
* PdS: Posto di Servizio
* PF: Punto Fine (d'itinerario)
* PO: Punto Origine (d'itinerario)
* UM: Ufficio Movimento
