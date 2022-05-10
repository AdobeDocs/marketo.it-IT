---
description: Domande frequenti sulla sincronizzazione degli account personali - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti sulla sincronizzazione dell’account personale
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Domande frequenti sulla sincronizzazione dell’account personale {#person-account-sync-faq}

Il Marketo Engage sincronizza l&#39;intero database con Veeva per il tipo di record Conto Persona. Dopo la sincronizzazione aspetta 5 minuti, poi sincronizza di nuovo, tutto il giorno, ogni giorno.

Gli account personali possono essere configurati in Veeva per soddisfare le esigenze della tua organizzazione.

>[!NOTE]
>
>Sincronizziamo solo gli account di livello &quot;Professional&quot; come account personali.

**Che cos’è un account persona?**

Un account persona è molto simile all&#39;oggetto account in Veeva CRM. Tuttavia, un account persona ha accesso sia ai campi dell’account che ai campi di contatto.

**Cosa succede quando un account persona viene sincronizzato con Marketo?**

Un account persona viene sincronizzato in Marketo come azienda e come persona.

>[!NOTE]
>
>I campi personalizzati per un account persona vengono copiati sia nella società che nella persona in Marketo.

**Come differenziare account aziendali e account personali?**

Utilizza il filtro account &quot;Is Person&quot; nel tuo Smart List per separare gli account delle persone dagli account aziendali standard.

**Quale campo e-mail devo utilizzare per gli account personali?**

Esistono due campi e-mail per un account persona. Utilizzare il campo Indirizzo e-mail nei moduli (non l’indirizzo e-mail personale) per garantire il corretto funzionamento della deduplicazione di Marketo e di altre elaborazioni e-mail.

## Direzione sincronizzazione {#sync-direction}

La sincronizzazione dei campi relativi al contatto dell’account persona è bidirezionale. Se apporti modifiche a un contatto in Veeva CRM o Marketo, gli aggiornamenti verranno rispecchiati in entrambi i sistemi. I campi sull&#39;account si sincronizzano in una sola direzione, da Veeva CRM a Marketo.

**Cosa succede se in entrambi i sistemi vengono apportate modifiche ai campi Contatto sull&#39;account personale contemporaneamente?**

Saremmo gentili e lasceremmo vincere Veeva CRM. Tuttavia, è raro che si verifichi questo tipo di conflitto di dati.

**Il tipo di record Lead o Contact è sincronizzato con Veeva CRM?**

Veeva CRM si occupa solo degli oggetti Account personali e dispone anche di Account commerciali. I tradizionali tipi di CRM di lead, contatti e opportunità non sono realmente in uso nei sistemi tradizionali di gestione delle relazioni con i clienti Veeva. Questi possono essere creati in Veeva CRM, ma non sono ufficialmente supportati utilizzando questo connettore.

**Posso convertire una persona in un contatto in Marketo?**

No, poiché Lead e Contatti non sono tipi supportati per la sincronizzazione con Veeva CRM. Di conseguenza, la conversione non è supportata.

**È possibile forzare manualmente la sincronizzazione di un contatto?**

No, poiché Contact non è un tipo di record indipendente, la sincronizzazione di una persona a Veeva non è supportata.

**Ogni singolo campo standard si sincronizza con Marketo?**

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui l’utente di Marketo Sync ha accesso.

**Marketo rispetterà le regole di convalida di Veeva?**

Sì, in caso di conflitto, il risultato verrà registrato nel registro attività del lead.

>[!MORELIKETHIS]
>
>* [Mappatura predefinita del campo Veeva](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;}
>* [Sincronizzazione dei messaggi chiave di chiamata e chiamata](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}

