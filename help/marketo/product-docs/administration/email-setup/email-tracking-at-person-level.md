---
description: Scopri in che modo le sostituzioni di tracciamento e-mail a livello di persona ti consentono di controllare il tracciamento delle e-mail aperte e dei clic per ogni persona, in modo da supportare i requisiti di consenso e privacy.
title: Tracciamento e-mail a livello di persona
feature: Email Setup
TQID: 'https://experienceleague.adobe.com/kF-5V-G6-xr3uV-NQBTmFNfhQnk-r-RYt-v0HvJ-4Go'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: a03c57fb-0705-4a0d-b463-bbc931d4cefa
    internal-label: Email setup
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a913c84b1c4f8927c951af685884edfc792ff213
workflow-type: tm+mt
source-wordcount: '1593'
ht-degree: 2%
---
# Tracciamento e-mail a livello di persona {#email-tracking-at-person-level}

Le sostituzioni del tracciamento e-mail a livello di persona consentono di applicare un valore predefinito a livello di ambiente Marketo, quindi di modificarlo per i singoli utenti. Il tracciamento delle aperture e il tracciamento dei clic sono controllati in modo indipendente.

Utilizza questa funzione quando i requisiti di privacy o le policy organizzative richiedono il consenso prima di poter tenere traccia del coinvolgimento nelle e-mail.

>[!IMPORTANT]
>
>Questa funzione fornisce controlli che possono essere utili per supportare gli obblighi di conformità; non determina quali leggi applicare o quali persone devono fornire il consenso. Collabora con i team legali e di privacy per decidere come configurare il tracciamento e come raccogliere e conservare il consenso.

## Funzionamento delle decisioni di tracciamento {#how-tracking-decisions-work}

Tre impostazioni funzionano insieme:

| Impostazione | Livello | Funzione |
|---|---|---|
| **Sostituzioni di tracciamento e-mail a livello di persona** | Ambiente | Attiva o disattiva la funzione. Se questa opzione è disattivata, Marketo Engage ignora i campi predefiniti dell’ambiente e i campi di sostituzione della persona e utilizza il normale comportamento di tracciamento. |
| **Verifica e-mail disattivata per impostazione predefinita** | Ambiente | Imposta il valore predefinito per il tracciamento di apertura e clic. Se è disabilitato, il tracciamento è attivato per impostazione predefinita. Quando è abilitato, il tracciamento è disattivato per impostazione predefinita. |
| **Ignora impostazioni predefinite tracciamento apertura** e **Ignora impostazioni predefinite tracciamento clic** | Persona | Campi persona booleani. Il valore `true` applica l&#39;opposto del valore predefinito dell&#39;ambiente per quel tipo di tracciamento. Un valore di `false` o un valore vuoto segue il valore predefinito dell&#39;ambiente. |

I campi di sostituzione non significano di per sé il consenso o la rinuncia. **`true`significa sempre &quot;l&#39;opposto dell&#39;impostazione predefinita dell&#39;ambiente&quot;**

### Tabella delle decisioni di tracciamento {#tracking-decision-table}

Marketo Engage applica questa decisione separatamente alle aperture delle e-mail e ai clic sulle e-mail.

| Funzione | Impostazione predefinita dell&#39;ambiente | La sostituzione della persona è `false` o vuota | La sostituzione della persona è `true` |
|---|---|---|---|
| Attivato | Tracciamento per impostazione predefinita | Tracciato | Non tracciato |
| Attivato | Tracking off per impostazione predefinita | Non tracciato | Tracciato |
| Disattivato | Non applicabile | Tracciamento normale; override e default vengono ignorati | Tracciamento normale; override e default vengono ignorati |

### Esempio {#example}

Supponiamo che la funzione sia attivata e che l’impostazione predefinita dell’ambiente sia il tracciamento attivato. Una persona ha **Override Open Tracking Default** impostato su `true`, mentre **Override Click Tracking Default** è vuoto. Marketo Engage non tiene traccia delle aperture dei messaggi e-mail di quella persona, ma continua a tenere traccia dei suoi clic e-mail.

## Scegli un modello di tracciamento {#choose-a-tracking-model}

Scegli il modello che soddisfa i requisiti di consenso e privacy prima di abilitare la funzione o popolare i campi di persona.

| Modello | Impostazione predefinita dell&#39;ambiente | Imposta l&#39;override su `true` quando | Uso tipico |
|---|---|---|---|
| Rinuncia | Tracciamento per impostazione predefinita | Una persona si oppone al tracciamento | Tieni traccia della maggior parte delle persone, ma interrompi il tracciamento per le persone che si oppongono. |
| Consenso (consenso) | Tracking off per impostazione predefinita | Una persona dà il consenso al tracciamento | Richiedi il consenso prima del tracciamento, anche per i destinatari coperti dalle linee guida CNIL o Garante applicabili. |

