---
unique-page-id: 12615800
description: Importa account denominati - Documenti Marketo - Documentazione prodotto
title: Importa account denominati
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---


# Importa account denominati {#import-named-accounts}

Hai già un CSV pieno di potenziali account di destinazione? Importateli direttamente in ABM!

1. Fare clic sul menu a discesa **Nuovo** e selezionare **Importa account denominati**.

   ![](assets/inaone.png)

1. Si aprirà una nuova finestra. Fare clic su **Sfoglia**, quindi selezionare il file di account denominati da importare.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Nel file, fornire [tutte le informazioni](http://docs.marketo.com/display/DOCS/Named+Account+Overview#NamedAccountOverview-NamedAccountAttributes) possibili. È possibile aggiungere solo informazioni relative alla fotografia; nessun valore calcolato da Marketo (ad es. Pipeline). Per creare account denominati basati su account CRM, è sufficiente esportare il nome account e l&#39;ID CRM dal CRM in un file CSV, utilizzare l&#39;opzione Nome account e mappare l&#39;ID CRM durante il processo di importazione. Per collegare correttamente un account CRM a un account denominato, devi fornire il nome esatto dell&#39;account CRM.

1. Scegliete tra due modalità di deduplicazione: Nome account o Nome dominio. In questo esempio sceglieremo Account. Fare clic sul menu a discesa **Modes** e selezionare **Per nome account**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se si sceglie **Per modalità di dominio**, è necessario includere sia l&#39;account denominato che i campi di dominio.

1. Per scegliere l&#39;elenco account a cui aggiungere l&#39;account, fare clic sul menu a discesa **Elenco account** ed effettuare la selezione.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >Potete anche creare un nuovo elenco account digitandone semplicemente il nome nella casella a discesa.

1. Per inviare una notifica dell&#39;importazione, fate clic sul menu a discesa **Invia avviso a** e selezionate un utente di Marketing. *non è possibile* inserire manualmente un indirizzo e-mail.

   ![](assets/inafive-2.png)

1. Fare clic su **Next**.

   ![](assets/inasix-2.png)

1. Mappare ciascun campo facendo doppio clic sul campo **Campo marketing** e selezionando il campo appropriato. Fare clic su **Next** al termine.

   ![](assets/inaseven.png)

   Successo!

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Controlla stato importazione&quot; mostra solo gli ultimi tre giorni di attività.

<table> 
 <tbody> 
  <tr> 
   <td>Importazione di record con nome account esistente</td> 
   <td><p>Aggiorneremo il record esistente</p></td> 
  </tr> 
  <tr> 
   <td>Importazione di record con nuovo nome account denominato</td> 
   <td>Creeremo un nuovo record</td> 
  </tr> 
 </tbody> 
</table>

Scenari di deduplicazione per Nome dominio:

| **Importazione di record con un nuovo nome account e un nuovo nome di dominio** | Creeremo un nuovo account denominato con le informazioni fornite |
|---|---|
| **Importazione di record con un nome account esistente e un nome di dominio esistente** | Verrà aggiornato l&#39;account denominato esistente |
| **Importazione di record con un nuovo nome account e un nome di dominio esistente** | Aggiungeremo il nuovo nome account all&#39;account denominato esistente che corrisponde al nome del dominio e aggiorneremo altre informazioni (ad esempio, Settore, Stato, ecc.) |
| **Importazione di record con nome account esistente e nuovo nome di dominio** | Aggiungeremo il nuovo nome di dominio all&#39;account denominato esistente che corrisponde al nome dell&#39;account e aggiorneremo altre informazioni (ad esempio, Settore, Stato, ecc.) |

>[!NOTE]
>
>Quando Marketo aggiunge un account denominato, stiamo aggiornando una regola (dietro le quinte) che ci consente di identificare le persone che dovrebbero essere parte dell&#39;account denominato. Esempio: se aggiorni &quot;IBM&quot; a &quot;IBM, USA&quot;, le persone con entrambi i nomi aziendali saranno associate all&#39;Account denominato.

Se Marketo trova documenti che vediamo come duplicati, elaboreremo solo il primo.

Scenari di deduplicazione per Nome account: