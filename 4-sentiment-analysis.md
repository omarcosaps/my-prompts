# Análise de Sentimento de Reviews

## Objetivo

Analise as avaliações contidas no arquivo **`{{ARQUIVO_CSV}}`** e classifique o sentimento de cada review.

---

## Arquivo de Entrada

- **Arquivo:** `{{ARQUIVO_CSV}}`
- **Localização:** `{{CAMINHO_DO_ARQUIVO}}`

---

## Tarefa

1. Leia todas as reviews presentes no arquivo CSV.
2. Adicione uma nova coluna chamada **`sentimento`**.
3. Classifique cada review utilizando apenas uma das categorias abaixo:
   - `satisfeito`
   - `insatisfeito`
   - `neutro`

---

## Critérios de Classificação

A classificação deve ser baseada principalmente na leitura completa da review, considerando:

- O significado da mensagem.
- A intenção do cliente.
- O tom da escrita.
- Emoções expressas.
- Contexto geral.
- Ironias, sarcasmo ou contradições.

A análise deve representar o que o cliente realmente quis comunicar, e não apenas palavras isoladas.

### Uso da nota (rating)

A nota deve ser utilizada **apenas como apoio**, quando:

- o texto for muito curto;
- houver ambiguidade;
- não existirem informações suficientes para identificar claramente o sentimento.

Em situações normais, a classificação deve ser baseada exclusivamente no texto da review.

---

## Regras

- Não altere nenhuma coluna existente.
- Preserve a ordem original das linhas.
- Crie apenas a coluna **`sentimento`**.
- Não modifique o conteúdo das reviews.
- Mantenha o arquivo no formato CSV.

---

## Resultado Esperado

O arquivo original deve ser atualizado contendo uma nova coluna chamada **`sentimento`**, mantendo todas as demais informações inalteradas.

Exemplo:

| review | rating | sentimento |
|--------|-------:|------------|
| Excelente atendimento e entrega rápida. | 5 | satisfeito |
| O produto chegou quebrado e ninguém respondeu. | 1 | insatisfeito |
| Recebi conforme anunciado. | 3 | neutro |

---

## Variáveis

| Variável | Descrição |
|----------|-----------|
| `{{ARQUIVO_CSV}}` | Nome do arquivo CSV que será analisado. |
| `{{CAMINHO_DO_ARQUIVO}}` | Caminho onde o arquivo está localizado. |
