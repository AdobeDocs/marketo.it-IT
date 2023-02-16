---
unique-page-id: 2360297
description: Limitare gli accessi a Marketo in base a IP - Marketo Docs - Documentazione del prodotto
title: Limitare gli accessi Marketo in base all’IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
source-git-commit: bd6f049d5959356a99314e81bb6cfe517c2efdfa
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Limitare gli accessi Marketo in base all’IP {#restrict-marketo-logins-based-on-ip}

È possibile limitare o consentire agli utenti di accedere a Marketo in base ai loro indirizzi IP. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Le informazioni contenute in questo articolo si applicano solo agli accessi diretti all’indirizzo login.marketo.com. Al momento non è possibile applicare restrizioni IP agli accessi single sign-on (SSO).

1. Vai a **Amministratore** area.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Fai clic su **Impostazioni di accesso**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Fai clic su **Modifica restrizioni IP**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Scegli se desideri **Consenti** o **Blocco** indirizzi specifici, inserisci gli indirizzi e fai clic su **Salva**.

   >[!NOTE]
   >
   >**Definizione**
   >
   >* **Indirizzi IP consentiti**: L’aggiunta di indirizzi IP consentiti è inclusiva. Includerà tutti gli indirizzi IP specificati ed escluderà tutto il resto.
   >* **Blocca indirizzi IP**: Impedisce l’accesso a Marketo a IP specifici.
   >* **Disabilita restrizioni IP**: Il controllo interrompe il funzionamento di tutte le regole di restrizione. Utilizzalo a scopo di test.


   >[!NOTE]
   >
   >È possibile aggiungere più restrizioni, ma possono essere bloccate solo tutte o TUTTE. Non è possibile combinare e abbinare consentito e bloccato.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Ben fatto, i tuoi dati di marketing sono ora più sicuri di quanto non siano mai stati!
