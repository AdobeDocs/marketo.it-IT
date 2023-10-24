---
unique-page-id: 2360219
description: Configurare una firma DKIM personalizzata - Documentazione Marketo - Documentazione del prodotto
title: Impostare una firma DKIM personalizzata
exl-id: a7c6429e-14ee-439e-9f47-1b25b98d41e7
feature: Deliverability
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Impostare una firma DKIM personalizzata {#set-up-a-custom-dkim-signature}

Per garantire un recapito messaggi di prima qualità, firmiamo automaticamente tutti i messaggi in uscita con una firma DKIM di Marketo condivisa.

>[!NOTE]
>
>Potrebbe essere necessario l’aiuto del team IT per completare alcuni dei passaggi descritti in questo articolo.

Puoi personalizzare la firma DKIM per riflettere i domini selezionati. Ecco come.

1. Vai a **Amministratore** sezione.

   ![](assets/set-up-a-custom-dkim-signature-1.png)

   >[!NOTE]
   >
   >Se imposti una firma DKIM personalizzata secondo la vecchia modalità, questa continuerà a funzionare e dovrebbe essere visualizzata qui.

1. Clic **E-mail**.

   ![](assets/set-up-a-custom-dkim-signature-2.png)

1. Fai clic su **SPF/DKIM** , quindi **Aggiungi dominio**.

   ![](assets/set-up-a-custom-dkim-signature-3.png)

1. Immetti il dominio che utilizzerai nelle e-mail Marketo come Indirizzo mittente. Scegli un selettore e una dimensione chiave. Clic **Aggiungi** al termine.

   ![](assets/set-up-a-custom-dkim-signature-4.png)

   >[!TIP]
   >
   >* È consigliabile impostare la dimensione della chiave su 2048.
   >* Se utilizzi un dominio diverso nell’indirizzo Da, verrà utilizzata la firma DKIM condivisa di Marketo.

   <table> 
   <tr>
   <td width="20%"><b>Selettore</b></td>
   <td>Stringa o identificatore univoco utilizzato per individuare la parte della chiave pubblica del record DKIM. Può trattarsi di una stringa arbitraria o di un identificatore univoco per separare e identificare lo scopo di tale chiave/record DKIM.</td>
   </tr>
   <tr> 
   <td width="20%"><b>Dimensione chiave</b></td>
   <td>Livello di protezione con cui crittografare la firma DKIM.</td>
   </tr>
   </tbody>
   </table>

   <p>

1. Invia il **Record host** e **Valore TXT** al tuo IT. Chiedere loro di creare il record e assicurarsi che venga propagato a tutti i server dei nomi associati al dominio di origine. La verifica DKIM di Marketo richiede che la chiave DKIM venga propagata a tutti i server dei nomi associati al dominio con firma DKIM.

   ![](assets/set-up-a-custom-dkim-signature-5.png)

1. Dopo aver confermato la creazione del record, torna a Marketo, seleziona il dominio e fai clic su **Controlla DNS**.

   ![](assets/set-up-a-custom-dkim-signature-6.png)

   >[!NOTE]
   >
   >Se la conferma non riesce e il reparto di IT ha creato correttamente il record, potrebbe trattarsi di una questione di propagazione DNS. Riprova più tardi.

   >[!CAUTION]
   >
   >La modifica o la rimozione del record DNS corrispondente compromette il recapito messaggi. Assicurati di eliminare la voce in Marketo prima di apportare modifiche DNS.

   Questo ti sarà di grande aiuto per il recapito dei messaggi e-mail. Dovresti ottenere la convalida che il record sia presente e corretto.
