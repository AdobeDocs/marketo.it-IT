---
description: Gestione di utenti e licenze - Documentazione di Marketo - Documentazione del prodotto
title: Gestione di utenti e licenze
exl-id: 1fee628b-e9f3-46ab-b993-f2d09fe5e183
feature: Interactive Webinars
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# Gestione di utenti e licenze {#user-and-license-management}

Scopri come aggiungere e rimuovere utenti e visualizzare le licenze correnti.

## Aggiungi un utente {#add-a-user}

1. Vai a **Amministratore** area.

   ![](assets/user-and-license-management-1.png)

1. Clic **Webinar interattivi**.

   ![](assets/user-and-license-management-2.png)

1. Clic **Aggiungi/Rimuovi utenti**.

   ![](assets/user-and-license-management-3.png)

1. Fai clic sul menu a discesa Utenti disponibili, seleziona gli utenti da aggiungere e fai clic su **OK**.

   ![](assets/user-and-license-management-4.png)

## Rimuovi un utente {#remove-a-user}

1. Vai a **Amministratore** area.

   ![](assets/user-and-license-management-5.png)

1. Clic **Webinar interattivi**.

   ![](assets/user-and-license-management-6.png)

1. Clic **Aggiungi/Rimuovi utenti**.

   ![](assets/user-and-license-management-7.png)

1. Evidenziare gli utenti che si desidera rimuovere e premere il tasto Canc sulla tastiera. Clic **OK** al termine.

   ![](assets/user-and-license-management-8.png)

## Utilizzo licenze {#license-usage}

I webinar interattivi offrono licenze specifiche per la creazione di eventi basati su Adobe Connect. Ogni volta che viene aggiunta una licenza, viene visualizzata una nuova casella di utilizzo della licenza. Gli amministratori di Marketo possono visualizzare (non modificare) le licenze seguendo la procedura riportata di seguito. Contatta l’Adobe Account Team (il tuo Account Manager) per ottenere ulteriori licenze.

1. Vai a **Amministratore** area.

   ![](assets/user-and-license-management-9.png)

1. Clic **Webinar interattivi**.

   ![](assets/user-and-license-management-10.png)

1. Scorri verso il basso fino alle schede Utilizzo licenze.

   ![](assets/user-and-license-management-11.png)

<table> 
  <tr> 
   <td><b>Data inizio</b></td>
   <td>Data di inizio della licenza.</td>
  </tr>
  <tr> 
   <td><b>Data di scadenza</b></td>
   <td>Data di scadenza della licenza.</td>
  </tr>
  <tr> 
   <td><b>Tipo</b></td>
   <td>Tipo di licenza acquistata. Sono disponibili tre tipi di licenza: Shared Events License, Shared Rooms License, Additional Storage License.</td>
  </tr>
  <tr> 
   <td><b>Capacità evento</b></td>
   <td>Il numero massimo di partecipanti che possono essere ospitati in un evento.</td>
  </tr>
  <tr> 
   <td><b>Eventi totali</b></td>
   <td>Numero totale di eventi per i quali è stato eseguito il provisioning con questa licenza.</td>
  </tr>
  <tr> 
   <td><b>Eventi utilizzati</b></td>
   <td>Numero totale di eventi completati.</td>
  </tr>
  <tr> 
   <td><b>Capacità di archiviazione</b></td>
   <td>Quantità di storage disponibile per l'archiviazione di registrazioni, materiale collaterale, heri images, documentazione e altre risorse.</td>
  </tr>
  </tbody>
</table>

**Aspetti da considerare**

* Il tipo &quot;Licenza di archiviazione aggiuntiva&quot; fornisce solo storage, pertanto il valore in ogni campo _oltre a_ La capacità di storage verrà elencata semplicemente come &quot;-&quot;.

* Il tipo &quot;Shared Room License&quot; ha eventi illimitati e &quot;Additional Storage License&quot; fornisce solo storage, pertanto il campo Total Events (Eventi totali) per queste licenze verrà elencato semplicemente come &quot;-&quot;.

* Ogni volta che un evento viene creato, verrà conteggiato come &quot;consumato&quot; dalla rispettiva licenza (a meno che non si tratti di una licenza per sala condivisa). La preferenza verrà data a &quot;Shared Event License&quot; se sono presenti sia &quot;Shared Event License&quot; che &quot;Shared Room License&quot; della stessa capacità. Se l&#39;evento non è stato consegnato e il programma eventi viene eliminato prima dell&#39;ora pianificata, il conteggio degli eventi viene rifornito sottraendo un evento dagli eventi consumati.

* Una volta esaurita la licenza, il riquadro rimane nella schermata Webinar interattivi della sezione Amministratore con &quot;Eventi totali&quot; e &quot;Eventi consumati&quot; che hanno lo stesso valore. La licenza verrà rimossa dalla schermata solo alla scadenza.
