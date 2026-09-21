# Relatório de Comparação dos Modelos

## Sprint 03 - Chatbot GoodWe

### Objetivo

Nesta Sprint fizemos testes com dois modelos diferentes para ver qual deles funcionaria melhor no chatbot da GoodWe.

Os modelos escolhidos foram:

- GPT-4o-mini
- GPT-4.1-mini

Para não favorecer nenhum dos dois, usamos as mesmas perguntas e os mesmos dados nos testes.

## Modelos utilizados

Os dois modelos foram utilizados com o OpenAI Agents SDK.

O GPT-4o-mini ficou como modelo do nosso agente principal e o GPT-4.1-mini foi adicionado para conseguirmos fazer a comparação.

Os dois tiveram acesso às mesmas ferramentas de consulta dos dados dos carregadores durante os testes.

## Testes realizados

Fizemos 5 perguntas para cada modelo:

1. Existem carregadores disponíveis?
2. Qual o tempo de espera atual?
3. Qual o faturamento de hoje?
4. Quantas sessões de carregamento foram realizadas hoje?
5. Existe algum carregador com falha ou em manutenção?

Depois comparamos as respostas com os dados que estavam sendo usados pelo sistema.

## Resultados

Os dois modelos conseguiram responder corretamente as 5 perguntas.

| Modelo | Testes | Respostas adequadas |
|---|---:|---:|
| GPT-4o-mini | 5 | 5 |
| GPT-4.1-mini | 5 | 5 |

Nesse ponto os dois tiveram praticamente o mesmo resultado, já que nenhum apresentou uma resposta que consideramos inadequada.

## Tempo de resposta

Também medimos o tempo de uma execução de cada modelo.

| Modelo | Tempo observado |
|---|---:|
| GPT-4o-mini | 2,08 segundos |
| GPT-4.1-mini | 2,56 segundos |

O GPT-4o-mini foi um pouco mais rápido nesse teste.

Esse tempo não significa que ele sempre vai responder nessa velocidade, porque fizemos apenas uma medição e o resultado pode mudar em outras execuções.

## Diferenças encontradas

Nas respostas não percebemos uma diferença muito grande. Os dois modelos entenderam as perguntas e conseguiram buscar os dados corretos.

A diferença mais fácil de perceber foi no tempo de resposta. No teste realizado, o GPT-4o-mini respondeu em 2,08 segundos e o GPT-4.1-mini em 2,56 segundos.

Como foi apenas uma execução, usamos esse resultado somente como uma comparação do nosso teste.

## Vantagens e limitações

### GPT-4o-mini

O modelo respondeu corretamente todos os testes e teve o menor tempo na medição que fizemos.

Outra vantagem foi que ele já estava sendo usado no agente principal junto com as ferramentas, memória e sistema de segurança.

Como limitação, ele depende da API da OpenAI e o tempo das respostas pode variar.

### GPT-4.1-mini

O GPT-4.1-mini também respondeu corretamente as cinco perguntas e conseguiu trabalhar com os mesmos dados utilizados pelo outro modelo.

No nosso teste ele demorou um pouco mais para responder.

Assim como o GPT-4o-mini, ele também depende da API e seu tempo de resposta pode mudar entre uma execução e outra.

## Modelo escolhido

Depois dos testes decidimos continuar utilizando o GPT-4o-mini como modelo principal.

Os dois modelos acertaram as 5 perguntas, então a qualidade das respostas ficou bem parecida nos testes que fizemos.

O GPT-4o-mini teve um tempo menor na nossa medição e já estava funcionando no agente principal junto com a memória, as ferramentas e os guardrails.

Por isso decidimos manter ele na versão final do projeto.

## Conclusão

Os testes foram importantes para não escolhermos o modelo apenas por preferência.

Os dois modelos tiveram bons resultados e responderam corretamente às perguntas. Mesmo assim, pelos resultados que tivemos e pela forma como ele já estava integrado ao projeto, escolhemos continuar com o GPT-4o-mini.

Com essa comparação conseguimos testar na prática dois modelos antes de decidir qual utilizar na versão final do chatbot.