---
description: Sincronizzazione campi personalizzati membro del programma - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione campo personalizzato del membro del programma
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 9%

---

# Sincronizzazione campo personalizzato del membro del programma {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Creazione di [campi personalizzati membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Sincronizza una  [!DNL Salesforce] campagna con un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>L&#39;oggetto Membro del programma può contenere fino a 20 campi personalizzati. Questi campi sono disponibili per qualsiasi programma.

## Mappa campi Salesforce ai campi personalizzati dei membri del programma {#map-salesforce-fields-to-program-member-custom-fields}

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Fare clic su **[!DNL Salesforce]**, quindi fare clic su **[!UICONTROL Edit]** accanto a Sincronizzazione campi personalizzati membro del programma.

   ![](assets/program-member-custom-field-sync-2.png)

1. Utilizzare la casella di ricerca per individuare i campi [!DNL Salesforce] da mappare. In questo esempio, utilizziamo Do Not Call.

   ![](assets/program-member-custom-field-sync-3.png)

1. Fai clic sul menu a discesa.

   ![](assets/program-member-custom-field-sync-4.png)

1. Scegliere il Marketo [!UICONTROL Program Member Custom Field] desiderato da mappare.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >Nell&#39;elenco a discesa verranno visualizzati solo [!UICONTROL Program Member Custom Fields] che corrispondono al tipo di dati del campo [!DNL Salesforce].

1. Per ulteriori mappature dei campi, deseleziona la casella di ricerca e ripeti i passaggi da 3 a 5.

1. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >Le modifiche ai dati dei membri del programma nei campi mappati verranno sincronizzate tra Marketo e [!DNL Salesforce] in futuro.

   >[!NOTE]
   >
   >Se si rinomina o si modifica il tipo di dati di un campo in [!DNL Salesforce], verrà rimossa qualsiasi mappatura di tale campo con [!UICONTROL Program Member Custom Field]. Ma puoi rimappare con il nuovo campo dopo la revisione.

## Annulla mappatura campi Salesforce dai campi personalizzati dei membri del programma {#unmap-salesforce-fields-from-program-member-custom-fields}

Se desideri liberare un campo per sostituirlo o semplicemente apportare una modifica generale, devi prima eseguire una rimozione dalla mappatura. Ecco come.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Fare clic su **[!DNL Salesforce]**, quindi fare clic su **[!UICONTROL Edit]** accanto a Sincronizzazione campi personalizzati membro del programma.

   ![](assets/program-member-custom-field-sync-8.png)

1. Utilizza la casella di ricerca per individuare i campi di cui vuoi annullare la mappatura. In questo esempio, utilizziamo Do Not Call.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >È possibile selezionare la casella di controllo **[!UICONTROL Mapped]** per visualizzare solo i campi mappati.

1. Annulla mappatura facendo clic su **X** accanto al campo.

   ![](assets/program-member-custom-field-sync-10.png)

1. La mappatura viene rimossa. Fai clic su **[!UICONTROL Save]**.

   ![](assets/program-member-custom-field-sync-11.png)

## Mappatura del tipo di dati {#data-type-mapping}

<table>
  <colgroup>
    <col/>
    <col/>
  </colgroup>
  <tbody>
    <tr>
      <th>Tipo di dati SFDC</th>
      <th>Tipo di dati campo personalizzato membro programma</th>
    </tr>
    <tr>
      <td>Testo</td>
      <td>Stringa</td>
    </tr>
    <tr>
      <td>Elenco a discesa</td>
      <td>Stringa</td>
    </tr>
    <tr>
      <td>Elenco a selezione multipla</td>
      <td>Stringa</td>
    </tr>
    <tr>
      <td>Telefono</td>
      <td>Stringa</td>
    </tr>
    <tr>
      <td>E-mail</td>
      <td>Stringa</td>
    </tr>
    <tr>
      <td>Numero(m)</td>
      <td>Intero</td>
    </tr>
    <tr>
      <td>Numero(m,n)</td>
      <td>Mobile</td>
    </tr>
    <tr>
      <td>Casella di controllo</td>
      <td>Booleano</td>
    </tr>
    <tr>
      <td>URL</td>
      <td>URL</td>
    </tr>
    <tr>
      <td>Data</td>
      <td>Data</td>
    </tr>
    <tr>
      <td>Data e ora</td>
      <td>Data e ora</td>
    </tr>
    <tr>
      <td>Ricerca (riferimento)</td>
      <td>Stringa</td>
    </tr>
    <tr>
      <td>Base64</td>
      <td>Stringa</td>
    </tr>
  </tbody>
</table>

>[!MORELIKETHIS]
>
>* [Modifica dati membro programma](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-member-data.md){target="_blank"}
>* [Visualizza dati sulla griglia dei membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/manage-and-view-members.md){target="_blank"}
>* [Sincronizzazione SFDC - Sincronizzazione Campagna](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
