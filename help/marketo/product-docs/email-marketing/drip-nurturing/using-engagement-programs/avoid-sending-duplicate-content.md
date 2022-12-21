---
unique-page-id: 10096409
description: Evita di inviare contenuti duplicati - Documenti Marketo - Documentazione del prodotto
title: Evita di inviare contenuti duplicati
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
source-git-commit: daaf3dc9b4da95db743409c6e2a6c426ed00e9c7
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 3%

---

# Evita di inviare contenuti duplicati {#avoid-sending-duplicate-content}

Lei ha mai ricevuto la stessa e-mail due volte? Fastidioso, vero?

Di seguito sono riportati sette possibili scenari e risultati di cui tenere conto per impedire a un utente di inviare lo stesso messaggio due volte con programmi di coinvolgimento.

## Scenari {#scenarios}

| L’e-mail viene inviata da | La persona è | La persona riceve l’e-mail |
|---|---|---|
| Una campagna in un programma separato, autonomo e predefinito | Non membro del programma predefinito | Sì |
| Una campagna in un programma separato, autonomo e predefinito | Membro del programma predefinito | No |
| Una campagna all’interno di un programma predefinito attivata da un cast all’interno di **stesso** programma CEE | Membro del programma predefinito | No |
| Una campagna all’interno di un programma predefinito attivata da un cast all’interno di **stesso** programma CEE | Non membro del programma predefinito | Sì |
| Una campagna all’interno di un programma predefinito attivata da un cast all’interno di un **diverso** programma CEE | Membro del programma predefinito | No |
| Una campagna all’interno di un programma predefinito attivata da un cast all’interno di un **diverso** programma CEE | Non membro del programma predefinito | Sì |
| A **diverso** Programma CEE che utilizza un flusso intelligente | Membro di entrambi i programmi CEE | No |
