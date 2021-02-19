---
unique-page-id: 11382815
description: Installazione plug-in di Marketo Outlook tramite l'IT - Documenti Marketo - Documentazione del prodotto
title: Installazione plug-in di Marketo Outlook da parte di IT
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---


# Installazione del plug-in di Microsoft Outlook Marketo da parte di IT {#marketo-outlook-plugin-installation-by-it}

A volte i criteri aziendali richiedono che il team IT installi tutti i software sui computer dei propri dipendenti. In questi casi, l&#39;IT spesso esegue questa operazione in remoto utilizzando il proprio software di distribuzione. Questo documento fornisce le righe di comando da utilizzare come input durante il processo di distribuzione per installare in remoto il plug-in di Outlook.

>[!PREREQUISITES]
>
>[Impostare ](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la chiave Enterprise.

Eseguite la riga di comando seguente come &quot;System&quot; o account utente amministratore con l&#39;opzione /i da installare.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Per la risoluzione dei problemi, potete abilitare la registrazione per creare un file di registro di output.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Per specificare una posizione dei file di registro, è possibile specificare il percorso del file nella riga di comando.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Il percorso di memorizzazione del file di registro deve esistere o l&#39;installazione verrà interrotta.

Fare riferimento all&#39; [elenco completo di switch di Microsoft](https://support.microsoft.com/en-us/kb/227091) se si desidera provare diversi livelli di registrazione o di interfaccia utente.

>[!MORELIKETHIS]
>
>[Disinstallazione plug-in di Marketo Outlook da parte di IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
