---
unique-page-id: 2360297
description: Limitare gli accessi Marketo basati su IP - Documentazione Marketo - Documentazione del prodotto
title: Limitare gli accessi a Marketo in base all’IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 11%

---

# Limitare gli accessi a Marketo in base all’IP {#restrict-marketo-logins-based-on-ip}

Puoi limitare o consentire agli utenti di accedere a Marketo in base ai loro indirizzi IP. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo sono destinate agli utenti che accedono direttamente a login.marketo.com e non sono applicabili a coloro che effettuano l’autenticazione con Adobe ID. Al momento non è possibile applicare restrizioni IP agli accessi Single Sign-On (SSO).

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Fai clic su **[!UICONTROL Login Settings]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Fai clic su **[!UICONTROL Edit IP Restrictions]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Scegli se desideri **Consentire** o **Bloccare** indirizzi specifici, immetti gli indirizzi, quindi fai clic su **[!UICONTROL Save]**.

   >[!NOTE]
   >
   >**Definizione**
   >
   >* **[!UICONTROL Allowed IP addresses]**: l&#39;aggiunta di indirizzi IP consentiti è inclusiva. Includerà tutti gli indirizzi IP specificati ed escluderà tutto il resto.
   >* **[!UICONTROL Block IP addresses]**: impedisce a IP specifici di accedere a Marketo.
   >* **[!UICONTROL Disable IP Restrictions]**: la selezione di questa opzione interromperà il funzionamento di tutte le regole di restrizione. Utilizzalo a scopo di test.

   >[!NOTE]
   >
   >È possibile aggiungere più restrizioni, ma queste possono essere solo TUTTE consentite o TUTTE bloccate. Non puoi combinare e abbinare ciò che è consentito e ciò che è bloccato.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Ben fatto, i tuoi dati di marketing sono ora più sicuri di quanto non lo siano mai stati!
