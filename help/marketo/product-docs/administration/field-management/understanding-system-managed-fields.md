---
unique-page-id: 5472615
description: Informazioni sui campi gestiti dal sistema - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sui campi gestiti dal sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 11%

---

# Informazioni sui campi gestiti dal sistema {#understanding-system-managed-fields}

È possibile che la [pagina dei dettagli della persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} contenga una serie di campi non modificabili creati da Marketo. Questi dati provengono da varie fonti, e ci sono innumerevoli valori che potrebbero essere visualizzati.

## Tipi di campi {#field-types}

<table><thead>
  <tr>
    <th>Nome campo</th>
    <th>Definizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Tipo di sorgente originale</td>
    <td>La posizione in cui una persona o un visitatore del sito Web è stato individuato per la prima volta (esempio: importazione elenco, visita pagina Web)</td>
  </tr>
  <tr>
    <td>Informazioni sorgente originali</td>
    <td>Informazioni specifiche sulla posizione (esempio: nome dell’elenco, URL della pagina web)</td>
  </tr>
  <tr>
    <td>Motore di ricerca originale</td>
    <td>Se del caso, il motore di ricerca che ha rinviato la persona alla fonte di ingresso originale</td>
  </tr>
  <tr>
    <td>Frase di ricerca originale</td>
    <td>Se applicabile, il termine di ricerca utilizzato che ha rinviato la persona alla sorgente di ingresso originale</td>
  </tr>
  <tr>
    <td>Destinatario che inoltra originale</td>
    <td>URL che ha ospitato l'origine della voce originale</td>
  </tr>
  <tr>
    <td>Tipo Source registrazione</td>
    <td>La posizione in cui un’attività è diventata per la prima volta una persona (esempio: importazione di elenchi, visita di pagine web)</td>
  </tr>
  <tr>
    <td>Registrazione informazioni Source</td>
    <td>Informazioni specifiche sulla posizione (esempio: nome dell’elenco, URL della pagina web)</td>
  </tr>
  <tr>
    <td>IP anonimo</td>
    <td>Indica l'indirizzo IP di una persona</td>
  </tr>
  <tr>
    <td>Azienda dedotta</td>
    <td>Migliore stima di Marketo (basata su IP) dell’azienda della persona</td>
  </tr>
  <tr>
    <td>Città dedotta</td>
    <td>Migliore stima di Marketo (basata su IP) della città della persona</td>
  </tr>
  <tr>
    <td>Area geografica dello stato dedotta</td>
    <td>Migliore stima di Marketo (basata su IP) dello stato o dell’area geografica della persona</td>
  </tr>
  <tr>
    <td>Codice postale dedotto</td>
    <td>Migliore stima di Marketo (basata su IP) del codice postale della persona</td>
  </tr>
  <tr>
    <td>Paese dedotto</td>
    <td>Migliore stima di Marketo (basata su IP) del paese della persona</td>
  </tr>
  <tr>
    <td>Area metropolitana dedotta</td>
    <td>L'ipotesi migliore di Marketo (basata su IP) dell'area metropolitana della persona</td>
  </tr>
  <tr>
    <td>Prefisso telefonico dedotto</td>
    <td>Migliore stima di Marketo (basata su IP) dell’indicativo di località della persona</td>
  </tr>
</tbody></table>

## Valori possibili per il tipo di Source originale e di registrazione {#possible-values-for-original-and-registration-source-type}

Di seguito sono riportati alcuni valori possibili e il loro significato.

<table><thead>
  <tr>
    <th>Tipo di sorgente originale</th>
    <th>Definizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Salesforce.com</td>
    <td>La persona è stata rilevata dalla sincronizzazione Salesforce</td>
  </tr>
  <tr>
    <td>Visite alle pagine web</td>
    <td>La persona è stata scoperta da una pagina web</td>
  </tr>
  <tr>
    <td>Compilazione modulo web</td>
    <td>La persona è stata scoperta dopo la compilazione di un modulo</td>
  </tr>
  <tr>
    <td>Importazione elenco</td>
    <td>Persona scoperta da un’importazione elenco</td>
  </tr>
  <tr>
    <td>Nuova persona</td>
    <td>La persona è stata inserita manualmente nel database</td>
  </tr>
  <tr>
    <td>Clic collegamento web</td>
    <td>La persona è stata scoperta dopo aver fatto clic su un collegamento</td>
  </tr>
  <tr>
    <td>E-mail vendita</td>
    <td>Alla persona è stata inviata un'e-mail tramite il componente aggiuntivo e-mail di Sales Insight</td>
  </tr>
  <tr>
    <td>Persona</td>
    <td>La persona è stata sincronizzata da Salesforce come persona</td>
  </tr>
  <tr>
    <td>Contatto</td>
    <td>La persona è stata sincronizzata dal webhook come contatto</td>
  </tr>
  <tr>
    <td>API MUNCHKIN</td>
    <td>La persona è stata scoperta dall’API Munchkin di Marketo Engage</td>
  </tr>
  <tr>
    <td>App social</td>
    <td>La persona è stata scoperta da un widget sociale</td>
  </tr>
  <tr>
    <td>API servizio Web</td>
    <td>La persona è stata rilevata da un’API del servizio web</td>
  </tr>
  <tr>
    <td>Partner evento</td>
    <td>La persona è stata scoperta tramite un servizio di webinar sincronizzato</td>
  </tr>
  <tr>
    <td>Associa lead</td>
    <td>Persona unita tramite chiamata API del lead associato</td>
  </tr>
</tbody></table>

<table><thead>
  <tr>
    <th>Tipo Source registrazione</th>
    <th>Definizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Importazione elenco</td>
    <td>Diventare una persona tramite un’importazione di elenchi</td>
  </tr>
  <tr>
    <td>Salesforce.com</td>
    <td>Diventare una persona tramite Salesforce Sync</td>
  </tr>
  <tr>
    <td>Compilazione modulo web</td>
    <td>Diventare una persona dopo la compilazione di un modulo</td>
  </tr>
  <tr>
    <td>E-mail vendita</td>
    <td>Alla persona è stata inviata un'e-mail tramite il componente aggiuntivo e-mail di Sales Insight</td>
  </tr>
  <tr>
    <td>API servizio Web</td>
    <td>La persona è stata creata tramite API SOAP/REST</td>
  </tr>
  <tr>
    <td>Nuova persona</td>
    <td>La persona è stata inserita manualmente nel database</td>
  </tr>
  <tr>
    <td>API MUNCHKIN</td>
    <td>Diventare una persona tramite API Munchkin di Marketo</td>
  </tr>
  <tr>
    <td>App social</td>
    <td>Diventare una persona tramite un widget sociale</td>
  </tr>
  <tr>
    <td>Partner evento</td>
    <td>Diventare una persona tramite un servizio di webinar collegato</td>
  </tr>
</tbody>
</table>
