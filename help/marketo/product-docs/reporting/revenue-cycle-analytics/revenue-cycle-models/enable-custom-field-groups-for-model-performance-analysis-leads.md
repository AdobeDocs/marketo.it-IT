---
unique-page-id: 3571890
description: Abilitare i gruppi di campi personalizzati per l’analisi delle prestazioni del modello (lead) - Documenti Marketo - Documentazione del prodotto
title: Abilitare gruppi di campi personalizzati per l’analisi delle prestazioni del modello (lead)
exl-id: 417fd74f-d8f5-477b-b633-0fdfdd68b22b
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 6%

---

# Abilitare gruppi di campi personalizzati per l’analisi delle prestazioni del modello (lead) {#enable-custom-field-groups-for-model-performance-analysis-leads}

>[!PREREQUISITES]
>
>Suddividere i campi standard o personalizzati in gruppi per la generazione di rapporti tramite l&#39;Organizer campi in Marketo. Per informazioni dettagliate, vedere [Creare gruppi di campi personalizzati tramite l&#39;Organizer campi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/field-organizers/create-custom-field-groups-using-the-field-organizer.md).

<table>
 <tbody>
  <tr>
   <td colspan="3" rowspan="1"><p align="center"><strong>In che modo l’abilitazione di un gruppo di campi personalizzato influisce su più aree di analisi in Revenue Cycle Explorer?</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Cosa succede quando...?</strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>Effetti sull'area <span class="uicontrol">Analisi prestazioni modello (lead)</span></strong></p></td>
   <td colspan="1" rowspan="1"><p><strong>Effetti sulle aree Analisi lead, Analisi campagna e Analisi opportunità</strong></p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Cosa succede quando si abilita un gruppo di campi personalizzato associato a un campo cliente potenziale o aziendale standard?</strong></p></td>
   <td colspan="1" rowspan="1"><p>Il gruppo di campi personalizzato è abilitato per la generazione di rapporti nell'area <span class="uicontrol">Analisi prestazioni modello (lead)</span></p></td>
   <td colspan="1" rowspan="1"><p>Nessun impatto</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>Cosa succede quando si abilita un gruppo di campi personalizzato associato a un campo personalizzato della persona o dell’azienda?</strong></p></td>
   <td colspan="1" rowspan="1"><p>Il gruppo di campi personalizzato è abilitato per la generazione di rapporti nell'area <span class="uicontrol">Analisi prestazioni modello (lead)</span></p></td>
   <td colspan="1" rowspan="1"><p>Il campo personalizzato è abilitato per la generazione di rapporti nelle aree Analisi lead, Analisi campagna e Analisi opportunità.</p><p><strong>NOTA:</strong> i gruppi di campi personalizzati NON sono supportati in queste aree di analisi, pertanto le associazioni dei gruppi non vengono visualizzate in Gestione cicli di ricavo.<em>solo</em> il campo personalizzato.</p></td>
  </tr>
 </tbody>
</table>

Per abilitare un gruppo di campi personalizzato per il reporting nell&#39;area [!UICONTROL Model Performance Analysis (Leads)], eseguire la procedura seguente.

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/one-1.png)

1. Fai clic su **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/two-1.png)

1. Fare clic su **[!UICONTROL None]** accanto a un gruppo di campi vuoto. Se sono già stati attivati tre gruppi di campi e si desidera apportare una modifica, fare clic sul nome del gruppo di campi che si desidera modificare.

   ![](assets/three.png)

1. Fare clic sul menu a discesa **[!UICONTROL Field]** e selezionare quello desiderato.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >In questo esempio viene abilitato un gruppo di campi personalizzato per un campo standard (State). È stata interessata solo l&#39;area [!UICONTROL Model Performance Analysis (Leads)]. Se è stato abilitato un gruppo di campi personalizzato per un campo persona o società personalizzato, il gruppo abilitato verrà visualizzato nella sezione [!UICONTROL Model Performance Analysis (Leads)] della scheda Riepilogo sincronizzazione e il conteggio dei campi personalizzati per Analisi lead, campagna e opportunità aumenterà di uno.

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/five-1.png)
