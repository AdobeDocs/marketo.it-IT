---
unique-page-id: 15695924
description: Ranking e Tuning del profilo dell'account - Marketo Docs - Documentazione del prodotto
title: Classificazione e ottimizzazione profilo account
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---


# Classificazione e ottimizzazione profilo account {#account-profiling-ranking-and-tuning}

Il profilo dell&#39;account identifica il profilo cliente ideale (ICP), classifica le società nel database in base all&#39;ICP e aggiunge i dati dell&#39;indicatore ICP agli account promossi come Account denominati.

## Risultati modello {#model-results}

I risultati mostrano tutti gli account noti suddivisi per grado. A è il grado più alto, D è il più basso.

![](assets/results.png)

Anche se opzionale, si consiglia di selezionare la casella di controllo Promuovi automaticamente, in quanto consente di risparmiare un sacco di tempo. Tuttavia, se si desidera esaminare ciascun account e [aggiungerlo manualmente](/help/marketo/product-docs/account-based-marketing/target/named-accounts/discover-accounts.md#discover-crm-accounts), è sufficiente lasciare deselezionata la casella.

<table> 
 <tbody> 
  <tr> 
   <td><strong>Classifica</strong></td> 
   <td> 
    <div>
      Classificazione account in base al profilo cliente ideale. A è la migliore, D è la meno adatta. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Propensità</strong></td> 
   <td> 
    <div>
      Incremento stimato del tasso di conversione rispetto a una selezione di conti non basata sull'ICP. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Account (%)</strong></td> 
   <td> 
    <div>
      Percentuale di conti in input modello con questo grado. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>% di base del modello</strong></td> 
   <td> 
    <div>
      Percentuale di conti in base al modello con questo grado. 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Sintonizzazione modello {#model-tuning}

Nella scheda Modello, fare clic sul pulsante Regola modello.

![](assets/two.png)

Ci sono diverse schede tra cui scegliere, consentendo una personalizzazione approfondita.

![](assets/tuning-page.png)

**Categorie indicatori**

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
   <td><strong>Progettazione</strong></td> 
   <td> 
    <div>
      Tecnologie, strutture, posizioni/assunzioni relative all'ingegneria. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Vendite</strong></td> 
   <td> 
    <div>
      Soluzioni e software per le vendite, posizioni/assunzioni relative alle vendite. 
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
      Soluzioni hardware e software, tecnologie, posizioni/cablaggio IT.
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Finanza</strong></td> 
   <td> 
    <div>
      Software di finanziamento, posizioni finanziarie/assunzioni. 
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
      Voci Forbes o Inc. o partnership aziendali. 
    </div></td> 
  </tr> 
  <tr> 
   <td><strong>Esperienza cliente e relazioni</strong></td> 
   <td> 
    <div>
      Successo del cliente e posizioni/assunzioni nelle relazioni con i clienti.
    </div></td> 
  </tr> 
 </tbody> 
</table>

Passate il puntatore del mouse sulle descrizioni di ciascuna colonna.

![](assets/tool-tip.png)

Fate clic sul menu a discesa Aggiungi indicatore ICP per inserire altri indicatori nel modello.

![](assets/add-icp.png)

Selezionando la casella Esporta è possibile visualizzare l&#39;indicatore ICP nella pagina Dettagli account denominato, nonché utilizzare l&#39;indicatore ICP selezionato come vincoli in [filtri account denominati](/help/marketo/product-docs/account-based-marketing/engage/account-filters.md).

![](assets/export.png)

>[!NOTE]
>
>Gli indicatori ICP sono inclusi come vincoli in **Membro di Account denominato** Filtri e attivatori.

Spessore indicatore è ciò che controlla il livello di importanza che ogni indicatore riceve nel modello.

![](assets/weightage.png)

Fate clic su Aggiorna modello per rendere effettive le modifiche.

![](assets/refresh-button.png)

Una volta completata l&#39;ottimizzazione del modello (dopo averlo aggiornato), tornare alla scheda Risultati modello e fare clic su **Salva e applica blocchi**.

![](assets/ranks.png)
