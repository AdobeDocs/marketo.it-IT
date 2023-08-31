---
description: Filtraggio dell’attività bot e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Filtraggio dell’attività bot e-mail
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
feature: Email Setup
source-git-commit: 9019cb4b81fb3acd744e644d51059644af454e5e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 11%

---

# Filtraggio dell’attività bot e-mail {#filtering-email-bot-activity}

A volte, l’attività di bot su e-mail può erroneamente gonfiare le aperture delle e-mail e fare clic sui dati. Per risolvere il problema, segui la procedura riportata di seguito.

Per confermare l’attività da bot usiamo due metodi separati:

* Corrispondenza con [Elenco dei bot di Interactive Advertising Bureau](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/){target="_blank"}: le attività che corrispondono a qualcosa nell’elenco IAB UA/IP (agente utente/indirizzo IP) verranno contrassegnate come bot.
* Corrispondenza con pattern di prossimità: quando più di due attività si verificano contemporaneamente (in meno di un secondo), vengono identificate come bot. Attributi considerati durante il confronto:
   * ID lead (deve essere lo stesso)
   * Risorsa e-mail (deve essere la stessa)
   * Clic collegamento o apertura e-mail
   * Differenza di tempo (deve essere inferiore a un secondo)

A seconda del clic sul collegamento e-mail e dell’attività di apertura e-mail, i nuovi attributi verranno compilati con i valori seguenti:

* Le attività identificate come bot avranno &quot;Bot Activity&quot; come &quot;True&quot; e &quot;Bot Activity Pattern&quot; come modello/metodo identificato
* Le attività identificate come non bot avranno &quot;Bot Activity&quot; come &quot;False&quot; e &quot;Bot Activity Pattern&quot; come &quot;N/D&quot;
* Le attività che si sono verificate prima dell’introduzione di questi attributi avranno &quot;Attività bot&quot; come &quot;&quot; (vuoto) e &quot;Modello di attività bot&quot; come &quot;&quot; (vuoto)

## Seleziona tipo di filtro {#select-filter-type}

1. Clic **[!UICONTROL Amministratore]**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Clic **[!UICONTROL E-mail]**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Fai clic su **[!UICONTROL Attività bot]** scheda.

   ![](assets/filtering-email-bot-activity-3.png)

1. Scegli per **[!UICONTROL Corrispondenza con elenco IAB]**, **[!UICONTROL Corrispondenza con pattern di prossimità]**, o entrambi. Scegli se [!UICONTROL registra attività bot] _o_ [!UICONTROL attività filtro bot].

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Se si sceglie [!UICONTROL Filtra attività bot], potrebbe verificarsi un calo nelle aperture delle e-mail e nei clic quando le attività false vengono eliminate.

**PASSAGGIO FACOLTATIVO**: per disattivare questa funzione, è sufficiente deselezionare i dispositivi di scorrimento. Se si disattiva, i dati non vengono ripristinati.

>[!TIP]
>
>Sfrutta i dati di attività bot negli elenchi avanzati tramite i filtri booleani &quot;Is Bot Activity&quot; (sì/no) e &quot;Bot Activity Pattern&quot; nei filtri &quot;Clicked Link in Email&quot; (Collegamento cliccato in e-mail) e &quot;Open Email&quot; (Apri e-mail) e i trigger &quot;Clicks Link in Email&quot; (Collegamento clic in e-mail) e &quot;Opens Email&quot; (Apri e-mail).

## INSERIRE NELL&#39;ELENCO BLOCCATI IP {#ip-blocklist}

Abbiamo compilato un elenco di indirizzi IP responsabili della generazione di milioni di falsi impegni, in quanto tali impegni ricevuti da uno qualsiasi dei seguenti IP vengono automaticamente filtrati e non aggiunti all’istanza di Marketo Engage. Questo può comportare una riduzione delle aperture delle e-mail, dei clic e di altre attività correlate. L&#39;elenco in appresso può essere aggiornato periodicamente.

* 40.94.34.52
* 40.94.34.86
* 52.34.76.65
* 54.70.53.60
* 54.71.187.124
* 60.28.2.248
* 64.235.150.252
* 64.235.153.10
* 64.235.153.2
* 64.235.154.105
* 64.235.154.109
* 64.235.154.140
* 64.74.215.1
* 64.74.215.100
* 64.74.215.138
* 64.74.215.139
* 64.74.215.142
* 64.74.215.146
* 64.74.215.150
* 64.74.215.154
* 64.74.215.158
* 64.74.215.162
* 64.74.215.164
* 64.74.215.166
* 64.74.215.170
* 64.74.215.174
* 64.74.215.176
* 64.74.215.178
* 64.74.215.51
* 64.74.215.56
* 64.74.215.58
* 64.74.215.59
* 64.74.215.86
* 64.74.215.98
* 65.154.226.101
* 66.249.91.149
* 70.42.131.106
* 74.125.217.116
* 74.217.90.250
* 104.129.41.4
* 104.47.55.126
* 104.47.58.126
* 104.47.70.126
* 104.47.73.126
* 104.47.73.254
* 104.47.74.126
* 128.220.160.1
* 155.70.39.101
* 162.129.251.14
* 162.129.251.42
* 208.52.157.204

>[!NOTE]
>
>Analizziamo e analizziamo meticolosamente ogni indirizzo IP prima di aggiungerlo a questo elenco, assicurandoci che vengano bloccati solo gli IP più critici e dannosi.
