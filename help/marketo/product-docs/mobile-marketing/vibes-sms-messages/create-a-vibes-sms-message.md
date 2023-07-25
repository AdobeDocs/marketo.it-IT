---
unique-page-id: 11378869
description: Creazione di un messaggio Vibes SMS - Documentazione di Marketo - Documentazione di prodotto
title: Creare un messaggio Vibes SMS
exl-id: 9ec0da97-7a80-4c40-be79-be08d7d1d9c1
feature: Mobile Marketing
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Creare un messaggio Vibes SMS {#create-a-vibes-sms-message}

Ecco come creare un messaggio SMS Vibes.

>[!AVAILABILITY]
>
>Questa funzione è disponibile come componente aggiuntivo per il tuo account Adobe Marketo Engage. Per essere fornito correttamente, deve essere acquistato tramite Adobe. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

>[!NOTE]
>
>I messaggi di testo SMS non sono conformi a HIPAA.

1. Vai a **Attività di marketing** e fare clic con il pulsante destro del mouse su un programma.

   ![](assets/mobile-right-click-hand.jpg)

1. Clic **Nuova risorsa locale**.

   ![](assets/new-local-asset-hand.jpg)

   >[!TIP]
   >
   >In alternativa, è possibile fare clic su **Nuovo** a discesa.

1. Clic **Messaggio SMS**.

   ![](assets/new-local-asset-selection-hand.jpg)

1. Immetti un nome e una descrizione facoltativa per il nuovo messaggio SMS e fai clic su **Crea**.

   ![](assets/new-sms-message-offer-ends-soon-hands.jpg)

1. Clic **Modifica bozza**.

   ![](assets/edit-draft-hand.jpg)

1. Nell’editor dei messaggi, fai clic all’interno della bolla blu e inizia a immettere il testo.

   ![](assets/message-text-pencil.jpg)

   >[!NOTE]
   >
   >I limiti per gli Stati Uniti e il Canada sono diversi, rispettivamente a 160 e 130 caratteri. Se superi questi limiti di caratteri, il messaggio potrebbe essere diviso. Anche se mostriamo quando superi il limite canadese, l’editor è ottimizzato per gli Stati Uniti e divide il messaggio in base al limite degli Stati Uniti.

1. Clic **Token** per aggiungere un token al messaggio.

   ![](assets/add-token-real-hand.jpg)

   >[!NOTE]
   >
   >L’aggiunta di un token può causare il superamento del limite di caratteri per il messaggio. Il messaggio verrà quindi suddiviso, con conseguente addebito di ulteriori costi.

1. Clic **Collegamento** per aggiungere un collegamento al messaggio.

   ![](assets/full-message-link-hand.jpg)

1. Seleziona un tipo di collegamento. Pagina di destinazione di Marketo è l’impostazione predefinita. Se utilizzi questa funzione, seleziona la pagina di destinazione dal menu a discesa e fai clic su **Inserisci**.

   ![](assets/insert-link-real-hands.jpg)

   >[!NOTE]
   >
   >I due collegamenti di tracciamento sono selezionati per impostazione predefinita.

1. Se invece desideri utilizzare un URL esterno, fai clic su **URL esterno** e immetti l’URL nel campo URL. Clic **Inserisci**.

   ![](assets/insert-link-url-hands.jpg)

1. Il collegamento viene visualizzato nel messaggio.

   ![](assets/link-added.jpg)

   >[!NOTE]
   >
   >In Marketo viene visualizzata un’anteprima dei collegamenti del dominio di tracciamento del marchio. Se deselezionate la casella di controllo Collegamento mkt_tok (Market_tok link), il collegamento viene modificato. Deseleziona anche la casella di controllo Track Link (Collegamento traccia) e l’URL verrà ridotto alla sua lunghezza di base (ad esempio, www.mygooglepage.com).

   ![](assets/image2016-7-27-16-3a20-3a16.png)

   >[!NOTE]
   >
   >Il conteggio dei caratteri riflette solo i caratteri contenuti nel messaggio più basso.

Se inserisci un numero di elementi superiore al limite per gli Stati Uniti, l’editor suddivide il messaggio in sezioni. Il limite totale assoluto è di 900 caratteri. Una volta raggiunto tale limite, il messaggio viene troncato automaticamente quando viene inviato al relativo pubblico.
