---
description: Scopri come abilitare le autorizzazioni di Marketo AI, configurare le regole organizzative e gestire impostazioni come integrazioni e notifiche.
title: Impostazioni e configurazione
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: d5f5c11a56f21e7dba3e1e79eb6785937f165b14
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Impostazioni e configurazione {#settings-setup}

Scopri come abilitare le autorizzazioni e utilizzare l’area Impostazioni per visualizzare i dettagli di connessione, definire regole organizzative e impostare integrazioni e notifiche.

## Autorizzazioni {#permissions}

>[!IMPORTANT]
>
>Nella fase Alpha di Marketo AI, l&#39;accesso _è abilitato per impostazione predefinita_ per i seguenti ruoli: Amministratore, Amministratore di prodotto Adobe, Utente di marketing, Utente standard. Pertanto, invece di attivarla per i ruoli a cui si desidera accedere, è necessario disattivarla per i ruoli non disponibili.

### Accesso per tutti {#access-for-all}

Se desideri abilitare Marketo AI per tutti i ruoli elencati sopra, non è necessario eseguire alcuna operazione.

### Accesso per alcuni {#access-for-some}

Se desideri rimuovere l’accesso per qualsiasi ruolo, segui la procedura riportata di seguito.

1. Nel tuo My Marketo, fai clic su **Amministratore**, quindi su **Utenti e ruoli**.

   ![](assets/settings-setup-1.png)

1. Nella scheda _Ruoli_, seleziona il ruolo o i ruoli desiderati e fai clic su **Modifica ruolo**.

   ![](assets/settings-setup-2.png)

1. Scorri verso il basso e _deseleziona_ la casella di controllo **Access Build with AI** e fai clic su **Salva**.

   ![](assets/settings-setup-3.png)

### Ruolo personalizzato {#custom-role}

È inoltre possibile [creare un nuovo ruolo](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} e personalizzarne le autorizzazioni, aggiungendo _Access Build con AI_, insieme a qualsiasi altro elemento desiderato, e [assegnare tale ruolo](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} a utenti specifici.

<!-- ## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

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
