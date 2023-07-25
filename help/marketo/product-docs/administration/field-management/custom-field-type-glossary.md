---
unique-page-id: 2951259
description: Glossario dei tipi di campo personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei tipi di campo personalizzati
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Glossario dei tipi di campo personalizzati {#custom-field-type-glossary}

Quando crei un campo personalizzato in Marketo, hai un elenco di tipi tra cui scegliere.

>[!PREREQUISITES]
>
>[Creare un campo personalizzato in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>A seconda del tipo di campo, filtro/trigger [operatori](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) sarà diverso.

>[!NOTE]
>
>La maggior parte dei campi non prevede un numero massimo di caratteri, ma solo un numero di byte. Per questo motivo, non è possibile fornire un limite di caratteri definitivo per ciascun campo. L’eccezione è **Stringa**, che non può superare i 255 caratteri.

## Booleano {#boolean}

**Nome esempio:** È cliente - Assegna tag alle persone come clienti

**Valori di esempio:** True (selezionato) / False (deselezionato)

**Operatori**: nessuna

## Valuta {#currency}

**Nome esempio:** Budget - Memorizza un valore numerico per il budget di una società

**Valori di esempio:** 100

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Data {#date}

**Nome esempio:** Data di rinnovo: memorizza le date di rinnovo dei clienti

**Valori di esempio:** 8/19/14

**Operatori**: è, non è, tra, nel passato, nel passato, prima, nel futuro, dopo, nell’intervallo di tempo, dopo, prima, il o dopo, il o prima di, è vuoto, non è vuoto

## Data e ora {#datetime}

**Nome esempio:** Data creazione: memorizza la data e l’ora di creazione di una persona.

**Valori di esempio:** 8/19/14 2:00

**Operatori**: è, non è, tra, nel passato, nel passato, prima, nel futuro, dopo, nell’intervallo di tempo, dopo, prima, il o dopo, il o prima di, è vuoto, non è vuoto

## E-mail {#email}

**Nome esempio:** E-mail alternativa: mantieni un indirizzo e-mail alternativo per le tue persone (non puoi effettivamente inviare e-mail a questo campo come nel campo dell’indirizzo e-mail predefinito, che è speciale)

**Valori di esempio:** name@company.com

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Mobile {#float}

**Nome esempio:** Media punti livello: consente di mantenere la media dei punti livello di una persona o qualsiasi altro valore numerico con decimali

**Valori di esempio:** 2,47

**Operatori**: tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Formula {#formula}

**Nome esempio:** Saluti: utilizza questo campo speciale in una [soluzione per ottenere il giusto saluto](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) in base al sesso

**Valori di esempio:** controllare la soluzione collegata

## Intero {#integer}

**Nome esempio:** Numero di dipendenti: memorizza un valore numerico che non richiede decimali

**Valori di esempio:** 600

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Percentuale {#percent}

**Nome esempio:** Probabilità di acquistare - memorizzare un valore percentuale (forse calcolato sul lato CRM)

**Valori di esempio:** 85%

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Telefono {#phone}

**Nome esempio:** Telefono alternativo: memorizza un numero di telefono aggiuntivo per le tue persone

**Esempio di valore:** 650 555 555

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Punteggio {#score}

**Nome esempio:** Punteggio comportamentale/Punteggio demografico: crea più campi di punteggio per tenere traccia dei diversi attributi

**Esempio di valore:** 14

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Stringa {#string}

**Nome esempio:** Secondo nome: memorizza un attributo di testo aggiuntivo

**Esempio di valore:** Rosa

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Area di testo {#text-area}

**Nome esempio:** Commenti: aggiungi un campo commenti ai moduli per consentire l’immissione di testo su più righe

**Esempio di valore:** Questo articolo è fantastico!

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## URL {#url}

**Nome esempio:** Blog: crea un campo per memorizzare gli URL del blog di una persona

**Esempio di valore:** www.myblog.com

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto
