---
unique-page-id: 12615800
description: Importa account denominati - Documenti Marketo - Documentazione del prodotto
title: Importa account denominati
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---

# Importa account denominati {#import-named-accounts}

Hai già un CSV pieno di potenziali account di destinazione? Importali direttamente in TAM!

1. Fai clic sul pulsante **Nuovo** a discesa e seleziona **Importa account denominati**.

   ![](assets/inaone.png)

1. Si aprirà una nuova finestra. Fai clic su **Sfoglia**, quindi selezionare il file degli account denominati da importare.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Nel file , fornisci [tanto più](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) il più possibile. È possibile aggiungere solo informazioni firmografiche; nulla viene calcolato da Marketo (ovvero pipeline). Per creare account denominati basati su account CRM, è sufficiente esportare il nome account e l’ID CRM dal CRM in un file CSV, utilizzare l’opzione Nome account e mappare l’ID CRM durante il processo di importazione. Per collegare correttamente un account CRM a un account denominato, devi fornire il nome esatto dell&#39;account CRM.

1. Scegli tra due modalità di deduplicazione: Nome account o nome di dominio. In questo esempio sceglieremo Account. Fai clic sul pulsante **Modalità** a discesa e seleziona **Per nome account**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se scegli **Per modalità dominio**, è necessario includere sia l’account con nome che i campi di dominio.

1. Per scegliere a quale elenco di account aggiungere l&#39;account denominato, fare clic su **Elenco account** a discesa ed effettua la selezione.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Puoi anche creare un nuovo elenco account digitandone il nome nella casella a discesa.

1. Per inviare una notifica dell’importazione, fai clic sul pulsante **Invia avviso a** e seleziona un utente Marketo. You _impossibile_ immetti manualmente un indirizzo e-mail.

   ![](assets/inafive-2.png)

1. Fai clic su **Successivo**.

   ![](assets/inasix-2.png)

1. Mappa ogni campo facendo doppio clic sul pulsante **Campo Marketo** e selezionando il campo appropriato. Fai clic su **Successivo** al termine.

   ![](assets/inaseven.png)

   Operazione riuscita!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Verifica stato importazione&quot; mostra solo gli ultimi tre giorni di attività.

Scenari di deduplicazione per nome account:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importazione di record con nome account esistente</strong></td> 
   <td><p>Il record esistente verrà aggiornato</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importazione di record con nuovo nome account denominato</strong></td> 
   <td>Creeremo un nuovo record</td> 
  </tr> 
 </tbody> 
</table>

Scenari di deduplicazione per nome di dominio:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importazione di record con un nuovo nome account e un nuovo nome di dominio</strong></td> 
   <td>Creeremo un nuovo account con nome con le informazioni fornite</td> 
  </tr> 
  <tr> 
   <td><strong>Importazione di record con un nome di account esistente e un nome di dominio esistente</strong></td> 
   <td>Verrà aggiornato l'account con nome esistente</td> 
  </tr> 
   <tr> 
   <td><strong>Importazione di record con un nuovo nome account e un nome di dominio esistente</strong></td> 
   <td>Aggiungeremo il nuovo nome account all’account con nome esistente che corrisponde al nome di dominio e aggiorneremo altre informazioni (ad esempio, Settore, Stato, ecc.)</td> 
  </tr> 
  <tr> 
   <td><strong>Importazione di record con nome account esistente e nuovo nome di dominio</strong></td> 
   <td>Aggiungeremo il nuovo nome di dominio all’account con nome esistente che corrisponde al nome dell’account e aggiorneremo altre informazioni (ad esempio, Settore, Stato, ecc.)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando Marketo aggiunge un account con nome, viene aggiornata una regola (dietro le quinte) che consente di identificare le persone che dovrebbero far parte dell’account con nome. Esempio: se aggiorni &quot;IBM&quot; a &quot;IBM, USA&quot;, le persone con uno dei due nomi aziendali saranno associate all&#39;account denominato.

Se Marketo trova record che vediamo come duplicati, elaboreremo solo il primo.
