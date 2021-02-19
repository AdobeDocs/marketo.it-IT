---
unique-page-id: 11382829
description: Marketo Outlook Plugin Disinstallazione per IT - Marketo Docs - Documentazione del prodotto
title: Disinstallazione plug-in di Marketo Outlook da parte di IT
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Disinstallazione plug-in di Marketo Outlook da parte di IT {#marketo-outlook-plugin-uninstall-by-it}

Ecco come l&#39;IT può disinstallare il plug-in Marketo Outlook in remoto.

Eseguite la riga di comando seguente come &quot;System&quot; o un account utente amministratore con lo switch /x per la disinstallazione.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Per la risoluzione dei problemi è possibile abilitare la registrazione per creare un file di registro di output.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Per specificare una posizione dei file di registro, è possibile specificare il percorso del file nella riga di comando.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>La disinstallazione remota del plug-in comporterà la chiusura forzata di Outlook nel computer dell&#39;utente.

Fare riferimento all&#39; [elenco completo di switch di Microsoft](https://support.microsoft.com/en-us/kb/227091) se si desidera provare diversi livelli di registrazione o di interfaccia utente.
