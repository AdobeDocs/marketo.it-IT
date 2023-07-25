---
unique-page-id: 12982909
description: Programmi di pianificazione del coinvolgimento con fuso orario del destinatario - Documentazione di Marketo - Documentazione del prodotto
title: Programmi di pianificazione del coinvolgimento con fuso orario del destinatario
exl-id: 818615be-3c7e-4051-adc7-2341783484b9
feature: Engagement Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# Programmi di pianificazione del coinvolgimento con fuso orario del destinatario {#schedule-engagement-programs-with-recipient-time-zone}

Quando pianifichi uno streaming del programma di coinvolgimento e il fuso orario del destinatario è attivo, il cast del programma inizierà a essere eseguito a mezzanotte nel primo fuso orario (UTC +14:00). È necessario pianificare il primo cast **almeno 25 ore** in futuro perché ci potrebbero essere persone che si qualificano per il cast in ogni fuso orario del mondo. L’avvio dell’elaborazione in questo momento in base al primo fuso orario garantisce la consegna dell’e-mail alla data e all’ora pianificate per ogni destinatario.

1. Nel programma di coinvolgimento, accedi al **Flussi** e fai clic sulla pianificazione della cadenza di un flusso per modificarla.

   ![](assets/image2017-12-5-13-3a36-3a21.png)

1. [Impostare le impostazioni della cadenza](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md) come si farebbe normalmente, quindi controllare il **Fuso orario destinatario** casella. Ricorda che il tuo primo cast deve durare almeno 25 ore in futuro. Clic **Salva**.

   ![](assets/image2017-12-5-13-3a50-3a32.png)

1. Tieni presente che con il fuso orario del destinatario attivo, la pianificazione della cadenza non mostrerà un fuso orario specifico, in quanto potrebbero esserci più fusi orari. Verrà visualizzata solo l’ora.

   ![](assets/image2017-12-5-13-3a56-3a21.png)

>[!MORELIKETHIS]
>
>* [Informazioni sul fuso orario del destinatario](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md)
>* [Imposta cadenza flusso](/help/marketo/product-docs/email-marketing/drip-nurturing/engagement-program-streams/set-stream-cadence.md)
