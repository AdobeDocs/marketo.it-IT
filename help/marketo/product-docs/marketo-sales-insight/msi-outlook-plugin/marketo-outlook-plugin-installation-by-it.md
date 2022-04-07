---
unique-page-id: 11382815
description: Installazione di Marketo Outlook Plugin da parte di IT - Marketo Docs - Documentazione del prodotto
title: Installazione di Marketo Outlook Plugin da parte di IT
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Installazione di Marketo Outlook Plugin da parte di IT {#marketo-outlook-plugin-installation-by-it}

A volte i criteri aziendali richiedono che il team IT installi tutti i software sui computer dei propri dipendenti. In questi casi, l&#39;IT spesso lo fa in remoto utilizzando il proprio software di distribuzione. Questo documento fornisce le righe di comando da utilizzare come input durante il processo di distribuzione per installare in remoto il plug-in outlook.

>[!PREREQUISITES]
>
>[Configurazione](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la chiave Enterprise.

Esegui la seguente riga di comando come account utente &quot;System&quot; o &quot;Administrative&quot; con lo switch /i da installare.

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

Per specificare una posizione dei file di registro, è possibile specificare il percorso del file nella riga di comando.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Esempio**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Il percorso di archiviazione del file di registro deve esistere o l&#39;installazione verrà interrotta.

Fai riferimento a [Elenco completo degli switch di Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) per provare diversi livelli di registrazione o di interfaccia utente.

>[!MORELIKETHIS]
>
>[Disinstallazione di Marketo Outlook Plugin da parte di IT](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
