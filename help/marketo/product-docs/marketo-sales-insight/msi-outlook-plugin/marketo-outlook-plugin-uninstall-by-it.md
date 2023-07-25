---
unique-page-id: 11382829
description: Disinstallazione del plug-in di Marketo Outlook da parte dell’IT - Documentazione di Marketo - Documentazione del prodotto
title: Disinstallazione del plug-in di Marketo Outlook da parte dell'IT
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 0%

---

# Disinstallazione del plug-in di Marketo Outlook da parte dell&#39;IT {#marketo-outlook-plugin-uninstall-by-it}

Per disinstallare il plug-in di Marketo Outlook in remoto, procedere come segue.

Eseguire la riga di comando seguente come account di sistema o account utente amministrativo con l&#39;opzione /x per disinstallare.

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

Per specificare un percorso per i file di registro, è possibile specificare il percorso del file nella riga di comando.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>La disinstallazione del plug-in in remoto comporta la chiusura forzata di Outlook nel computer dell&#39;utente.

Fare riferimento a [Elenco completo degli switch di Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) per provare diversi livelli di registrazione o di interfaccia utente.
