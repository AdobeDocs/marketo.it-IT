---
description: Panoramica sull’annullamento dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica sull’annullamento dell’abbonamento
exl-id: 7598efa9-9686-4dd0-840b-f8b6de4ab2be
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Panoramica sull’annullamento dell’abbonamento {#unsubscribe-overview}

Sta diventando sempre più importante per le organizzazioni rispettare le leggi sulla privacy delle e-mail. Per aiutarci con questo, abbiamo apportato alcuni miglioramenti alla nostra esperienza di annullamento dell’iscrizione.

* I collegamenti per l&#39;annullamento dell&#39;abbonamento vengono inseriti in tutte le e-mail inviate da [!DNL Marketo Sales] e [!DNL Salesforce] (questo non si applica alle e-mail personalizzate inviate da [!DNL Outlook] o Gmail)
* Gli amministratori possono modificare i messaggi di annullamento dell’iscrizione per l’intero team
* Le informazioni di annullamento dell&#39;abbonamento vengono memorizzate in PDV
* Gli annullamenti dell&#39;iscrizione possono essere eseguiti manualmente: collegamento selezionato, sincronizzazione di [!DNL Salesforce] e mancato recapito
* Nuova pagina di destinazione con collegamento per annullare l’abbonamento

## Pagina di destinazione collegamento per annullare l’iscrizione {#unsubscribe-link-landing-page}

Quando una persona fa clic sul collegamento per annullare l’abbonamento, viene indirizzata a una pagina di destinazione per annullare l’abbonamento, in cui può selezionare l’utente dal quale desidera annullare l’abbonamento e il motivo per cui farlo.

![](assets/unsubscribe-overview-1.png)

Queste informazioni verranno salvate nella vista dei dettagli della persona per essere visualizzate in un secondo momento.

## Annulla sottoscrizione gruppo {#unsubscribe-group}

Visualizza e gestisci tutte le persone non iscritte in un&#39;unica posizione.

![](assets/unsubscribe-overview-2.png)

Utilizza la barra di ricerca per cercare le persone non iscritte.

![](assets/unsubscribe-overview-3.png)

Se sei un amministratore, puoi passare al gruppo di annullamento dell&#39;iscrizione per filtrare in base a [!UICONTROL Account Unsubscribes] e visualizzare tutti gli annullamenti dell&#39;iscrizione raccolti nel database delle persone.

![](assets/unsubscribe-overview-4.png)

## Scheda Cronologia per annullare l’iscrizione {#unsubscribe-history-card}

La scheda [!UICONTROL Unsubscribe History] consente agli amministratori e agli utenti di ottenere informazioni contestuali sulla cronologia degli annullamenti dell&#39;abbonamento dei loro contatti. Passare alla scheda [!UICONTROL People] e selezionare una persona. Si trova nella parte inferiore della scheda [!UICONTROL About] nella visualizzazione Dettagli persona.

>[!NOTE]
>
>Ci sarà una carta [!UICONTROL Unsubscribe History] solo se la persona ha _rinnovato l&#39;abbonamento_ ad un certo punto.

![](assets/unsubscribe-overview-5.png)

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>[!UICONTROL Date]</strong></td> 
   <td><p>Mostra la data in cui si è verificato l’annullamento/il reabbonamento.</p></td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Details]</strong></td> 
   <td><p>Risottoscrivi: un amministratore [!DNL Sales Connect] ha rimosso manualmente l'annullamento dell'iscrizione dal record del contatto. Potrebbero inoltre essere visualizzati alcuni dettagli relativi al motivo per cui il contatto ha annullato l’abbonamento.</p><p>Annulla iscrizione: il contatto ha annullato l’iscrizione.</p></td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Source]</strong></td> 
   <td><p>[!DNL Salesforce] Sincronizzazione: l'annullamento dell'abbonamento è stato acquisito da una sincronizzazione da [!DNL Salesforce].</p><p>Manuale: l’utente ha fatto clic sul pulsante per annullare l’abbonamento e rinunciare.</p><p>Collegamento selezionato: il destinatario di un’e-mail ha fatto clic sul collegamento per annullare l’abbonamento.</p><p>"Admin Name" (Nome amministratore): il nome di un amministratore viene visualizzato quando l’azione consisteva nel riabbonare i contatti. In questo modo gli utenti possono sapere chi ha rimosso l’annullamento dell’abbonamento.</p></td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Personalizza messaggio di collegamento per annullare l&#39;iscrizione](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/customize-unsubscribe-link-message.md)
