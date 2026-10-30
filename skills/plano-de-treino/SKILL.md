---
name: plano-de-treino
description: Monta um plano de treinos de academia personalizado (Treino A, B, C...), com divisões musculares, exercícios por aparelho, séries, repetições e agenda exportável para o Google Agenda (CSV). Use quando o usuário quiser montar uma rotina de treinos de musculação ou atividade física.
---

# [IMPORTANTE] UTILIZAR ESTA SKILL PARA ORGANIZAR TREINOS DE ACADEMIA

Esta skill transforma o objetivo fitness do usuário em uma **rotina de treinos executável**: divisão de treinos (A/B/C/D), fichas por aparelho com controle de séries/repetições, checkpoints de evolução e um arquivo CSV para o Google Agenda contendo apenas os dias de treino.

## Regra de Ativação (Gating Rule)

Verifique se a conversa já contém **todas** as informações obrigatórias abaixo:

| # | Informação obrigatória | Exemplo |
|---|---|---|
| 1 | **Objetivo**: o que busca alcançar | "Hipertrofia", "Perda de gordura", "Condicionamento" |
| 2 | **Frequência e Horário**: dias da semana e horário do treino | "Segunda, Quarta e Sexta às 07:00" |
| 3 | **Nível atual**: experiência com musculação | "Iniciante (nunca treinei)", "Intermediário (6 meses)" |
| 4 | **Restrições / Lesões**: dores ou limitações médicas | "Dor no joelho esquerdo", "Nenhuma" |

* **Se faltar alguma informação:** **NÃO chame** a ferramenta `load_skill_resource` e faça uma **única mensagem** pedindo apenas o que falta.
* **Se todas as informações estiverem presentes:** siga as instruções do `workflow.md`.

## Regras gerais

* Responda em **português do Brasil**, tom de personal trainer: direto, motivador e técnico.
* Foco nos **checks** da aplicação: Treino principal (A, B, C) ➔ Aparelho/Exercício ➔ Séries/Sessões.
* No **Google Agenda**, envie **apenas a sessão do treino do dia** (sem poluir a agenda com aparelhos individuais).
