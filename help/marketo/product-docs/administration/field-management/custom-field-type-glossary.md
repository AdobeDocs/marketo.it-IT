---
unique-page-id: 2951259
description: Glossario dei tipi di campo personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei tipi di campo personalizzato
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---

# Glossario dei tipi di campo personalizzato {#custom-field-type-glossary}

Quando crei un campo personalizzato in Marketo, hai un elenco di tipi tra cui scegliere.

>[!PREREQUISITES]
>
>[Crea un campo personalizzato in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>A seconda del tipo di campo, il filtro/trigger [operatori](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) sarà diverso.

>[!NOTE]
>
>La maggior parte dei campi non prevede un numero massimo di caratteri, ma solo un numero di byte. Per questo motivo, non è possibile fornire un limite di caratteri definitivo per ciascun campo. L&#39;eccezione è **String**, che non può superare i 255 caratteri.

## Booleano {#boolean}

**Nome esempio:** è un cliente - Assegna tag alle persone come clienti

**Valori di esempio:** True (selezionato) / False (deselezionato)

**Operatori**: nessuno

## Valuta {#currency}

**Nome esempio:** Budget - Memorizza un valore numerico per il budget di una società

**Valori di esempio:** 100

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Data {#date}

**Nome esempio:** Data di rinnovo - Memorizza le date di rinnovo dei clienti

**Valori di esempio:** 8/19/14

**Operatori**: è, non è, tra, passato, passato, passato, futuro, dopo, nell&#39;intervallo di tempo, dopo, prima, il o dopo, il o prima, è vuoto, non è vuoto

## Data e ora {#datetime}

**Nome esempio:** Data creazione - Memorizza la data e l&#39;ora di creazione di una persona

**Valori di esempio:** 8/19/14 2:00

**Operatori**: è, non è, tra, passato, passato, passato, futuro, dopo, nell&#39;intervallo di tempo, dopo, prima, il o dopo, il o prima, è vuoto, non è vuoto

## E-mail {#email}

**Nome esempio:** e-mail alternativa - Mantieni un indirizzo e-mail alternativo per le tue persone (non può effettivamente inviare e-mail a questo campo come il campo indirizzo e-mail predefinito, che è speciale)

**Valori di esempio:** <name@company.com>

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Mobile {#float}

**Nome esempio:** Media punti livello - Mantieni la media punti livello di una persona o qualsiasi altro valore numerico con decimali

**Valori di esempio:** 2.47

**Operatori**: tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Formula {#formula}

**Nome esempio:** Saluti. Utilizzare questo campo speciale in una [soluzione per ottenere la formula di apertura corretta](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) in base al sesso

**Valori di esempio:** controllare la soluzione collegata

## Intero {#integer}

**Nome esempio:** Numero di dipendenti - memorizzare un valore numerico che non richiede decimali

**Valori di esempio:** 600

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Percentuale {#percent}

**Nome esempio:** probabile acquisto - memorizzare un valore percentuale (forse calcolato sul lato CRM)

**Valori di esempio:** 85%

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Telefono {#phone}

**Nome esempio:** telefono alternativo - memorizzare un numero di telefono aggiuntivo per le persone

**Valore di esempio:** 650-555-5555

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Punteggio {#score}

**Nome esempio:** Punteggio comportamentale/Punteggio demografico - crea più campi di punteggio per tenere traccia di attributi diversi

**Valore di esempio:** 14

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Stringa {#string}

**Nome esempio:** secondo nome - memorizzare un attributo di testo aggiuntivo

**Valore di esempio:** Rose

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Area di testo {#text-area}

**Nome esempio:** Commenti - aggiungi un campo commenti ai moduli per consentire l&#39;immissione di testo su più righe

**Valore di esempio:** Questo articolo è fantastico!

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## URL {#url}

**Nome esempio:** Blog - crea un campo per memorizzare gli URL del blog della persona

**Valore di esempio:** &lt;www.myblog.com>

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto
