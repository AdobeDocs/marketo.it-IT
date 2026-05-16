---
unique-page-id: 11382815
description: Scopri come il reparto IT può installare il plug-in di Marketo Outlook per l’organizzazione. Distribuire il componente aggiuntivo su larga scala per gli utenti di Outlook.
title: Installazione del plug-in Marketo [!DNL Outlook] da parte dell'IT
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/7Gq4FJlVf9jvqL2Bz34oQVL8HtBNYCjEHl32g-0RXYk
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 195
ht-degree: 1%

---

# Installazione del plug-in Marketo [!DNL Outlook] da parte dell&#39;IT {#marketo-outlook-plugin-installation-by-it}

A volte le politiche aziendali richiedono che il team IT installi tutto il software sui computer dei dipendenti. In questi casi, spesso l&#39;IT esegue questa operazione in remoto utilizzando il proprio software di distribuzione. Questo documento fornisce le righe di comando da utilizzare come input durante il processo di distribuzione per installare il plug-in di Outlook in modalità remota.

>[!PREREQUISITES]
>
>[Configura](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la chiave Enterprise.

Eseguire la seguente riga di comando come account utente &quot;System&quot; o Amministratore con l&#39;opzione /i per installare.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Per la risoluzione dei problemi, è possibile abilitare la registrazione per creare un file di registro di output.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Per specificare un percorso per i file di registro, è possibile specificare il percorso del file nella riga di comando.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Il percorso di archiviazione del file di registro deve esistere o l&#39;installazione verrà interrotta.

Fare riferimento a [Elenco completo di opzioni di Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) se si desidera provare livelli di registrazione o di interfaccia utente diversi.

>[!MORELIKETHIS]
>
>[Marketo [!DNL Outlook] Disinstallazione del plug-in da parte dell&#39;IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
