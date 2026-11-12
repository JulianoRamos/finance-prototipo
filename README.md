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
| `Inicio` | A estrutura do app e o seletor de contexto financeiro aberto |
| `Sessoes` | As sessões ativas e a troca de senha |
| `Entidades` | A lista de entidades e o detalhe da empresa, com a operação de clínica e as participações societárias |
| `GruposFinanceiros` | Os grupos financeiros e os membros da Visão Familiar |
| `Usuarios` | Os usuários, a permissão por entidade e o link de recuperação |
| `HistoricoRegistro` | O histórico de alterações de um registro |
