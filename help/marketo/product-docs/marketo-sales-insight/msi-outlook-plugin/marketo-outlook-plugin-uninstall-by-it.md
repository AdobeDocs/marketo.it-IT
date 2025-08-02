---
unique-page-id: 11382829
description: Disinstallazione del plug-in Marketo [!DNL Outlook] da parte dell'IT - Documentazione di Marketo - Documentazione del prodotto
title: Disinstallazione del plug-in Marketo [!DNL Outlook] da parte dell'IT
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '114'
ht-degree: 2%

---

# Disinstallazione del plug-in di Marketo [!DNL Outlook] da parte dell&#39;IT {#marketo-outlook-plugin-uninstall-by-it}

Ecco come il reparto IT può disinstallare il plug-in di Marketo [!DNL Outlook] in remoto.

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
>La disinstallazione remota del plug-in determinerà la chiusura forzata di [!DNL Outlook] nel computer dell&#39;utente.

Fare riferimento all&#39;[elenco completo degli switch di Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) se si desidera provare livelli di registrazione o di interfaccia utente diversi.
