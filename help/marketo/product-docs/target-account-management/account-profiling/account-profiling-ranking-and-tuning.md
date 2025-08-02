---
unique-page-id: 15695924
description: Classificazione e ottimizzazione della profilatura dell’account - Documentazione di Marketo - Documentazione del prodotto
title: Classificazione e tuning profilo account
exl-id: 9c5d0a03-0ebe-43cc-95ef-faab19a7f673
feature: Target Account Management
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Classificazione e tuning profilo account {#account-profiling-ranking-and-tuning}

Il profilo account identifica il profilo cliente ideale (ICP), classifica le aziende nel database in base all&#39;ICP e aggiunge i dati degli indicatori ICP agli account promossi come [!UICONTROL Named Accounts].

>[!IMPORTANT]
>
>A partire dal 2025, la profilazione degli account non è più disponibile per i nuovi utenti. Continuerà a funzionare per gli utenti esistenti.

## Risultati modello {#model-results}

I risultati mostrano tutti i tuoi account noti suddivisi per livello. A è il grado più alto, D è il più basso.

![](assets/results.png)

Anche se facoltativo, è consigliabile selezionare la casella di controllo Promuovi automaticamente in quanto consente di risparmiare molto tempo. Tuttavia, se desideri esaminare ogni account e [aggiungerlo manualmente](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), lascia la casella deselezionata.

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Classifica</span></strong></td>
   <td>
    <div>
      Classificazione dell’account in base al profilo cliente ideale. A è la misura migliore, D è la misura minore.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Propensione</span></strong></td>
   <td>
    <div>
      Aumento stimato del tasso di conversione rispetto a una selezione di conti non basata su ICP.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Account (%)</span></strong></td>
   <td>
    <div>
      Percentuale di conti in input modello con questa classificazione.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">% della base del modello</span></strong></td>
   <td>
    <div>
      Percentuale di conti in base a modello che hanno questa classificazione.
    </div></td>
  </tr>
 </tbody>
</table>

## Regolazione modello {#model-tuning}

Nella scheda Modello fare clic sul pulsante **[!UICONTROL Tune Model]**.

![](assets/two.png)

Sono disponibili diverse schede tra cui scegliere, che consentono una personalizzazione approfondita.

![](assets/tuning-page.png)

**Categorie indicatore**

<table>
 <tbody>
  <tr>
   <td><strong><span class="uicontrol">Conformità</span></strong></td>
   <td>
    <div>
      Certificazioni, posizioni relative alla conformità/assunzione.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Operazioni</span></strong></td>
   <td>
    <div>
      Posizioni/assunzioni legate alle operazioni.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">ORE</span></strong></td>
   <td>
    <div>
      Software HR o Payroll, posizioni/assunzioni relative alle risorse umane.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Progettazione</span></strong></td>
   <td>
    <div>
      Tecnologie, quadri di riferimento, posizioni/assunzioni correlate all'ingegneria.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Vendite</span></strong></td>
   <td>
    <div>
      Soluzioni e software per la vendita, posizioni di vendita/noleggio.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Intento</span></strong></td>
   <td>
    <div>
      Indicatori di intento.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">IT</span></strong></td>
   <td>
    <div>
      Soluzioni hardware e software, tecnologie, posizioni/assunzioni relative all'IT.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Finanza</span></strong></td>
   <td>
    <div>
      Software finanziario, posizioni finanziarie/assunzioni.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Marketing</span></strong></td>
   <td>
    <div>
      Tecnologie e software di marketing, posizioni di marketing/noleggio.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Business</span></strong></td>
   <td>
    <div>
      Inserzioni o partnership commerciali con Forbes o Inc.
    </div></td>
  </tr>
  <tr>
   <td><strong><span class="uicontrol">Esperienza cliente e relazioni</span></strong></td>
   <td>
    <div>
      Posizioni/assunzioni relative a relazioni con i clienti e successo del cliente.
    </div></td>
  </tr>
 </tbody>
</table>

Passa il cursore del mouse sulle descrizioni per visualizzare una descrizione di ciascuna colonna.

![](assets/tool-tip.png)

Fare clic sul menu a discesa [!UICONTROL Add ICP Indicator] per inserire indicatori aggiuntivi nel modello.

![](assets/add-icp.png)

La selezione della casella [!UICONTROL Export] consente di visualizzare l&#39;indicatore ICP nella pagina dei dettagli [!UICONTROL Named Account] e di utilizzare l&#39;indicatore ICP selezionato come vincoli nei [filtri account denominati](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Gli indicatori ICP sono inclusi come vincoli nei filtri e trigger **[!UICONTROL Member of Named Account]**.

[!UICONTROL Indicator Weightage] è ciò che controlla il livello di importanza che ogni indicatore riceve nel modello.

![](assets/weightage.png)

Fare clic su **[!UICONTROL Refresh Model]** per rendere effettive le modifiche.

![](assets/refresh-button.png)

Al termine dell&#39;ottimizzazione del modello (dopo averlo aggiornato), tornare alla scheda Risultati modello e fare clic su **[!UICONTROL Save & Apply Ranks]**.

![](assets/ranks.png)
