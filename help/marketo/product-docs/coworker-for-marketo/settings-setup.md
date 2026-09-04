---
description: Scopri come abilitare Collaboratore per le autorizzazioni di Marketo Engage, configurare le regole organizzative e gestire impostazioni come integrazioni e notifiche.
title: Impostazioni e configurazione
source-git-commit: 01cad5c7d14083c0ef7127850f2488dbfd71f57b
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 1%

---

# Impostazioni e configurazione {#settings-setup}

Scopri come abilitare le autorizzazioni e utilizzare l’area Impostazioni per visualizzare i dettagli di connessione, definire regole organizzative e impostare integrazioni e notifiche.

>[!AVAILABILITY]
>
>Questa funzione è disponibile per tutti gli abbonamenti. Se non trovi il riquadro Collaboratore per Marketo Engage nella schermata My Marketo, contatta il tuo account manager. Devi accettare anche i [Termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}.

## Autorizzazioni e ruoli {#permission-and-role}

Sono disponibili l&#39;autorizzazione _Accesso a Coworker per Marketo Engage_ e il ruolo _Collaboratore per l&#39;utente Marketo Engage_, che offre agli amministratori un maggiore controllo sugli utenti che possono accedere alla funzionalità **Collaboratore per Marketo Engage**. L’autorizzazione viene assegnata a livello di ruolo. Il ruolo _Collaboratore per l&#39;utente Marketo Engage_ include l&#39;autorizzazione _Accesso a Collaboratore per Marketo Engage_ abilitata per impostazione predefinita.

>[!NOTE]
>
>L&#39;autorizzazione _Access Coworker for Marketo Engage_ non è abilitata per impostazione predefinita per tutti i ruoli. Per ulteriori informazioni, consulta la tabella seguente.

| Ruolo | Stato predefinito |
| --- | --- |
| Amministratore | Abilitata |
| Amministratore di prodotto Adobe | Abilitata |
| Utente marketing | Disabilitata |
| Utente standard | Non disponibile |
| Collaboratore per utente Marketo Engage | Abilitata |
| Ruoli personalizzati | Disabilitata |

### Accesso a Collaboratore per l’autorizzazione Marketo Engage {#access-coworker-marketo-permission}

Segui i passaggi seguenti per abilitare _Access Coworker for Marketo Engage_ per i ruoli idonei per i quali non è già abilitato.

1. Nel tuo My Marketo, fai clic su **Amministratore**, quindi su **Utenti e ruoli**.

   ![](assets/settings-setup-1.png)

1. Nella scheda _Ruoli_, seleziona il ruolo desiderato e fai clic su **Modifica ruolo**.

   ![](assets/settings-setup-2.png)

1. Scorri verso il basso e seleziona la casella di controllo _Accedi a Coworker per Marketo Engage_, quindi fai clic su **Salva**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >È possibile utilizzare la stessa procedura per rimuovere l&#39;autorizzazione **un** selezionando la casella di controllo _Accedi a Coworker per Marketo Engage_.

### Ruolo Collaboratore per Marketo Engage {#coworker-marketo-user-role}

Segui questi passaggi per assegnare un utente specifico al ruolo _Collaboratore per l&#39;utente Marketo Engage_.

>[!NOTE]
>
>Questo ruolo **only** contiene l&#39;autorizzazione _Access Coworker for Marketo Engage_.

1. Nel tuo My Marketo, fai clic su **Amministratore**, quindi su **Utenti e ruoli**.

   ![](assets/settings-setup-4.png)

1. Selezionare l&#39;utente desiderato e fare clic su **Modifica utente**.

   ![](assets/settings-setup-5.png)

1. In _Ruoli e aree di lavoro_, selezionare la casella di controllo _Collaboratore per l&#39;utente di Marketo Engage_. Se si dispone di più aree di lavoro, è possibile specificare a quali di esse è consentito l&#39;accesso nel menu a discesa del segno **+**. Al termine, fai clic su **Salva**.

   ![](assets/settings-setup-6.png)

### Ruolo personalizzato {#custom-role}

È inoltre possibile [creare un nuovo ruolo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} e personalizzarne le autorizzazioni, aggiungendo _Access Coworker per Marketo Engage_, insieme a qualsiasi altro elemento desiderato, e [assegnare tale ruolo](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a utenti specifici.

## Impostazioni {#settings}

1. Nel Marketo personale, fare clic sul riquadro **[!UICONTROL Coworker for Marketo Engage]**.

   ![](assets/settings-setup-7.png)

1. Fai clic sull’icona a forma di ingranaggio.

   ![](assets/settings-setup-8.png)

### Connessione {#connection}

Questa scheda non contiene campi modificabili. Mostra informazioni sull’account come il tuo Munchkin ID e l’organizzazione IMS.

![](assets/settings-setup-9.png)

### Regole organizzative {#organizational-rules}

Definisci le linee guida e i vincoli organizzativi che il Collaboratore per Marketo Engage deve rispettare durante la creazione o la modifica di risorse Marketo Engage.

![](assets/settings-setup-10.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Le regole utilizzano il formato Markdown con il frontmatter YAML. Le regole globali si applicano a tutte le aree di lavoro. Le regole di Workspace sovrascrivono le impostazioni globali.

### Integrazioni (presto disponibili) {#integrations}

Configurare le connessioni a servizi e API esterni.

_Questa scheda può essere visualizzata nell&#39;interfaccia utente, ma non è ancora disponibile. Controlla di nuovo la disponibilità di aggiornamenti_.

### Notifiche (disponibili a breve) {#notifications}

Gestisce le preferenze degli avvisi e i canali di notifica.

_Questa scheda può essere visualizzata nell&#39;interfaccia utente, ma non è ancora disponibile. Controllare la disponibilità di aggiornamenti in questo articolo_.
