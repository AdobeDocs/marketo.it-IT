---
unique-page-id: 15695924
description: Classificazione e tuning del profilo dell'account - Documenti Marketo - Documentazione del prodotto
title: Classificazione e tuning del profilo dell'account
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Classificazione e tuning del profilo dell&#39;account {#account-profiling-ranking-and-tuning}

La profilazione dell&#39;account identifica il tuo profilo cliente ideale (ICP), classifica le aziende nel tuo database in base all&#39;ICP e aggiunge i dati dell&#39;indicatore ICP agli account promossi come Account denominati.

## Risultati modello {#model-results}

I risultati mostrano tutti gli account noti suddivisi per grado. A è il grado più alto, D è il più basso.

![](assets/results.png)

Anche se opzionale, è consigliabile selezionare la casella di controllo Promuovi automaticamente , in quanto consente di risparmiare un sacco di tempo. Tuttavia, se desideri esaminare ciascun account e [aggiungerlo manualmente](/help/marketo/product-docs/target-account-management/target/named-accounts/discover-accounts.md#discover-crm-accounts), lascia la casella deselezionata.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classificazione</strong></td> 
   <td> 
    <div>
      Classificazione dell'account in base al profilo cliente ideale. A è la migliore vestibilità, D è la meno adatta. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensione</strong></td> 
   <td> 
    <div>
      Incremento stimato del tasso di conversione rispetto a una selezione di conti non basata su ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Account (%)</strong></td> 
   <td> 
    <div>
      Percentuale di account in input modello con questo rango. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% di base del modello</strong></td> 
   <td> 
    <div>
      Percentuale di conti in base al modello con questo rango. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Ottimizzazione del modello {#model-tuning}

Nella scheda Modello fare clic sul pulsante Sintonizza modello.

![](assets/two.png)

Ci sono diverse schede tra cui scegliere, consentendo una personalizzazione approfondita.

![](assets/tuning-page.png)

**Categorie di indicatori**

<table> 
 <tbody> 
  <tr> 
   <td><strong>Conformità</strong></td> 
   <td> 
    <div>
      Certificazioni, posizioni/assunzioni relative alla conformità. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Operazioni</strong></td> 
   <td> 
    <div>
      Posizioni/assunzioni relative alle operazioni. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>HR</strong></td> 
   <td> 
    <div>
      Software HR o Payroll, posizioni/assunzioni relative alle risorse umane.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Ingegneria</strong></td> 
   <td> 
    <div>
      Tecnologie, quadri, posizioni/assunzioni relative all'ingegneria. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vendite</strong></td> 
   <td> 
    <div>
      Soluzioni e software per le vendite, posizioni relative alle vendite/assunzioni. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Intento</strong></td> 
   <td> 
    <div>
      Indicatori di intento. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>IT</strong></td> 
   <td> 
    <div>
      Soluzioni hardware e software, tecnologie, posizioni/assunzioni relative all'IT.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanza</strong></td> 
   <td> 
    <div>
      Software finanziario, posizioni finanziarie/assunzioni. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Marketing</strong></td> 
   <td> 
    <div>
      Tecnologie e software di marketing, posizioni/assunzioni relative al marketing. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Business</strong></td> 
   <td> 
    <div>
      Annunci Forbes o Inc o partnership commerciale. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Esperienza cliente e relazioni</strong></td> 
   <td> 
    <div>
      Successo del cliente e posizioni/assunzioni di relazioni con i clienti.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Passa il puntatore del mouse sulle descrizioni comandi per ottenere una descrizione di ciascuna colonna.

![](assets/tool-tip.png)

Fai clic sul menu a discesa Aggiungi indicatore ICP per inserire ulteriori indicatori nel modello.

![](assets/add-icp.png)

Selezionando la casella Esporta è possibile visualizzare l&#39;indicatore ICP nella pagina Dettagli conto denominato, nonché utilizzare l&#39;indicatore ICP selezionato come vincoli in [filtri account denominati](/help/marketo/product-docs/target-account-management/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Gli indicatori ICP sono inclusi come vincoli in **Membro di Account denominato** Filtri e Triggers.

La ponderazione dell&#39;indicatore è ciò che controlla il livello di importanza che ogni indicatore riceve nel modello.

![](assets/weightage.png)

Fare clic su Aggiorna modello per rendere effettive le modifiche.

![](assets/refresh-button.png)

Al termine della regolazione del modello (dopo averlo aggiornato), torna alla scheda Risultati modello e fai clic su **Salva e applica blocchi**.

![](assets/ranks.png)
