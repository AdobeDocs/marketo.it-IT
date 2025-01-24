---
description: Rendere visibile una campagna di marketing nelle azioni di approfondimento sulle vendite - Documenti Marketo - Documentazione del prodotto
title: Rendere visibile una campagna di marketing nelle azioni di approfondimento sulle vendite
exl-id: 223baca3-159e-4f0d-b26f-f4c924a39fc3
feature: Sales Insight Actions
source-git-commit: c6132bf5b393df38700ad9dd6f0c6414860e8bb6
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Rendere visibile una campagna di marketing nelle azioni di approfondimento sulle vendite {#make-a-marketing-campaign-visible-in-sales-insight-actions}

Le campagne possono essere condivise solo se sono rese visibili.

Con le azioni di approfondimento sulle vendite, gli utenti avranno accesso a una nuova app di vendita denominata toutapp.com. Questa app offre loro una nuova serie di funzionalità di azione, ma eredita anche la funzionalità _Aggiungi a campagna di marketing_ disponibile nella versione di base di Sales Insights. È importante tenerlo presente, perché a seconda della posizione in cui desideri che gli utenti accedano alla funzione Aggiungi a campagna di marketing (toutapp.com o l’esperienza del pacchetto MSI SFDC), le campagne Marketo dovranno essere configurate in modo diverso. Per ulteriori informazioni, consulta la nota nel passaggio 4.

1. Seleziona (o crea) la campagna da condividere.

   ![](assets/make-a-marketing-campaign-visible-sia-1.png)

1. Fare clic sulla scheda **Elenco avanzato**.

   ![](assets/make-a-marketing-campaign-visible-sia-2.png)

1. Aggiungere il trigger _Campaign is Requested_.

   ![](assets/make-a-marketing-campaign-visible-sia-3.png)

1. Per l&#39;origine, scegliere &quot;is&quot; **API servizio Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-4.png)

   >[!NOTE]
   >
   >Se desideri mostrare la campagna di marketing agli utenti che utilizzano _Aggiungi alla campagna di marketing_ dall&#39;app Web toutapp.com (anche se l&#39;app Web è incorporata nel sistema CRM tramite l&#39;oggetto Marketo Sales Outbox), imposta l&#39;origine richiesta di Campaign su &quot;Web Service API&quot;. Se desideri che la campagna di marketing venga visualizzata quando un utente utilizza le azioni nel pannello MSI di Salesforce sul lead, il contatto, la pagina dell’account o i pulsanti di azione collettiva nelle visualizzazioni elenco lead e contatti, aggiorna l’origine richiesta della campagna in &quot;Informazioni sulle vendite&quot;

1. Fare clic sulla scheda **Flusso**.

   ![](assets/make-a-marketing-campaign-visible-sia-5.png)

1. Aggiungi l&#39;azione di flusso _Momento di interesse_.

   ![](assets/make-a-marketing-campaign-visible-sia-6.png)

1. Per Tipo, selezionare **Web**.

   ![](assets/make-a-marketing-campaign-visible-sia-7.png)

1. Nella casella _Descrizione_, scrivi un messaggio al team vendite. In questo esempio utilizziamo i token per specificare il modulo compilato.

   ![](assets/make-a-marketing-campaign-visible-sia-8.png)

1. Fai clic sulla scheda **Pianifica** e **Attiva** la campagna.

   ![](assets/make-a-marketing-campaign-visible-sia-9.png)
