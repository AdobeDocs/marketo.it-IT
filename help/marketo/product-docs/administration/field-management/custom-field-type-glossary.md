---
unique-page-id: 2951259
description: Glossario sul tipo di campo personalizzato - Documenti Marketo - Documentazione sul prodotto
title: Glossario tipo di campo personalizzato
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---


# Glossario tipo di campo personalizzato {#custom-field-type-glossary}

Quando si crea un campo personalizzato in Marketo è disponibile un elenco di tipi tra cui scegliere.

>[!PREREQUISITES]
>
>* [Creare un campo personalizzato in Marketo](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>A seconda del tipo di campo, il filtro/trigger [operatori](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) sarà diverso.

>[!NOTE]
>
>La maggior parte dei campi non si limita al numero di caratteri, ma alla quantità di byte. Per questo motivo, non è possibile specificare un limite di caratteri definitivo per ciascun campo. L&#39;eccezione è **String**, che equivale a 255 caratteri.

## Booleano {#boolean}

**Nome esempio:** È cliente - Assegnare tag alle persone come clienti

**Valori di esempio:** True (selezionato) / False (non selezionato)

**Operatori**: None

## Valuta {#currency}

**Nome esempio:** Budget - Memorizza un valore numerico per il budget di una società

**Valori Di Esempio:** 100

**Operatori**: è, non è, tra, maggiore di, almeno minore di, è vuoto, non è vuoto

## Data {#date}

**Nome esempio:Data** rinnovo - Memorizza le date di rinnovo dei clienti

**Valori Di Esempio:** 8/19/14

**Operatori**: è, non è, tra, in passato, in passato, prima, in futuro, dopo, nell&#39;intervallo di tempo, dopo, prima, dopo, dopo, dopo, dopo, dopo, on o prima, è vuoto, non è vuoto

## Datetime {#datetime}

**Nome esempio:Data** creazione - Memorizza la data e l&#39;ora in cui viene creata una persona

**Valori Di Esempio:** 8/19/14 2:00

**Operatori**: è, non è, tra, in passato, in passato, prima, in futuro, dopo, nell&#39;intervallo di tempo, dopo, prima, dopo, dopo, dopo, dopo, dopo, on o prima, è vuoto, non è vuoto

## E-mail {#email}

**Nome esempio:E-mail** alternativa - Mantenere un indirizzo e-mail alternativo per le persone (non può inviare e-mail a questo campo come il campo dell&#39;indirizzo e-mail predefinito, che è speciale)

**Valori di esempio:** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Mobile {#float}

**Nome esempio:Media punti** di livello - Mantenere la media dei punti di valutazione di una persona o qualsiasi altro valore numerico con decimali

**Valori Di Esempio:** 2.47

**Operatori**: è vuoto, il valore è maggiore o minore di, almeno, è vuoto, non è vuoto

## Formula {#formula}

**Nome esempio:** Salutazioni - usa questo campo speciale in una  [soluzione per ottenere la giusta formula di ](create-and-use-a-concatenated-string-formula-field.md) formula basata sul genere

**Valori di esempio:** verificare la soluzione collegata

## Numero intero {#integer}

**Nome esempio:** Numero di dipendenti - memorizzare un valore numerico che non richiede decimali

**Valori Di Esempio:** 600

**Operatori**: è, non è, tra, maggiore di, almeno minore di, è vuoto, non è vuoto

## Percentuale {#percent}

**Nome esempio:** Probabile da acquistare - memorizzare un valore percentuale (forse calcolato sul lato CRM)

**Valori Di Esempio:** 85%

**Operatori**: è, non è, tra, maggiore di, almeno minore di, è vuoto, non è vuoto

## Telefono {#phone}

**Nome esempio:** Telefono alternativo - memorizzare un numero di telefono aggiuntivo per le persone

**Valore Di Esempio:** 650-555-5555

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Punteggio {#score}

**Nome esempio:** Punteggio comportamentale/Punteggio demografico: create più campi di valutazione per tenere traccia dei diversi attributi.

**Valore Di Esempio:** 14

**Operatori**: è, non è, tra, maggiore di, almeno minore di, è vuoto, non è vuoto

## Stringa {#string}

**Nome esempio:Nome** centrale - memorizzare un attributo di testo aggiuntivo

**Valore Di Esempio:** Rose

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Area di testo {#text-area}

**Nome esempio:** Commenti - aggiungere un campo commenti ai moduli per consentire l&#39;immissione di testo su più righe

**Esempio di valore:** Questo articolo è fantastico!

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## URL {#url}

**Nome esempio:** Blog - creare un campo per memorizzare gli URL dei blog delle persone

**Valore Di Esempio:** www.myblog.com

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto
