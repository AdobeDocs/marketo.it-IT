---
description: Generazione di domande - Documentazione di Marketo - Documentazione del prodotto
title: Generazione di domande
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 9ba9e80e9dcfb2ac835d172635489cc65307270c
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Generazione di domande {#question-generation}

Visualizza tutte le attività e i relativi dettagli pertinenti, ad esempio quando sono state generate, il numero totale di domande, lo stato di approvazione e altro ancora.

## Genera domande {#generate-questions}

1. In IA generativa, fai clic su **Risposte assistite**.

   ![](assets/question-generation-1.png)

1. Clic **Genera domande**.

   ![](assets/question-generation-2.png)

1. Assegna un nome all’attività e inserisci un URL di origine (fino a 50) dal quale verrà estratto tutto il contenuto. Immettere gli argomenti/parole chiave desiderati e premere Invio sulla tastiera. Al termine, fai clic su **Genera**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Affinché il Marketo Engage possa raschiare il contenuto dagli URL forniti, devi prima inserire nell&#39;elenco Consentiti alcuni indirizzi IP. Per evitare che il contenuto venga rimosso dagli URL forniti, devi prima diversi indirizzi IP. [Per ulteriori informazioni, consulta di seguito](#ip-addresses-to-allowlist).

1. In base al contenuto, la generazione di domande e risposte può richiedere fino a 30 minuti. Clic **OK**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Lo stato sulla pagina non viene aggiornato in tempo reale. Premi Aggiorna per vedere quando passa da &quot;Elaborazione&quot; a &quot;Completo&quot;.

   ![](assets/question-generation-5.png)

## Scaricare domande e risposte {#download-questions-and-responses}

>[!NOTE]
>
>Le domande e le risposte generate sono visualizzabili anche in [Libreria di risposte](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Trova l’attività desiderata e fai clic sull’icona Scarica accanto al nome.

   ![](assets/question-generation-6.png)

1. Individua la cartella dei download nel browser e seleziona il file. Questo aspetto può variare a seconda del browser utilizzato.

   ![](assets/question-generation-7.png)

1. Nel file di Excel, **Dettagli attività** mostra solo questo, vari dettagli sull’attività, comprese istruzioni su come aggiungere/modificare domande e/o risposte.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Se decidi di modificare domande e/o risposte in blocco, [scopri come ricaricarli qui](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Il **Domande e risposte** fornisce ulteriori dettagli, incluse le domande e le risposte generate.

   ![](assets/question-generation-9.png)

## Indirizzi IP da Inserire nell&#39;elenco Consentiti per l accesso {#ip-addresses-to-allowlist}

Per abilitare l’estrazione dei contenuti dagli URL web durante la generazione di domande e risposte, assicurati che tutti gli indirizzi IP riportati di seguito siano stati inseriti nell&#39;elenco Consentiti dal team web.

<table width="150">
  <tr>
    <td>20 167 0 149</td>
  </tr>
  <tr>
    <td>20 248 129 111</td>
  </tr>
  <tr>
    <td>20 167 0 146</td>
  </tr>
  <tr>
    <td>20 167 0 205</td>
  </tr>
  <tr>
    <td>20 248 135 80</td>
  </tr>
  <tr>
    <td>20 92 173 115</td>
  </tr>
  <tr>
    <td>20 167 0 195</td>
  </tr>
  <tr>
    <td>20 248 128 31</td>
  </tr>
  <tr>
    <td>20 167 1 48</td>
  </tr>
  <tr>
    <td>20 167 1 63</td>
  </tr>
  <tr>
    <td>20 167 1 92</td>
  </tr>
  <tr>
    <td>20 167 1 155</td>
  </tr>
  <tr>
    <td>20 248 135 132</td>
  </tr>
  <tr>
    <td>20 248 135 108</td>
  </tr>
  <tr>
    <td>20 248 134 140</td>
  </tr>
  <tr>
    <td>20 167 1 242</td>
  </tr>
  <tr>
    <td>20 167 0 198</td>
  </tr>
  <tr>
    <td>20 248 133 185</td>
  </tr>
  <tr>
    <td>20 248 134 190</td>
  </tr>
  <tr>
    <td>20 167 1 254</td>
  </tr>
  <tr>
    <td>20 248 128 118</td>
  </tr>
  <tr>
    <td>20 248 131 252</td>
  </tr>
  <tr>
    <td>20 167 0 188</td>
  </tr>
  <tr>
    <td>20.167.0.201</td>
  </tr>
  <tr>
    <td>20 211 64 11</td>
  </tr>
  <tr>
    <td>20 76 243 87</td>
  </tr>
  <tr>
    <td>20.76.244.212</td>
  </tr>
  <tr>
    <td>20 76 245 48</td>
  </tr>
  <tr>
    <td>20 76 245 76</td>
  </tr>
  <tr>
    <td>20 76 246 63</td>
  </tr>
  <tr>
    <td>20 76 246 146</td>
  </tr>
  <tr>
    <td>20 76 246 248</td>
  </tr>
  <tr>
    <td>20 76 247 92</td>
  </tr>
  <tr>
    <td>20 76 247 134</td>
  </tr>
  <tr>
    <td>20 76 247 244</td>
  </tr>
  <tr>
    <td>20 93 168 10</td>
  </tr>
  <tr>
    <td>20 93 168 44</td>
  </tr>
  <tr>
    <td>20 93 168 137</td>
  </tr>
  <tr>
    <td>20 93 169 20</td>
  </tr>
  <tr>
    <td>20 93 169 115</td>
  </tr>
  <tr>
    <td>20 93 169 214</td>
  </tr>
  <tr>
    <td>20 93 170 130</td>
  </tr>
  <tr>
    <td>20 93 170 138</td>
  </tr>
  <tr>
    <td>20 93 170 149</td>
  </tr>
  <tr>
    <td>20 93 172 63</td>
  </tr>
  <tr>
    <td>20 93 173 217</td>
  </tr>
  <tr>
    <td>20 93 173 243</td>
  </tr>
  <tr>
    <td>20 93 174 120</td>
  </tr>
  <tr>
    <td>20 93 174 159</td>
  </tr>
  <tr>
    <td>20 105 224 16</td>
  </tr>
  <tr>
    <td>20.10.235.102</td>
  </tr>
  <tr>
    <td>20 10 235 103</td>
  </tr>
  <tr>
    <td>20 10 235 143</td>
  </tr>
  <tr>
    <td>20 10 235 146</td>
  </tr>
  <tr>
    <td>20 10 235 147</td>
  </tr>
  <tr>
    <td>20 10 235 148</td>
  </tr>
  <tr>
    <td>20 10 235 188</td>
  </tr>
  <tr>
    <td>20.10.235.189</td>
  </tr>
  <tr>
    <td>20 10 235 246</td>
  </tr>
  <tr>
    <td>20 10 235 248</td>
  </tr>
  <tr>
    <td>20 10 235 255</td>
  </tr>
  <tr>
    <td>20.10.236.96</td>
  </tr>
  <tr>
    <td>20.10.236.97</td>
  </tr>
  <tr>
    <td>20.10.236.110</td>
  </tr>
  <tr>
    <td>20 10 236 111</td>
  </tr>
  <tr>
    <td>20 10 235 254</td>
  </tr>
  <tr>
    <td>20 10 236 138</td>
  </tr>
  <tr>
    <td>20.10.236.139</td>
  </tr>
  <tr>
    <td>20 10 236 140</td>
  </tr>
  <tr>
    <td>20 10 236 141</td>
  </tr>
  <tr>
    <td>20.10.236,84</td>
  </tr>
  <tr>
    <td>20.10.236,85</td>
  </tr>
  <tr>
    <td>20.10.236.86</td>
  </tr>
  <tr>
    <td>20.10.236,87</td>
  </tr>
  <tr>
    <td>20 119 144 14</td>
  </tr>
  <tr>
    <td>20 75 41 107</td>
  </tr>
  <tr>
    <td>20 75 43 104</td>
  </tr>
  <tr>
    <td>20 75 43 107</td>
  </tr>
  <tr>
    <td>20.75.43.113</td>
  </tr>
  <tr>
    <td>20 75 43 124</td>
  </tr>
  <tr>
    <td>20.75.43.204</td>
  </tr>
  <tr>
    <td>20.75.43.207</td>
  </tr>
  <tr>
    <td>20.75.43.214</td>
  </tr>
  <tr>
    <td>20.75.43.220</td>
  </tr>
  <tr>
    <td>20.75.44.0</td>
  </tr>
  <tr>
    <td>20.75.44.9</td>
  </tr>
  <tr>
    <td>20.75.44.52</td>
  </tr>
  <tr>
    <td>20 75 44 66</td>
  </tr>
  <tr>
    <td>20.75.44.82</td>
  </tr>
  <tr>
    <td>20.75.44.105</td>
  </tr>
  <tr>
    <td>20 75 44 108</td>
  </tr>
  <tr>
    <td>20 75 44 133</td>
  </tr>
  <tr>
    <td>20.75.44.135</td>
  </tr>
  <tr>
    <td>20 75 44 137</td>
  </tr>
  <tr>
    <td>20 75 44 147</td>
  </tr>
  <tr>
    <td>20 75 44 154</td>
  </tr>
  <tr>
    <td>20.75.44.195</td>
  </tr>
  <tr>
    <td>20.75.44.198</td>
  </tr>
  <tr>
    <td>20.75.45.32</td>
  </tr>
  <tr>
    <td>20 119 136 14</td>
  </tr>
  <tr>
    <td>172 177 93 157</td>
  </tr>
  <tr>
    <td>52 252 22 155</td>
  </tr>
  <tr>
    <td>20.62.18.64</td>
  </tr>
  <tr>
    <td>52 179 234</td>
  </tr>
  <tr>
    <td>52 179 234,1</td>
  </tr>
  <tr>
    <td>52 179 237 99</td>
  </tr>
  <tr>
    <td>52 179 237 148</td>
  </tr>
  <tr>
    <td>52 252 23 246</td>
  </tr>
  <tr>
    <td>52 253 64 47</td>
  </tr>
  <tr>
    <td>52 253 64 124</td>
  </tr>
  <tr>
    <td>52 253 64 125</td>
  </tr>
  <tr>
    <td>52 253 65 84</td>
  </tr>
  <tr>
    <td>52 253 65 85</td>
  </tr>
  <tr>
    <td>52 254 103 240</td>
  </tr>
  <tr>
    <td>52 253 65 92</td>
  </tr>
  <tr>
    <td>52 253 65 93</td>
  </tr>
  <tr>
    <td>52 177 89 135</td>
  </tr>
  <tr>
    <td>52 253 69 207</td>
  </tr>
  <tr>
    <td>52 253 69 240</td>
  </tr>
  <tr>
    <td>52 167 19 211</td>
  </tr>
  <tr>
    <td>52 177 147 229</td>
  </tr>
  <tr>
    <td>40 65 238 53</td>
  </tr>
  <tr>
    <td>52 177 147 249</td>
  </tr>
  <tr>
    <td>20 44 83 102</td>
  </tr>
  <tr>
    <td>52 177 148 19</td>
  </tr>
  <tr>
    <td>20.49.97.17</td>
  </tr>
  <tr>
    <td>20.14.171,7</td>
  </tr>
  <tr>
    <td>172 177 93 157</td>
  </tr>
  <tr>
    <td>20 213 91 77</td>
  </tr>
  <tr>
    <td>20 105 150 224</td>
  </tr>
  <tr>
    <td>13 68 17 252</td>
  </tr>
</table>