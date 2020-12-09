---
unique-page-id: 11382815
description: Installazione plug-in di Marketo Outlook tramite l'IT - Documenti Marketo - Documentazione del prodotto
title: Installazione plug-in di Marketo Outlook da parte di IT
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Installazione plug-in di Marketo Outlook da parte di IT {#marketo-outlook-plugin-installation-by-it}

A volte i criteri aziendali richiedono che il team IT installi tutti i software sui computer dei propri dipendenti. In questi casi, l&#39;IT spesso esegue questa operazione in remoto utilizzando il proprio software di distribuzione. Questo documento fornisce le righe di comando da utilizzare come input durante il processo di distribuzione per installare in remoto il plug-in di Outlook.

>[!PREREQUISITES]
>
>[Configurare](http://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) la chiave Enterprise.

Eseguite la riga di comando seguente come &quot;System&quot; o account utente amministratore con l&#39;opzione /i da installare.  `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Per la risoluzione dei problemi, potete abilitare la registrazione per creare un file di registro di output.  `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Per specificare una posizione dei file di registro, è possibile specificare il percorso del file nella riga di comando.  `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Il percorso di memorizzazione del file di registro deve esistere o l&#39;installazione verrà interrotta.

Per provare a utilizzare livelli di accesso o interfaccia utente diversi, fare riferimento all&#39;elenco completo delle opzioni [di](https://support.microsoft.com/en-us/kb/227091) Microsoft.

>[!NOTE]
>
>**Articoli correlati**
>
>[Disinstallazione plug-in di Marketo Outlook da parte di IT](marketo-outlook-plugin-uninstall-by-it.md)

