---
unique-page-id: 2951259
description: Glossario sul tipo di campo personalizzato - Documenti Marketo - Documentazione del prodotto
title: Glossario del tipo di campo personalizzato
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 1%

---

# Glossario del tipo di campo personalizzato {#custom-field-type-glossary}

Quando crei un campo personalizzato in Marketo puoi scegliere un elenco di tipi.

>[!PREREQUISITES]
>
>[Creare un campo personalizzato in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>A seconda del tipo di campo, filtrare/attivare [operatori](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) sarà diverso.

>[!NOTE]
>
>La maggior parte dei campi non si limita al numero di caratteri, ma alla quantità di byte. Per questo motivo non è possibile fornire un limite di caratteri definitivo per ciascun campo. L&#39;eccezione è **Stringa**, che corrisponde a 255 caratteri.

## Booleano {#boolean}

**Nome esempio:** È cliente : contrassegna le persone come clienti

**Valori di esempio:** True (selezionato) / False (non selezionato)

**Operatori**: Nessuno

## Valuta {#currency}

**Nome esempio:** Budget - Memorizza un valore numerico per il budget di un&#39;azienda

**Valori di esempio:** 100

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Data {#date}

**Nome esempio:** Data di rinnovo - Memorizza le date di rinnovo dei clienti

**Valori di esempio:** 19/08/14

**Operatori**: è, non è, tra, in passato, in passato, prima, in futuro, in futuro, dopo, nell&#39;intervallo di tempo, dopo, prima, dopo, dopo, dopo, in o prima, è vuoto, non è vuoto

## Datetime {#datetime}

**Nome esempio:** Data creazione: consente di memorizzare la data e l’ora in cui viene creata una persona

**Valori di esempio:** 19/08/14 2:00

**Operatori**: è, non è, tra, in passato, in passato, prima, in futuro, in futuro, dopo, nell&#39;intervallo di tempo, dopo, prima, dopo, dopo, dopo, in o prima, è vuoto, non è vuoto

## E-mail {#email}

**Nome esempio:** E-mail alternativa: mantieni un indirizzo e-mail alternativo per le persone (non può effettivamente inviare e-mail a questo campo, come il campo dell’indirizzo e-mail predefinito, che è speciale)

**Valori di esempio:** name@company.com

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Mobile {#float}

**Nome esempio:** Media punti di livello - Mantenere la media dei punti di livello di una persona o qualsiasi altro valore numerico con decimali

**Valori di esempio:** 2,47

**Operatori**: tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Formula {#formula}

**Nome esempio:** Saluti - utilizza questo campo speciale in un [soluzione per ottenere il giusto saluto](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) in base al genere

**Valori di esempio:** controlla la soluzione collegata

## Intero {#integer}

**Nome esempio:** Numero di dipendenti - memorizzare un valore numerico che non richiede decimali

**Valori di esempio:** 600

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Percentuale {#percent}

**Nome esempio:** Probabile da acquistare - memorizzare un valore percentuale (forse calcolato sul lato CRM)

**Valori di esempio:** 85%

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Telefono {#phone}

**Nome esempio:** Telefono alternativo - memorizzare un numero di telefono aggiuntivo per il tuo popolo

**Valore di esempio:** 650-555-5555

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Punteggio {#score}

**Nome esempio:** Punteggio comportamentale/Punteggio demografico: crea più campi di punteggio per tenere traccia di attributi diversi.

**Valore di esempio:** 14

**Operatori**: è, non è, tra, maggiore di, minore di, almeno, è vuoto, non è vuoto

## Stringa {#string}

**Nome esempio:** Nome intermedio - Memorizza un attributo di testo aggiuntivo

**Valore di esempio:** Rosa

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## Area di testo {#text-area}

**Nome esempio:** Commenti : aggiungere ai moduli un campo commenti per consentire l’immissione di testo su più righe

**Valore di esempio:** Questo articolo è fantastico!

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto

## URL {#url}

**Nome esempio:** Blog - crea un campo per memorizzare gli url dei blog personali

**Valore di esempio:** www.myblog.com

**Operatori**: è, non è, inizia con, non inizia con, contiene, non contiene, è vuoto, non è vuoto
