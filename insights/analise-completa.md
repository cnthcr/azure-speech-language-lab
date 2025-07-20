# 🎧 INSIGHTS - Azure Speech Studio & Language Studio  
**Música analisada:** *"Adult Girl"* – MARINA

---

## 🎙️ Speech Studio – Transcrição de Áudio

### ✅ O que foi feito:
Utilizei o Azure Speech Studio para converter a música em texto (*speech-to-text*), a partir de um trecho da faixa *"Adult Girl"*.

### 🔍 Resultado obtido:
O serviço conseguiu captar fragmentos da letra, porém com diversas falhas de compreensão e cortes no texto.

> **Transcrição gerada:**  
> “My age, but the child will be. She wants to scream and cry and rage and who am I to her grave? The teenage years are never lived…”

> **Trecho original correspondente:**  
> “Try my best to act my age, but the child won't behave. She wants to scream and cry and rage. And who am I to take her grave?”

### ⚠️ Principais dificuldades observadas:
- O Speech Studio não conseguiu identificar a música por completo.
- Houve perda de trechos importantes e substituições incorretas de palavras.
- A qualidade da transcrição pode ter sido impactada por:
  - Música de fundo e vocais melódicos  
  - Estilo vocal da cantora  
  - Limitações na detecção de áudio artístico/cantado

### 💡 O que poderia melhorar:
- Utilizar trechos de voz limpa (sem música)
- Usar áudios falados, como podcasts ou depoimentos
- Inserir legendas manuais para treinar modelos personalizados

---

## 🧠 Language Studio – Análise de Sentimentos

### ✅ O que foi feito:
A transcrição gerada foi utilizada no Azure Language Studio para análise de linguagem natural, especialmente para detectar sentimentos.

### 🔍 Resultado da análise:

| Trecho                                                                 | Sentimento | Score |
|------------------------------------------------------------------------|------------|--------|
| “She wants to scream and cry and rage...”                              | Negativo   | 0.61   |
| “The teenage years I never lived... carefree joy and pure delight...” | Positivo   | 0.68   |
| “Spent my twenties on the run dreamin' of suicide and love...”        | Negativo   | 0.67   |
| “Messy numb razors and knives... Robbed me of a teenage world...”     | Negativo   | 0.95   |
| “Someone, tell me how to heal the terror livin’ inside me...”         | Neutro     | 0.54   |
| “All the things I lost and loved… Now I understand the world of adult boys…” | Positivo | 0.92   |

### 💡 Observações:
- O modelo detectou sentimentos com precisão em trechos emocionalmente carregados.
- Trechos com ambiguidade poética foram classificados como neutros ou mistos.
- Mesmo com uma transcrição incompleta, os resultados foram coerentes.

---

## 🧾 Conclusão

O uso combinado do Speech Studio e do Language Studio permitiu entender na prática como funcionam os modelos de IA da Azure para voz e linguagem. Apesar das limitações na transcrição de música cantada, a análise de sentimentos foi bastante satisfatória.

### ➡️ Recomendações para próximos testes:
- Utilizar áudios falados com clareza
- Inserir transcrições manuais como referência
- Aplicar em casos reais, como atendimento, entrevistas e diálogos
