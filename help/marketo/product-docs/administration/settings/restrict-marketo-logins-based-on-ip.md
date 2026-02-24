---
unique-page-id: 2360297
description: Limitare gli accessi Marketo basati su IP - Documentazione Marketo - Documentazione del prodotto
title: Limitare gli accessi a Marketo in base all’IP
exl-id: 5d9d0b88-b4bc-4e1b-b70c-2c2e7b4269f5
feature: Administration
source-git-commit: b6680c404075f13b1713ce28299e60a4d26f4a06
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 10%

---

# Limitare gli accessi a Marketo in base all’IP {#restrict-marketo-logins-based-on-ip}

Puoi limitare o consentire agli utenti di accedere a Marketo in base ai loro indirizzi IP. Ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>Adobe Admin Console (AAC) supporta [il controllo degli accessi basato su IP](https://helpx.adobe.com/it/enterprise/using/ip-based-access.html){target="_blank"}. Per garantire una transizione senza problemi, le restrizioni IP di Marketo Engage esistenti saranno attive, tra cui gli utenti di Adobe ID fino al primo trimestre del 2027 negli abbonamenti in cui questa funzione è abilitata.
>
>* È possibile configurare l&#39;accesso basato su IP AAC in qualsiasi momento.
>* Le restrizioni AAC e Marketo Engage possono essere eseguite contemporaneamente. Utilizza lo stesso elenco consentiti IP per la compatibilità.
>
>Dopo il primo trimestre del 2027, le restrizioni IP di Marketo Engage verranno ritirate. L’accesso basato su IP verrà gestito esclusivamente tramite AAC e deve essere configurato in modo da applicare le restrizioni di accesso. La data finale della transizione verrà annunciata in seguito.

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
