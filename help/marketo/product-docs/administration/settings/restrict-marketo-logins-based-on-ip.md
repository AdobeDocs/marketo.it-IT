---
unique-page-id: 2360297
description: Limitare gli accessi Marketo basati su IP - Documentazione Marketo - Documentazione del prodotto
title: Limita gli accessi a Marketo in base all’IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: b4bd06d3e5ee205744478e0f5556f490f9f5abe4
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Limita gli accessi a Marketo in base all’IP {#restrict-marketo-logins-based-on-ip}

Puoi limitare o consentire agli utenti di accedere a Marketo in base ai loro indirizzi IP. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>Le informazioni contenute in questo articolo sono destinate agli utenti che accedono direttamente a login.marketo.com e non sono applicabili a coloro che effettuano l’autenticazione con Adobe ID. Al momento non è possibile applicare restrizioni IP agli accessi Single Sign-On (SSO).

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/restrict-marketo-logins-based-on-ip-1.png)

1. Clic **[!UICONTROL Impostazioni di accesso]**.

   ![](assets/restrict-marketo-logins-based-on-ip-2.png)

1. Clic **[!UICONTROL Modifica restrizioni IP]**.

   ![](assets/restrict-marketo-logins-based-on-ip-3.png)

1. Scegli se desideri **Consenti** o **Blocca** indirizzi specifici, inserisci gli indirizzi, quindi fai clic su **[!UICONTROL Salva]**.

   >[!NOTE]
   >
   >**Definizione**
   >
   >* **[!UICONTROL Indirizzi IP consentiti]**: l’aggiunta di indirizzi IP consentiti è inclusiva. Includerà tutti gli indirizzi IP specificati ed escluderà tutto il resto.
   >* **[!UICONTROL Blocca indirizzi IP]**: impedisce a IP specifici di accedere a Marketo.
   >* **[!UICONTROL Disabilita restrizioni IP]**: selezionando questa opzione, tutte le regole di restrizione non funzioneranno più. Utilizzalo a scopo di test.

   >[!NOTE]
   >
   >È possibile aggiungere più restrizioni, ma queste possono essere solo TUTTE consentite o TUTTE bloccate. Non puoi combinare e abbinare ciò che è consentito e ciò che è bloccato.

   ![](assets/restrict-marketo-logins-based-on-ip-4.png)

   Ben fatto, i tuoi dati di marketing sono ora più sicuri di quanto non lo siano mai stati!
