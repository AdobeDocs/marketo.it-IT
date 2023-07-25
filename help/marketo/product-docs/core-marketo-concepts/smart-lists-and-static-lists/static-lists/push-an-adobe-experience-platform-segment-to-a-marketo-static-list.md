---
description: Invio di un segmento Adobe Experience Platform a un elenco statico Marketo - Documenti Marketo - Documentazione del prodotto
title: Invio di un segmento Adobe Experience Platform a un elenco statico Marketo
exl-id: 8df11bf4-06f4-4927-8dfb-954414fce6dc
feature: Static Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# Invio di un segmento Adobe Experience Platform a un elenco statico Marketo {#push-an-adobe-experience-platform-segment-to-a-marketo-static-list}

Questa funzione consente di inviare a Marketo i segmenti presenti nel Adobe Experience Platform sotto forma di elenco statico.

>[!PREREQUISITES]
>
>* [Modifica il ruolo API](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#edit-an-existing-role) per assicurarsi che abbia **Persona di lettura/scrittura** autorizzazione (disponibile nel menu a discesa API di Access ).
>* [Creare un utente API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) in Marketo.
>* Vai a **Amministratore** > **Launchpoint**. Individuare il nome del ruolo appena creato e fare clic su **Visualizza dettagli**. Copiare e salvare le informazioni in **ID client** e **Segreto client**, in quanto potrebbe essere necessario per il passaggio 7.
>* In Marketo, crea un elenco statico oppure individuane e selezionane uno già creato. Avrai bisogno del suo ID.

1. Accedi a [Adobe Experience Platform](https://experience.adobe.com/).

   ![](assets/push-an-adobe-experience-platform-segment-1.png)

1. Fai clic sull’icona della griglia e seleziona **Experience Platform**.

   ![](assets/push-an-adobe-experience-platform-segment-2.png)

1. Nella barra di navigazione a sinistra, fai clic su **Destinazioni**.

   ![](assets/push-an-adobe-experience-platform-segment-3.png)

1. Clic **Catalogo**.

   ![](assets/push-an-adobe-experience-platform-segment-4.png)

1. Trova il riquadro Marketo Engage e fai clic su **Attiva**.

   ![](assets/push-an-adobe-experience-platform-segment-5.png)

1. Clic **Configura nuova destinazione**.

   ![](assets/push-an-adobe-experience-platform-segment-6.png)


1. In Tipo di account, seleziona il pulsante di opzione Account esistente o nuovo (in questo esempio, scegliamo **Account esistente**). Fai clic sull’icona Seleziona account.

   ![](assets/push-an-adobe-experience-platform-segment-7.png)

   >[!NOTE]
   >
   >Se scegli un nuovo account, puoi trovare il tuo ID Munchkin da **Amministratore** > **Munchkin** (una volta effettuato l’accesso, fa anche parte dell’URL di Marketo). ID client/Segreto dovrebbe essere possibile seguire i prerequisiti nella parte superiore di questo articolo.

1. Scegli l’account di destinazione e fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-8.png)

1. Immetti una destinazione **Nome** e una Descrizione facoltativa. Fai clic sull’elenco a discesa Creazione persona e scegli &quot;Abbina persone Marketo esistenti e crea persone mancanti in Marketo&quot; _o_ &quot;Abbina solo persone Marketo esistenti&quot; (in questo esempio stiamo scegliendo la prima). Devi anche scegliere un **Workspace**.

   ![](assets/push-an-adobe-experience-platform-segment-9.png)

   >[!NOTE]
   >
   >Se scegli &quot;Match Existing Marketo People Only&quot; (Confronta solo persone esistenti), dovrai mappare solo l’e-mail e/o l’ECID, quindi puoi saltare i passaggi 13-16.

1. Questa sezione è facoltativa. Clic **Crea** da saltare.

   ![](assets/push-an-adobe-experience-platform-segment-10.png)

1. Seleziona la destinazione creata e fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-11.png)

