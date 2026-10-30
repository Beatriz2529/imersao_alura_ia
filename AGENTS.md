# AGENTS.md: Agente de Treinos de Academia

## Goal

Construir o **`agente-treinos`**: um agente **Google ADK** (Python) movido a skills, que gera planos de treino personalizados a partir da skill `skills/plano-de-treino/`. O plano inclui divisão de treinos (Ex: A, B, C), ficha detalhada com exercícios/aparelhos, séries, repetições, checkpoints de evolução/execução e exportação dos treinos para o **Google Agenda** (CSV). O agente salva essa agenda em arquivo com o **EnvironmentToolset** do ADK.

## Context

* **Foco do Projeto:** Sistema de academia focado em acompanhamento e check-in. O usuário pode fazer check do treino (A, B, C), check do aparelho e check da série/sessão realizada.
* **Integração com Google Agenda:** Serão agendados **apenas os dias de treino** no Google Agenda (não aparelhos ou séries individuais), indicando qual treino será realizado naquele dia (ex: "🏋️ Treino A: Peito e Tríceps").
* **Skills do ADK:** `load_skill_from_dir` com `SkillToolset`.
  * **L1:** `name` e `description` no frontmatter de `SKILL.md`.
  * **L2:** O corpo do `SKILL.md` (regras e gating).
  * **L3:** `references/workflow.md`, `references/tecnicas.md`, `references/salvar_agenda.md`, `assets/plano_template.md` e `assets/exemplo_plano.md`.

## Constraints

* **Gating:** Requer Objetivo (hipertrofia, emagrecimento, etc.), Dias/Frequência semanal, Nível atual e Restrições/Lesões.
* **Google Agenda:** Salva apenas os eventos de treino com `WriteFile` em `plano-de-treino.csv`.
