---
description: Creazione di un messaggio SMS - Documentazione di Marketo - Documentazione del prodotto
title: Creare un messaggio SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 96bc28212ef275920fb106d69293958522cb4eb0
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Creare un messaggio SMS {#create-an-sms-message}

Ecco come creare un messaggio SMS.

>[!AVAILABILITY]
>
>Questa funzione è disponibile come componente aggiuntivo per il tuo account Adobe Marketo Engage. Per essere fornito correttamente, deve essere acquistato tramite Adobe. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

>[!PREREQUISITES]
>
>[Aggiungere Vibes come servizio LaunchPoint](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md)

1. Vai a **[!UICONTROL Attività di marketing]**.

   ![](assets/create-an-sms-message-1.png)

1. Fai clic con il pulsante destro del mouse sul programma desiderato e seleziona (Condividi) **[!UICONTROL Nuova risorsa locale]**.

   ![](assets/create-an-sms-message-2.png)

1. Seleziona **Messaggio SMS**.

   ![](assets/create-an-sms-message-3.png)

1. Immetti un nome e una descrizione facoltativa per il nuovo messaggio SMS e fai clic su **Crea**.

   ![](assets/create-an-sms-message-4.png)

1. Nell’editor, fai clic all’interno della bolla blu e inizia a immettere il testo.

   ![](assets/create-an-sms-message-5.png)

   >[!NOTE]
   >
   >Il limite di caratteri per un messaggio SMS è di 160 caratteri utilizzando il set di caratteri ASCII standard. Se superi i 160 caratteri, il messaggio verrà suddiviso in base al numero totale di caratteri.

1. Per aggiungere un token al messaggio, scrivi un saluto rapido e fai clic su **Token**.

   ![](assets/create-an-sms-message-6.png)

   >[!NOTE]
   >
   >L’aggiunta di un token può causare il superamento del limite di caratteri per il messaggio. Il messaggio viene quindi suddiviso, creando un messaggio aggiuntivo.

   >[!IMPORTANT]
   >
   >Conformità SMS: tutti i messaggi SMS in uscita devono includere il nome del marchio o la descrizione del programma. Le istruzioni HELP e STOP devono essere fornite almeno una volta al mese per ogni abbonato ai programmi con messaggi ricorrenti.

1. Seleziona il **Token**, immettere un valore facoltativo **Valore predefinito** e fai clic su **Crea**.

   ![](assets/create-an-sms-message-7.png)

1. Per aggiungere un collegamento, seleziona la posizione del messaggio da visualizzare e fai clic su **Collegamento**.

   ![](assets/create-an-sms-message-8.png)

1. Seleziona un tipo di collegamento. Pagina di destinazione di Marketo è l’impostazione predefinita. Se si continua, fare clic sul menu a discesa Pagina di destinazione e selezionare la pagina desiderata. Clic **Inserisci** al termine.

   ![](assets/create-an-sms-message-9.png)

   >[!NOTE]
   >
   >I due collegamenti di tracciamento sono selezionati per impostazione predefinita. Deselezionando Solo Includi mkt_tok sarà comunque possibile tenere traccia del collegamento, ma dopo il reindirizzamento l’URL di destinazione non includerà il parametro della stringa di query mkt_tok. Questo parametro viene utilizzato dalle pagine di destinazione di Marketo e da Munchkin per garantire il corretto tracciamento delle attività della persona (come quando una persona rinuncia).

1. Se invece desideri utilizzare un URL esterno, seleziona **URL esterno**, immetti/incolla l’URL e fai clic su **Inserisci**.

   ![](assets/create-an-sms-message-10.png)

   >[!NOTE]
   >
   >Quando si mantiene selezionato &quot;Traccia collegamento&quot;, Marketo modifica automaticamente l’URL a scopo di tracciamento. Se scegli di disabilitare il tracciamento, l’URL non verrà modificato nel messaggio (ad esempio, `www.adobe.com`).

   >[!CAUTION]
   >
   >Si consiglia di: _non_ utilizza abbreviazioni URL (ad esempio, Bits), in quanto i gestori potrebbero contrassegnare il messaggio come spam.

1. Il collegamento viene visualizzato nel messaggio.

   ![](assets/create-an-sms-message-11.png)

   >[!NOTE]
   >
   >In Marketo viene visualizzata un’anteprima dei collegamenti del dominio di tracciamento del marchio. Se deselezionate la casella di controllo Collegamento mkt_tok (Market_tok link), il collegamento viene modificato.

Se inserisci più di 160 caratteri, l’editor suddivide l’SMS in sezioni. È previsto un limite complessivo di 900 caratteri per messaggio. Se superi questo limite, il messaggio verrà troncato alla consegna.
