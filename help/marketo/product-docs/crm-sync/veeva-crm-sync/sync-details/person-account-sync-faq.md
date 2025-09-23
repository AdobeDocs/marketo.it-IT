---
description: Domande frequenti sulla sincronizzazione dell’account della persona - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti sulla sincronizzazione dell’account persona
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# Domande frequenti sulla sincronizzazione dell’account persona {#person-account-sync-faq}

Marketo Engage sincronizza l&#39;intero database con [!DNL Veeva] per il tipo di record Account persona. Dopo la sincronizzazione attende 5 minuti, quindi sincronizza di nuovo, tutto il giorno, ogni giorno.

Gli account personali possono essere impostati in [!DNL Veeva] per soddisfare le esigenze della tua organizzazione.

>[!NOTE]
>
>Sincronizziamo solo gli account di livello &quot;Professional&quot; come account persona.

**Che cos&#39;è un account persona?**

Un account persona è molto simile all&#39;oggetto account in [!DNL Veeva] CRM. Tuttavia, un account persona ha accesso sia ai campi account che ai campi contatto.

**Cosa succede quando un account utente viene sincronizzato con Marketo?**

Un account persona viene sincronizzato in Marketo come azienda e come persona.

>[!NOTE]
>
>I campi personalizzati per un account persona vengono copiati sia nella società che nella persona in Marketo.

**Come posso distinguere gli account aziendali dagli account personali?**

Utilizza il filtro Account &quot;Is Person&quot; (È persona) nel tuo elenco avanzato per separare gli account persona dagli account aziendali standard.

**Quale campo di posta elettronica utilizzare per gli account personali?**

Per un account persona sono disponibili due campi e-mail. Utilizza il campo Indirizzo e-mail nei moduli (non l’Indirizzo e-mail della persona) per garantire che la deduplicazione di Marketo e altre forme di elaborazione e-mail funzionino correttamente.

## Direzione di sincronizzazione {#sync-direction}

La sincronizzazione dei campi relativi al contatto dell’account persona è bidirezionale. Se si apportano modifiche a un contatto in [!DNL Veeva] CRM o Marketo, gli aggiornamenti verranno applicati in entrambi i sistemi. I campi dell&#39;account vengono sincronizzati in una sola direzione, da [!DNL Veeva] CRM a Marketo.

**Cosa succede se in entrambi i sistemi vengono apportate modifiche ai campi Contatto sull&#39;account della persona contemporaneamente?**

Saremmo gentili e lasceremmo vincere [!DNL Veeva] CRM. Tuttavia, è raro che si verifichi questo tipo di conflitto di dati.

**Il tipo di record Lead o Contatto è sincronizzato con [!DNL Veeva] CRM?**

[!DNL Veeva] CRM si occupa solo degli oggetti dell&#39;account della persona e dispone anche di account aziendali. I tipi di CRM tradizionali di lead, contatti e opportunità non sono realmente utilizzati nei sistemi CRM tradizionali di [!DNL Veeva]. Possono essere create in [!DNL Veeva] CRM, ma non sono ufficialmente supportate tramite questo connettore.

**È possibile convertire una persona in un contatto in Marketo?**

No, poiché lead e contatti non sono tipi supportati per la sincronizzazione con il sistema CRM [!DNL Veeva]. Di conseguenza, la conversione non è supportata.

**È possibile forzare manualmente la sincronizzazione di un contatto?**

No, poiché Contact non è un tipo di record indipendente, la sincronizzazione di una persona con [!DNL Veeva] non è supportata.

**Ogni singolo campo standard è sincronizzato con Marketo?**

No, non tutti i campi standard sono utili. Tutti i campi personalizzati possono far parte della sincronizzazione.

>[!NOTE]
>
>Marketo sincronizzerà solo i campi a cui l’utente di Marketo Sync ha accesso.

**Marketo rispetterà le [!DNL Veeva] regole di convalida?**

Sì, se si verifica un conflitto, il risultato verrà registrato nel registro attività del lead.

>[!MORELIKETHIS]
>
>* [Predefinito [!DNL Veeva] Mappatura campi](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Sincronizzazione dei messaggi chiave di chiamata e chiamata](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
