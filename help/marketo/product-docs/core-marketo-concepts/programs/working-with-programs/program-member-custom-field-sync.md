---
description: Sincronizzazione campi personalizzati membro del programma - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione campo personalizzato membro programma
exl-id: 7facfc79-a411-4ad9-b847-2002763af5bb
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 5%

---

# Sincronizzazione campo personalizzato membro programma {#program-member-custom-field-sync}

>[!PREREQUISITES]
>
>* Creazione di [Campi personalizzati del membro del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md){target="_blank"}
>* [Sincronizzare una campagna Salesforce con un programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/sync-an-sfdc-campaign-with-a-program.md){target="_blank"}

>[!NOTE]
>
>L&#39;oggetto Membro del programma può contenere fino a 20 campi personalizzati. Questi campi sono disponibili per qualsiasi programma.

## Mappa i campi Salesforce ai campi personalizzati dei membri del programma {#map-salesforce-fields-to-program-member-custom-fields}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/program-member-custom-field-sync-1.png)

1. Clic **Salesforce**, quindi fai clic su **Modifica** accanto a Sincronizzazione campi personalizzati membro programma.

   ![](assets/program-member-custom-field-sync-2.png)

1. Utilizza la casella di ricerca per individuare i campi Salesforce che desideri mappare. In questo esempio, utilizziamo Do Not Call.

   ![](assets/program-member-custom-field-sync-3.png)

1. Fai clic sul menu a discesa.

   ![](assets/program-member-custom-field-sync-4.png)

1. Scegliere il campo personalizzato del membro del programma Marketo desiderato da mappare.

   ![](assets/program-member-custom-field-sync-5.png)

   >[!NOTE]
   >
   >Nell&#39;elenco a discesa vengono visualizzati solo i campi personalizzati dei membri del programma che corrispondono al tipo di dati del campo Salesforce.

1. Per ulteriori mappature dei campi, deseleziona la casella di ricerca e ripeti i passaggi da 3 a 5.

1. Clic **Salva** al termine.

   ![](assets/program-member-custom-field-sync-6.png)

   >[!IMPORTANT]
   >
   >In futuro, le modifiche ai dati dei membri del programma nei campi mappati verranno sincronizzate tra Marketo e Salesforce.

   >[!NOTE]
   >
   >Se si rinomina o si modifica il tipo di dati di un campo in Salesforce, verrà rimossa qualsiasi mappatura di tale campo con il campo personalizzato Membro del programma. Ma puoi rimappare con il nuovo campo dopo la revisione.

## Annulla mappatura campi Salesforce da campi personalizzati membri del programma {#unmap-salesforce-fields-from-program-member-custom-fields}

Se desideri liberare un campo per sostituirlo o semplicemente apportare una modifica generale, devi prima eseguire una rimozione dalla mappatura. Ecco come.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/program-member-custom-field-sync-7.png)

1. Clic **Salesforce**, quindi fai clic su **Modifica** accanto a Sincronizzazione campi personalizzati membro programma.

   ![](assets/program-member-custom-field-sync-8.png)

1. Utilizza la casella di ricerca per individuare i campi di cui vuoi annullare la mappatura. In questo esempio, utilizziamo Do Not Call.

   ![](assets/program-member-custom-field-sync-9.png)

   >[!TIP]
   >
   >È possibile selezionare **Mappato** per visualizzare solo i campi mappati.

1. Per annullare la mappatura, fai clic su **X** accanto al campo.

   ![](assets/program-member-custom-field-sync-10.png)

1. La mappatura viene rimossa. Clic **Salva**.

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
>* [Sincronizzazione SFDC - Sincronizzazione campagna](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}
