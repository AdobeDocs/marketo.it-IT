---
description: Iscriviti alle notifiche di stato del sistema - Documentazione di Marketo Engage - Documentazione del prodotto
title: Iscriviti alle notifiche di stato del sistema
feature: Getting Started
hide: true
hidefromtoc: true
source-git-commit: cf60167b9e9ee2ea2a2861a3cd3c661781dbf0b0
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Iscriviti alle notifiche di stato del sistema {#subscribe-to-system-status-notifications}

TESTO INTRODUTTIVO

>[!PREREQUISITES]
>
>Prima di creare una sottoscrizione, è necessario identificare il centro dati e il pod/server in cui si trova la sottoscrizione.

## Identificazione del centro dati {#identify}

+++Identificazione del centro dati e del pod/server

1. Nella sezione **Amministratore** di Marketo Engage, fai clic su **Il mio account**.

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. Scorri verso il basso fino a _Informazioni di supporto_.

   ![](assets/subscribe-to-system-status-notifications-2.png)

Nel campo _Data center_, le lettere sono il data center e i numeri sono il pod. Nell’esempio precedente, l’utente si trova nel nostro data center Ashburn sul pod 49.

Nel passaggio 7 di [creazione di una sottoscrizione](#create-a-subscription), questo utente selezionerà il percorso regionale **Marketo Ashburn** e il pod **ab49**.

<table style="width:225px;">
  <tr>
    <th colspan="2">Abbreviazioni data center</th>
  </tr>
  <tr>
    <td style="width:25%;">ab</td>
    <td>Ashburn</td>
  </tr>
  <tr>
    <td style="width:25%;">sj</td>
    <td>San Jose</td>
  </tr>
  <tr>
    <td style="width:25%;">sn</td>
    <td>Sydney</td>
  </tr>
  <tr>
    <td style="width:25%;">lon</td>
    <td>Londra</td>
  </tr>
  <tr>
    <td style="width:25%;">nld</td>
    <td>Amsterdam</td>
  </tr>
</table>

>[!TIP]
>
>Questo metodo può essere utilizzato anche per identificare il pod/server Real Time Personalization (RTP) in cui si trova l’abbonamento.

+++

## Creare una sottoscrizione {#create-a-subscription}

Dopo [aver identificato il centro dati e il pod/server](#identify), eseguire la procedura seguente per creare una sottoscrizione.

1. In [status.adobe.com](https://status.adobe.com/it), fai clic su **Gestisci sottoscrizioni**.

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. Accedi (se non lo hai già fatto) utilizzando le tue credenziali Adobe oppure fai clic su **Crea un account** se non ne hai uno.

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. Rimani nella scheda _Descrizioni prodotto_ e fai clic su **Crea abbonamenti**.

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. Fai clic sull&#39;icona ![segno più](assets/icon-plus-sign.png) accanto a _Experience Cloud_ per espandere il menu. Eseguire la stessa operazione per _Adobe Marketo Engage_.

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800" zoomable="yes"}

1. Selezionare le offerte di prodotti e i servizi desiderati per i quali si desidera ricevere notifiche e fare clic su **Continua**.

   >[!TIP]
   >
   >Seleziona _Adobe Marketo Engage_ per selezionare tutti.

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800" zoomable="yes"}

1. Seleziona i tipi di evento desiderati.

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:600px;">
   <tr>
   <td style="width:30%;"><b>Problema del servizio grave</b></td>
   <td>Indisponibilità del servizio o grave deterioramento delle prestazioni per più utenti sui sistemi di produzione.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Problema del servizio non grave</b></td>
   <td>Indisponibilità parziale del servizio o moderato peggioramento delle prestazioni per più utenti sui sistemi di produzione.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Manutenzione del servizio</b></td>
   <td>Testo</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Annunci</b></td>
   <td>Annunci relativi a...</td>
   </tr>
   </table>

1. Seleziona la località geografica e l’ambiente desiderati. Fai clic su **Continua**.

   ![](assets/subscribe-to-system-status-notifications-9.png){width="800" zoomable="yes"}

1. Scegli la tua preferenza di abbonamento, **E-mail** o **Slack**, quindi fai clic su **Continua**.

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. Rivedi le tue selezioni e fai clic su **Conferma preferenze**.

   ![](assets/subscribe-to-system-status-notifications-11.png)
