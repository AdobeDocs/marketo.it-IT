---
unique-page-id: 11382829
description: Disinstallazione di Marketo Outlook Plugin da IT - Marketo Docs - Documentazione del prodotto
title: Disinstallazione di Marketo Outlook Plugin da parte di IT
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# Disinstallazione di Marketo Outlook Plugin da parte di IT {#marketo-outlook-plugin-uninstall-by-it}

Ecco come l&#39;IT può disinstallare il plugin di Marketo Outlook in remoto.

Esegui la seguente riga di comando come &quot;System&quot; o un account utente amministratore con l&#39;opzione /x da disinstallare.

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
>La disinstallazione remota del plug-in chiuderà forzatamente Outlook sul computer dell&#39;utente.

Fai riferimento a [Elenco completo degli switch di Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) per provare diversi livelli di registrazione o di interfaccia utente.
