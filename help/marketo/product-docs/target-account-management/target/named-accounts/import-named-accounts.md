---
unique-page-id: 12615800
description: Importa [!UICONTROL Named Accounts] - Documentazione Marketo - Documentazione del prodotto
title: Importa [!UICONTROL Named Accounts]
exl-id: 3f40e567-9256-4efd-beea-4e818770759f
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Importa [!UICONTROL Named Accounts] {#import-named-accounts}

Hai già un file CSV pieno di potenziali account di destinazione? Importateli direttamente in TAM!

1. Fare clic sul menu a discesa **[!UICONTROL New]** e selezionare **[!UICONTROL Import Named Accounts]**.

   ![](assets/inaone.png)

1. Si aprirà una nuova finestra. Fare clic su **[!UICONTROL Browse]**, quindi selezionare il file di account denominati che si desidera importare.

   ![](assets/inatwo.png)

   >[!TIP]
   >
   >Nel file, fornisci [quante più informazioni possibile](/help/marketo/product-docs/target-account-management/target/named-accounts/named-account-overview.md#named-account-attributes). È possibile aggiungere solo informazioni firmografiche; nulla viene calcolato da Marketo (ad esempio, pipeline). Per creare account denominati basati su account CRM, è sufficiente esportare il nome account e l’ID CRM dal CRM in un file CSV, utilizzare l’opzione Nome account e mappare l’ID CRM durante il processo di importazione. Per collegare correttamente un account CRM a un account denominato, è necessario fornire il nome esatto dell&#39;account CRM.

1. È possibile scegliere tra due modalità di deduplicazione: Nome account o Nome dominio. In questo esempio sceglieremo Account. Fare clic sul menu a discesa **[!UICONTROL Modes]** e selezionare **[!UICONTROL By Account Name]**.

   ![](assets/inathree.png)

   >[!NOTE]
   >
   >Se si sceglie **[!UICONTROL By Domain Name]**, è necessario includere sia il campo account denominato che il campo dominio.

1. Per scegliere l&#39;elenco di account a cui aggiungere l&#39;account denominato, fare clic sull&#39;elenco a discesa **[!UICONTROL Account List]** e selezionare l&#39;account desiderato.

   ![](assets/inafour.png)

   >[!NOTE]
   >
   >È inoltre possibile creare un [!UICONTROL Account List] nuovo digitandone semplicemente il nome nella casella a discesa.

1. Per inviare una notifica dell&#39;importazione, fare clic sul menu a discesa **[!UICONTROL Send Alert To]** e selezionare un utente Marketo. _impossibile_ immettere manualmente un indirizzo e-mail.

   ![](assets/inafive-2.png)

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/inasix-2.png)

1. Mappare ogni campo facendo doppio clic sull&#39;elenco a discesa **[!UICONTROL Marketo Field]** e selezionando il campo appropriato. Al termine, fai clic su **[!UICONTROL Next]**.

   ![](assets/inaseven.png)

   Operazione completata.

   ![](assets/inanine.png)

   >[!NOTE]
   >
   >&quot;Controlla stato importazione&quot; mostra solo gli ultimi tre giorni di attività.

Scenari durante la deduplicazione di [!UICONTROL by Account Name]:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importazione del record con il nome <span class="uicontrol">Account denominato</span> esistente</strong></td> 
   <td><p>Il record esistente verrà aggiornato</p></td> 
  </tr> 
  <tr> 
   <td><strong>Importazione del record con il nuovo nome <span class="uicontrol">Account denominato</span></strong></td> 
   <td>Verrà creato un nuovo record</td> 
  </tr> 
 </tbody> 
</table>

Scenari durante la deduplicazione di [!UICONTROL by Domain Name]:

<table> 
 <tbody> 
  <tr> 
   <td><strong>Importazione di record con un nuovo nome account e un nuovo nome dominio</strong></td> 
   <td>Verrà creato un nuovo <span class="uicontrol">account denominato</span> con le informazioni fornite</td> 
  </tr> 
  <tr> 
   <td><strong>Importazione del record con un nome account e un nome dominio esistenti</strong></td> 
   <td>Verrà aggiornato l'account denominato <span class="uicontrol">esistente</span></td> 
  </tr> 
   <tr> 
   <td><strong>Importazione del record con un nuovo nome account e un nome dominio esistente</strong></td> 
   <td>Il nuovo nome account verrà aggiunto al <span class="uicontrol">Account denominato</span> esistente che corrisponde al nome di dominio e aggiornerà altre informazioni (ad esempio, Industria, Stato, ecc.)</td> 
  </tr> 
  <tr> 
   <td><strong>Importazione record con nome <span class="uicontrol">Account denominato</span> esistente e nuovo nome dominio</strong></td> 
   <td>Il nuovo nome di dominio verrà aggiunto all'<span class="uicontrol">account denominato</span> esistente che corrisponde al nome dell'account e aggiornerà altre informazioni (ad esempio, settore, stato e così via)</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando Marketo aggiunge un account con nome, si aggiorna una regola (dietro le quinte) che consente di identificare le persone che dovrebbero far parte di [!UICONTROL Named Account]. Esempio: se aggiorni &quot;IBM&quot; a &quot;IBM, USA&quot;, le persone con uno dei due nomi di società saranno associate a [!UICONTROL Named Account].

Se Marketo trova record che consideriamo duplicati, elaborerà solo il primo.