>[!CAUTION]
>
>Scegli il modello prima di popolare i campi di sostituzione ed evita di modificare successivamente i valori predefiniti dell’ambiente. Poiché `true` significa &quot;l&#39;opposto del valore predefinito&quot;, la modifica del valore predefinito inverte l&#39;effetto di ogni valore di sostituzione esistente. Ad esempio, il passaggio dal tracciamento attivato per impostazione predefinita al tracciamento disattivato per impostazione predefinita può causare la tracciabilità delle persone che in precedenza si sono opposte al tracciamento. Se devi modificare l’impostazione predefinita, aggiorna i valori di sostituzione per tutte le persone interessate prima che la modifica diventi effettiva.

## Abilita la funzione {#enable-the-feature}

Le sostituzioni del tracciamento e-mail a livello di persona sono disattivate per impostazione predefinita. Per abilitarlo, contatta l’Assistenza clienti Adobe. È inoltre possibile specificare se si desidera che lo stato predefinito della funzionalità sia **Abilitato** o **Disabilitato** per l&#39;ambiente Marketo.

>[!NOTE]
>
>Per inviare questa richiesta è necessario essere amministratore di Marketo.

>[!TIP]
>
>Prima di richiedere ad Adobe di abilitare la funzione, compila i campi di sostituzione per le persone esistenti. Questo consente di garantire che il comportamento di tracciamento previsto si applichi dalla prima e-mail preparata dopo l’abilitazione.

## Imposta i valori di sostituzione per le persone {#set-override-values-for-people}

I campi di sostituzione sono campi persona booleani. Impostale utilizzando il metodo adatto al flusso di lavoro:

| Metodo | Note |
|---|---|
| [Passaggio del flusso del valore dei dati di modifica](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value){target="_blank"} | Utilizza una campagna intelligente per impostare un campo quando una persona soddisfa i tuoi criteri, ad esempio l’invio di una casella di controllo di consenso in un modulo. |
| Moduli | Mappare una casella di controllo o un campo nascosto in un modulo di Marketo Engage al campo persona. |
| Importazione elenco | Includi il campo come colonna nel file di importazione. |
| REST API | Utilizzare i nomi dei campi API `overrideOpenTrackingDefault` e `overrideClickTrackingDefault`. |

Imposta ogni campo in base al consenso della persona. Se la lingua del consenso tratta le aperture e i clic separatamente, configura ogni campo in modo indipendente.

## Cosa cambia nell’e-mail {#what-changes-in-the-email}

Quando Marketo Engage non tiene traccia di una persona, modifica il contenuto dell’e-mail che invia a tale persona.

| Tracciamento disattivato per | Cosa cambia | Cosa funziona ancora |
|---|---|---|
| Aperti | L’e-mail non include il pixel di tracciamento aperto. Nessuna attività **Apri e-mail** registrata. | Altre funzionalità e-mail, incluso il tracciamento dei clic, se ancora abilitato. |
| Clic | I collegamenti vanno direttamente alle loro destinazioni invece che attraverso il dominio di tracciamento Marketo Engage. Il collegamento di tracciamento nascosto non viene aggiunto. Nessuna attività **E-mail per clic** registrata. | I collegamenti per annullare l&#39;abbonamento, il collegamento di rinuncia al piè di pagina e-mail, `list-unsubscribe` e **Visualizza come pagina Web** continuano a funzionare. L&#39;utilizzo di questi collegamenti non consente di registrare un&#39;attività di tipo **Invia e-mail a un clic**. |

## Quali e-mail sono interessate {#which-emails-are-affected}

| Tipo di e-mail | Sostituzioni applicate? |
|---|---|
| E-mail in batch, ad esempio e-mail inviate da un programma e-mail o una campagna Smart in batch | Sì |
| Attivare le e-mail, ad esempio quelle inviate da una Smart Campaign con trigger | Sì |
| E-mail con test A/B o varianti di campioni/sfidanti | Sì. Il tracciamento viene deciso separatamente per ogni persona, indipendentemente dalla variante che riceve. |
| Visualizza come pagina Web | Sì. La versione web segue le impostazioni correnti dell’utente. La visualizzazione di una modifica può richiedere fino a un&#39;ora. |
| [E-mail operative](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational){target="_blank"} | No. Seguono il normale comportamento di tracciamento. |
| E-mail di esempio (di prova) | No. Seguono il normale comportamento di tracciamento. |
| Anteprime e-mail | Nessun cambiamento. Le anteprime non vengono tracciate. |
| E-mail di avviso | Nessun cambiamento. Gli avvisi non vengono tracciati. |
| Messaggi SMS | No. Questa funzione si applica solo all’e-mail. |

## Quando Marketo Engage prende la decisione di tracciamento {#when-marketo-engage-makes-the-tracking-decision}

Marketo Engage legge i valori di sostituzione di una persona durante la preparazione dell’e-mail per l’invio.

