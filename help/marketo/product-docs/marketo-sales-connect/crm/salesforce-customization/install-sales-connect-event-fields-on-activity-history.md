---
unique-page-id: 14352475
description: Installa i campi evento Sales Connect nella cronologia delle attività - Marketo Docs - Documentazione del prodotto
title: Installa i campi evento Sales Connect nella cronologia delle attività
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Installa i campi evento Sales Connect nella cronologia delle attività {#install-sales-connect-event-fields-on-activity-history}

Una volta installato il pacchetto Enterprise in Salesforce, è possibile installare i campi evento Sales Connect nella sezione della cronologia delle attività. I campi evento di vendita Connect includono informazioni quali visualizzazioni, clic e campagne. Questo ti consente di importare direttamente in Salesforce le informazioni sulle e-mail.

Assicurati di collaborare con il tuo amministratore Salesforce quando esegui questi passaggi. In questo esempio verranno installati i campi nel **Lead del layout di pagina**. È inoltre possibile installare i campi nei layout della pagina Contatto, Account e Opportunità. Ricorda che, quando esegui la registrazione delle e-mail sugli account e sulle opportunità, avrai bisogno del contatto a cui ti stai associando come ruolo di contatto.

1. Fai clic su **Configurazione**.
1. Fai clic su **Personalizza**.
1. Fai clic su **Lead**.
1. Fai clic su **Layout di pagina**.
1. Fai clic su **Modifica** accanto al layout di pagina che si desidera modificare.

   >[!NOTE]
   >
   >Sales Connect vi installerà alcuni layout di pagina, ma se ne avete già uno predefinito che il vostro team sta utilizzando, vorrete installarlo lì. È possibile eliminare i layout di pagina di Sales Connect se non si desidera utilizzarli.

1. Scorri verso il basso fino alla sezione Cronologia attività .
1. Fai clic sulla chiave inglese da modificare.
1. Selezionare i campi Connetti alle vendite che si desidera includere nella sezione Cronologia attività. Se i campi di vendita Connect non sono visualizzati, è possibile che sia stato installato il pacchetto Salesforce errato.
1. Fai clic su **Aggiungi** per spostare i campi desiderati.
1. Fai clic su **OK**.
1. Fai clic su **Salva**.

   Gli utenti possono ora vedere informazioni e aggiornamenti utili sulle loro e-mail in Salesforce!
