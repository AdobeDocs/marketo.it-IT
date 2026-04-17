---
description: Scopri come abilitare le autorizzazioni di Marketo AI, configurare le regole organizzative e gestire impostazioni come integrazioni e notifiche.
title: Impostazioni e configurazione
hide: true
hidefromtoc: true
source-git-commit: 2e7e068ac53c9f26075d700822fc1f89274dddbe
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Impostazioni e configurazione {#settings-setup}

Scopri come abilitare le autorizzazioni e utilizzare l’area Impostazioni per visualizzare i dettagli di connessione, definire regole organizzative e impostare integrazioni e notifiche.

## Autorizzazioni e ruoli {#permission-and-role}

Esiste una build di _accesso con autorizzazione AI_ e un ruolo _Build con utente AI_, che offre agli amministratori un maggiore controllo sugli utenti che possono accedere alla funzionalità **Build con AI**. L’autorizzazione viene assegnata a livello di ruolo. Il ruolo _Build con utente AI_ viene fornito con l&#39;autorizzazione _Build di accesso con IA_ abilitata per impostazione predefinita.

>[!IMPORTANT]
>
>Per impostazione predefinita, la compilazione di accesso _con autorizzazione AI_ non è abilitata per tutti i ruoli. Per ulteriori informazioni, consulta la tabella seguente.

| Ruolo | Stato predefinito |
| --- | --- |
| Amministratore | Abilitata |
| Amministratore di prodotto Adobe | Abilitata |
| Utente marketing | Disabilitata |
| Utente standard | Non disponibile |
| Genera con utente AI | Abilitata |
| Ruoli personalizzati | Disabilitata |

### Accedere alla build con l’autorizzazione AI {#access-build-with-ai-permission}

Segui i passaggi seguenti per abilitare _Access Build con AI_ per i ruoli idonei per i quali non è già abilitata.

1. Nel tuo My Marketo, fai clic su **Amministratore**, quindi su **Utenti e ruoli**.

   ![](assets/settings-setup-1.png)

1. Nella scheda _Ruoli_, seleziona il ruolo desiderato e fai clic su **Modifica ruolo**.

   ![](assets/settings-setup-2.png)

1. Scorri verso il basso e seleziona la casella di controllo _Access Build with AI_ e fai clic su **Salva**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Puoi utilizzare gli stessi passaggi per rimuovere l&#39;autorizzazione selezionando la casella di controllo **un** Access Build with AI _._

### Creare con il ruolo utente di IA {#build-with-ai-user-role}

Segui questi passaggi per assegnare un utente specifico al ruolo _Genera con utente AI_.

>[!NOTE]
>
>Questo ruolo **only** contiene _Access Build con autorizzazioni AI_.

1. Nel tuo My Marketo, fai clic su **Amministratore**, quindi su **Utenti e ruoli**.

   ![](assets/settings-setup-1.png)

1. Selezionare l&#39;utente desiderato e fare clic su **Modifica utente**.

   ![](assets/settings-setup-5b.png)

1. In _Ruoli e aree di lavoro_, selezionare la casella di controllo _Genera con utente AI_. Se si dispone di più aree di lavoro, è possibile specificare a quali di esse è consentito l&#39;accesso nel menu a discesa del segno **+**. Al termine, fai clic su **Salva**.

   ![](assets/settings-setup-6b.png)

### Ruolo personalizzato {#custom-role}

È inoltre possibile [creare un nuovo ruolo](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} e personalizzarne le autorizzazioni, aggiungendo _Access Build con AI_, insieme a qualsiasi altro elemento desiderato, e [assegnare tale ruolo](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a utenti specifici.

## Impostazioni {#settings}

1. In Il mio Marketo, fai clic sul riquadro **Genera con IA**.

   ![](assets/settings-setup-4.png)

1. Fai clic sull’icona a forma di ingranaggio.

   ![](assets/settings-setup-5.png)

### Connessione {#connection}

Questa scheda non contiene campi modificabili. Mostra informazioni sull’account, come il tuo Munchkin ID e l’organizzazione IMS.

![](assets/settings-setup-6.png)

### Regole organizzative {#organizational-rules}

Definisci le linee guida e i vincoli organizzativi che Marketo AI segue durante la creazione o la modifica di risorse Marketo Engage.

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Le regole utilizzano il formato Markdown con il frontmatter YAML. Le regole globali si applicano a tutte le aree di lavoro. Le regole di Workspace sovrascrivono le impostazioni globali.

### Integrazioni (presto disponibili) {#integrations}

Configurare le connessioni a servizi e API esterni.

_Questa scheda può essere visualizzata nell&#39;interfaccia utente, ma non è ancora disponibile. Controlla di nuovo la disponibilità di aggiornamenti_.

### Notifiche (disponibili a breve) {#notifications}

Gestisce le preferenze degli avvisi e i canali di notifica.

_Questa scheda può essere visualizzata nell&#39;interfaccia utente, ma non è ancora disponibile. Controlla di nuovo la disponibilità di aggiornamenti_.