- **Consegna pianificata o ritardata:** Se un&#39;e-mail viene preparata ora e consegnata in un secondo momento (ad esempio, con [Inizio intestazione](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/head-start-for-email-programs){target="_blank"} o [Fuso orario destinatario](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone){target="_blank"}), vengono applicati i valori al momento della preparazione. Una modifica apportata dopo la preparazione non modifica tale e-mail.
- **E-mail già consegnate:** la modifica della sostituzione di una persona non comporta la modifica delle e-mail già ricevute. I clic sui collegamenti nelle e-mail inviate in precedenza possono ancora essere tracciati se tali collegamenti sono stati preparati con il tracciamento abilitato.
- **E-mail future:** Una modifica si applica alle e-mail che Marketo Engage si prepara dopo la modifica.

Se una persona revoca il consenso, aggiorna il valore di sostituzione il prima possibile in modo che la modifica si applichi all’e-mail successiva preparata per essa.

## Impatto su reporting, elenchi avanzati e punteggio {#impact-on-reporting-smart-lists-and-scoring}

Quando Marketo Engage non tiene traccia di una persona, non registra le attività **Apri e-mail** o **Fai clic su E-mail**. Di conseguenza:

- **Elenchi smart/Campagne:** I filtri e i trigger, ad esempio **E-mail aperta** e **Collegamento clic nell&#39;e-mail**, non corrispondono o non vengono attivati per tale persona quando non viene tenuta traccia dell&#39;attività corrispondente.
- **Rapporti e dashboard:** i tassi di apertura delle e-mail, i tassi di clic e le prestazioni dei collegamenti riflettono solo le persone tracciate. Le metriche di coinvolgimento possono diminuire in quanto non vengono tracciate più persone.
- **Punteggio e successo del programma:** Le regole e i passaggi di successo del programma basati su aperture o clic non sono applicabili alle persone le cui attività non sono tracciate. Rivedi queste regole in modo che le persone non siano ingiustamente valutate o avanzate.
- **Associazione attività Web:** Quando il tracciamento dei clic è disattivato, i collegamenti e-mail non contengono il token di tracciamento di Marketo Engage. Se la persona non è già nota a Munchkin, una visita al sito web da tale e-mail non viene associata alla persona tramite il collegamento.

>[!NOTE]
>
>Non influisce sulle attività inviate, consegnate, non recapitate e non sottoscritte.

## Funzionamento con altre impostazioni di tracciamento {#how-this-works-with-other-tracking-settings}

Le sostituzioni del tracciamento e-mail a livello di persona possono disattivare il tracciamento per una persona. Non attiva il tracciamento quando un’altra impostazione lo ha già disabilitato. Ad esempio, i collegamenti contrassegnati con la classe `mktNoTrack` rimangono non tracciati anche quando le impostazioni della persona consentono il tracciamento dei clic.

## Disattiva la funzione {#disable-the-feature}

Per disabilitare le sostituzioni di tracciamento e-mail a livello di persona, contatta l’Assistenza clienti Adobe.

>[!NOTE]
>
>Per inviare questa richiesta è necessario essere amministratore di Marketo.

Dopo la disattivazione, le e-mail preparate dopo la modifica tornano al normale comportamento di tracciamento. I valori di sostituzione rimangono nei record persona ma vengono ignorati. Se la funzione viene riattivata in un secondo momento, i valori memorizzati vengono nuovamente applicati.

## Domande frequenti {#frequently-asked-questions}

### È possibile tenere traccia delle aperture ma non dei clic di una persona o viceversa? {#can-i-track-opens-but-not-clicks-for-a-person-or-the-reverse}

Sì. Il tracciamento delle aperture e dei clic viene deciso in modo indipendente. Imposta solo il campo di sostituzione per il tipo di tracciamento che desideri modificare.

### Questa funzione mi impedisce di inviare e-mail a una persona? {#does-this-feature-stop-me-from-sending-emails-to-a-person}

No. Controlla solo il tracciamento. Per interrompere l’invio di e-mail di marketing a una persona, utilizza le funzioni esistenti di annullamento dell’abbonamento e consenso.

### Le persone non tracciate visualizzano ancora collegamenti di annullamento dell’abbonamento in corso di lavorazione? {#do-people-who-are-not-tracked-still-see-working-unsubscribe-links}

Sì. I collegamenti per annullare l&#39;abbonamento e **Visualizza come pagina Web** continuano a funzionare per tutti gli utenti.

### Perché una persona che ha rinunciato ha ancora un’attività Click Email? {#why-does-a-person-who-opted-out-still-have-a-click-email-activity}

Probabilmente hanno fatto clic su un collegamento in un messaggio e-mail preparato prima della modifica del valore di sostituzione. Le modifiche vengono applicate alle e-mail preparate dopo la modifica.

### Devo modificare i miei modelli e-mail? {#do-i-need-to-change-my-email-templates}

No. Marketo Engage applica la decisione di tracciamento quando crea ogni e-mail. Non è necessario modificare i modelli o le e-mail.
