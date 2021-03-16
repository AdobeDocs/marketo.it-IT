---
unique-page-id: 12615800
description: Importa account denominati - Documenti Marketo - Documentazione del prodotto
title: Importa account denominati
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 0%

---


# Importa account denominati {#import-named-accounts}

Hai già un CSV pieno di potenziali account di destinazione? Importali direttamente in TAM!

1. Fai clic sull&#39;elenco a discesa **Nuovo** e seleziona **Importa account denominati**.

   ![](assets/inaone.png)

1. Si aprirà una nuova finestra. Fare clic su **Sfoglia**, quindi selezionare il file degli account denominati da importare.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Nel file , fornisci [tutte le informazioni](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes) possibili. È possibile aggiungere solo informazioni firmografiche; non viene calcolato nulla da Marketo (ad esempio Pipeline). Per creare account denominati basati su account CRM, è sufficiente esportare il nome account e l’ID CRM dal CRM in un file CSV, utilizzare l’opzione Nome account e mappare l’ID CRM durante il processo di importazione. Per collegare correttamente un account CRM a un account denominato, devi fornire il nome esatto dell&#39;account CRM.

1. Scegli tra due modalità di deduplicazione: Nome account o nome di dominio. In questo esempio sceglieremo Account. Fai clic sull&#39;elenco a discesa **Modalità** e seleziona **Per nome account**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se si sceglie **Per modalità dominio**, è necessario includere sia l&#39;account denominato che i campi di dominio.

1. Per scegliere a quale elenco di account aggiungere l&#39;account denominato, fai clic sul menu a discesa **Elenco account** e seleziona l&#39;account.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Puoi anche creare un nuovo elenco account digitandone il nome nella casella a discesa.

1. Per inviare una notifica dell’importazione, fai clic sul menu a discesa **Invia avviso a** e seleziona un utente di Marketo. _non è possibile_ inserire manualmente un indirizzo e-mail.

   ![](assets/inafive-2.png)

1. Fare clic su **Avanti**.

   ![](assets/inasix-2.png)

1. Mappa ogni campo facendo doppio clic sul menu a discesa **Campo Marketo** e selezionando il campo appropriato. Al termine, fai clic su **Avanti**.

   ![](assets/inaseven.png)

   Successo!

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
>Quando Marketo aggiunge un account con nome, aggiorna una regola (dietro le quinte) che consente di identificare le persone che dovrebbero far parte dell’account con nome. Esempio: se aggiorni &quot;IBM&quot; a &quot;IBM, USA&quot;, le persone con uno dei due nomi aziendali saranno associate all&#39;account denominato.

Se Marketo trova record che vediamo come duplicati, elaboreremo solo il primo.