1. Scegli il segmento da inviare a Marketo e fai clic su **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-12.png)

   >[!NOTE]
   >
   >Se scegli più segmenti, dovrai mappare ciascun segmento a un elenco statico specificato nella scheda Pianificazione segmenti.

   >[!IMPORTANT]
   >
   >Dopo che un segmento è stato attivato nella destinazione Marketo per la prima volta, i profili di backfill già presenti nel segmento prima dell’attivazione della destinazione Marketo possono richiedere **fino a 24 ore**. In futuro, ogni volta che i profili verranno aggiunti al segmento, verranno aggiunti immediatamente a Marketo.

1. Clic **Aggiungi nuova mappatura**.

   ![](assets/push-an-adobe-experience-platform-segment-13.png)

1. Fai clic sull’icona di mappatura.

   ![](assets/push-an-adobe-experience-platform-segment-14.png)

1. Scegli gli attributi desiderati e fai clic su **Seleziona**. In questo esempio, scegliamo nome, cognome e indirizzo e-mail.

   ![](assets/push-an-adobe-experience-platform-segment-15.png)

   >[!NOTE]
   >
   >È possibile mappare gli attributi da Experience Platform a qualsiasi attributo a cui l&#39;organizzazione ha accesso in Marketi Engage. Utilizza il [Descrizione della richiesta API](https://developers.marketo.com/rest-api/lead-database/leads/#describe){target="_blank"} per recuperare i campi attributo a cui la tua organizzazione ha accesso.

1. Mappare Cognome e Nome società facendo clic su **Aggiungi nuova mappatura** e ripetendo due volte il passaggio 15, scegliendo **lastName** e poi **companyName**.

   ![](assets/push-an-adobe-experience-platform-segment-16.png)

1. Ora è il momento di mappare l’indirizzo e-mail. Clic **Aggiungi nuova mappatura** di nuovo.

   ![](assets/push-an-adobe-experience-platform-segment-17.png)

1. Fai clic sull’icona di mappatura.

   ![](assets/push-an-adobe-experience-platform-segment-18.png)

1. Fai clic sul pulsante di opzione Seleziona lo spazio dei nomi dell’identità, scegli  **E-mail**, quindi fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-19.png)

   >[!IMPORTANT]
   >
   >Mappatura di e-mail e/o ECID da **Spazio dei nomi identità** La scheda è la cosa più importante da fare per garantire che la persona corrisponda in Marketo. La mappatura dell’e-mail garantirà la percentuale di corrispondenza più elevata.

1. Ora è il momento di scegliere i campi sorgente. Per l’e-mail, fai clic sull’icona del cursore.

   ![](assets/push-an-adobe-experience-platform-segment-20.png)

1. Fai clic sul pulsante di opzione Seleziona lo spazio dei nomi dell’identità, individua e seleziona **E-mail**, quindi fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-21.png)

1. Per scegliere il campo di origine Nome società, fare clic sull&#39;icona del cursore nella riga corrispondente.

   ![](assets/push-an-adobe-experience-platform-segment-22.png)

1. Lasciare selezionato il pulsante di opzione Seleziona attributi. Cerca &quot;azienda&quot; e seleziona **companyName**, quindi fai clic su **Seleziona**.

   ![](assets/push-an-adobe-experience-platform-segment-23.png)

1. Mappare i campi di origine per Cognome e Nome facendo clic sull&#39;icona del cursore per ogni campo e ripetendo due volte il passaggio 23, scegliendo **lastName** e poi **firstName**.

   ![](assets/push-an-adobe-experience-platform-segment-24.png)

1. Clic **Successivo**.

   ![](assets/push-an-adobe-experience-platform-segment-25.png)

1. Rivedi le modifiche e fai clic su **Fine**.

   ![](assets/push-an-adobe-experience-platform-segment-26.png)
