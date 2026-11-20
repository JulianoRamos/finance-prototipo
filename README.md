# Protótipo do finance

As telas do finance, desenhadas no Claude Design sobre o design system do projeto. Cada tela é um arquivo `<Tela>.dc.html` na raiz, citado pelo nome sem a extensão nas specs e nos tickets, sempre num commit fixo.

O protótipo anda à frente do código: ele nunca é o escopo. O escopo é o recorte que a spec e o ticket fazem de cada tela. A linguagem visual é a do `docs/design-system.md` do repositório do finance.

Este repositório é público: as telas só trazem dados fictícios.

## Telas da fase 1

| Tela | O que mostra |
| --- | --- |
| `Login` | Entrar com e-mail e senha, com o estado de erro |
| `DefinirSenha` | Definir a senha pelo link de uso único, com o estado de link vencido |
| `RecuperarAcesso` | Como pedir um link de recuperação, já que o sistema não envia e-mail |
| `Inicio` | A estrutura do app (barra lateral, barra superior, cabeçalho e corpo) e o seletor de contexto financeiro |
| `Sessoes` | Minha conta: as sessões ativas, com o menu de ações de cada uma, e a troca de senha |
| `Pesquisa` | A paleta de pesquisa, com sugestões, resultados e o estado vazio |
| `Entidades` | A lista de entidades e o detalhe da empresa, com as operações e as participações societárias, e os formulários de criar, editar, registrar e encerrar participação |
| `GruposFinanceiros` | Os grupos financeiros, os membros da Visão Familiar, e criar, editar e excluir um grupo |
| `Usuarios` | Os usuários, a permissão por entidade, o link de recuperação, e criar, editar e desativar um usuário |
| `HistoricoRegistro` | O histórico de alterações de um registro, num painel lateral sobre Entidades |

## Telas da fase 2

| Tela | O que mostra |
| --- | --- |
| `Contas` | A lista de contas do contexto, com o saldo de cada uma, e o detalhe da conta, com os saldos (hoje, numa data e o inicial) e as movimentações; os formulários de criar e editar, e os diálogos de nova movimentação, ajustar o saldo e desativar |
| `ContasCelular` | Contas no celular: a lista, o detalhe como página própria, as movimentações como lista, o formulário com as ações fixas no rodapé e os diálogos como folha |

## Estados

Cada tela mostra os estados por opções do Claude Design. Uma spec ou um ticket cita o estado pelo nome da opção e do valor, como `Entidades`, modo `nova`.

| Opção | Telas | Valores |
| --- | --- | --- |
| `erro` | `Login` | ligado ou desligado |
| `estado` | `DefinirSenha` | `formulário`, `link vencido` |
| `estado` | `Pesquisa` | `sugestoes`, `resultados`, `vazio` |
| `rolagem` | Telas do app | `topo` (com o cabeçalho da página), `rolada` (sem ele) |
| `barra` | Telas do app | `expandida`, `recolhida` |
| `menu` | Telas do app, salvo `Pesquisa` e `HistoricoRegistro` | `nenhum`, `contexto`, `usuario`, `configuracoes` |
| `modo` | `Entidades` | `detalhe`, `nova`, `editar`, `participacao`, `encerrar`, `desligar` |
| `modo` | `GruposFinanceiros` | `detalhe`, `novo`, `editar`, `excluir`, `excluir_com_metas` |
| `modo` | `Usuarios` | `detalhe`, `novo`, `criado`, `editar`, `desativar` |
| `lista` | `Entidades`, `HistoricoRegistro`, `Sessoes` | `muitas` (10 por página, com a paginação no rodapé), `poucas` |
| `lista` | `GruposFinanceiros`, `Usuarios` | `muitos` (10 por página, com a paginação no rodapé), `poucos` |
| `acoes` | `Sessoes` | `fechado`, `aberto` (o menu de ações da linha aberto) |
| `estado` | `Contas` | `lista`, `vazia`, `carregando`, `erro` |
| `modo` | `Contas` | `detalhe`, `nova`, `editar`, `movimentacao`, `ajuste`, `desativar` |
| `tela` | `ContasCelular` | `lista`, `detalhe`, `nova`, `movimentacao`, `ajuste`, `desativar` |
