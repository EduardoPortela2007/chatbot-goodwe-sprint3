# Chatbot GoodWe - Sprint 03

Projeto desenvolvido para a Sprint 03 do curso de Ciência da Computação da FIAP.

O objetivo do projeto é criar um chatbot para auxiliar na consulta de informações sobre carregadores elétricos, como disponibilidade, tempo de espera, sessões realizadas, faturamento, manutenção e falhas.

## Tecnologias utilizadas

- Python
- Google Colab
- OpenAI Agents SDK
- OpenAI API
- SQLiteSession

## Como funciona

Na Sprint 03 o chatbot foi desenvolvido utilizando agentes.

O agente possui ferramentas para consultar os dados simulados dos carregadores e utiliza SQLiteSession para manter o histórico da conversa.

Também foi criado um guardrail para verificar as mensagens recebidas e bloquear pedidos fora do escopo ou que possam apresentar riscos.

## Modelos testados

Durante o projeto foram testados dois modelos:

- GPT-4o-mini
- GPT-4.1-mini

Os dois responderam adequadamente às 5 perguntas utilizadas nos testes funcionais.

Após os testes, o GPT-4o-mini foi mantido como modelo principal.

## Testes

Foram realizados testes de:

- Funcionamento do chatbot
- Memória da conversa
- Prompt Injection
- Assuntos fora do escopo
- Instruções elétricas perigosas
- Informações técnicas inventadas
- Aconselhamento jurídico
- Aconselhamento financeiro

Os testes completos estão no arquivo `testes.md`.

## Como executar

O projeto foi desenvolvido no Google Colab.

Para executar:

1. Abra o arquivo do projeto no Google Colab.
2. Execute a célula de instalação das dependências.
3. Adicione sua chave da OpenAI nos Secrets do Google Colab.
4. Execute as células do notebook na ordem.

A chave da API não deve ser colocada diretamente no código nem enviada para o GitHub.

## Arquivos

- `GoodWe_Sprint03` - código principal do projeto
- `relatorio_modelos.md` - comparação entre os modelos
- `testes.md` - testes realizados
- `Relatorio_Evolucao_GoodWe_Sprint03.pdf` - relatório de evolução
- `integrantes.txt` - integrantes do grupo

## Integrantes

- Bruno Riquelme Coutinho Pereira - RM 569619
- Eduardo Bigoli Portela - RM 569897
- Gabriel Martins Cordeiro Rodrigues - RM 570497
- Gustavo Fondato de Souza - RM 573651
- Gustavo Martins da Silva - RM 570584
- Lucas Lino Marques da Silva - RM 572863