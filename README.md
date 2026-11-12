# Estoque de Vídeos

Página de acompanhamento do estoque de vídeos de um canal de YouTube: fila de postagem, plano por dia, histórico de desempenho, totais mensais do canal e relatório mensal.

Versão da fórmula: 1.0

## O que tem aqui

- `index.html`: a estrutura da página e as abas (Estoque, Histórico, Canal, Relatório).
- `styles.css`: o visual.
- `js/base.js`: funções de apoio, cores por jogo e leitura das capas.
- `js/estoque.js`: aba Estoque, com o gráfico de notas, o plano de postagem e o cadastro de vídeos.
- `js/historico.js`: aba Histórico, com maturação, resultados e tabela.
- `js/canal.js`: aba Canal, com os totais mês a mês e o acumulado.
- `js/relatorio.js`: aba Relatório mensal.
- `js/main.js`: troca de abas e carregamento dos dados.

## Os dados não estão no repositório

Esta página lê e grava os dados em um banco do claude.ai (coleções `videos`, `historico`, `ranking`, `config`, `desempenho`, `relatorios` e `meses`). Por isso:

- Sem o banco, a página abre, mas mostra "A lista não está disponível nesta visualização".
- Para usar em outro lugar, é preciso trocar a camada de dados (`claude.use("db")` em `js/main.js`) por um banco próprio e recriar as coleções.

Nenhum dado de canal, vídeo ou receita está nos arquivos deste repositório.

## Como abrir

Abra `index.html` no navegador. Para ver dados reais, a página precisa rodar dentro do claude.ai como artefato.
