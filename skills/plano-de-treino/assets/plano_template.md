# Template de Saída: Plano de Treino

## 🏋️ Plano de Treino: [Objetivo]

**Nível:** [Iniciante/Intermediário/Avançado] · **Frequência:** [Dias da Semana] às [HH:MM]  
**Divisão:** [Ex: Treino A / Treino B / Treino C]

### 1. Fichas de Treino Detalhadas

#### 🔴 Treino A: [Foco, Ex: Peito e Tríceps]
| # | Aparelho / Exercício | Séries | Repetições | Descanso |
|---|---|---|---|---|
| 1 | Supino Reto (Barra/Móvel) | 3 | 10 - 12 | 60s |
| 2 | Crossover (Cabo) | 3 | 12 - 15 | 45s |
| 3 | Tríceps Pulley | 3 | 10 - 12 | 45s |

#### 🔵 Treino B: [Foco, Ex: Costas e Bíceps]
| # | Aparelho / Exercício | Séries | Repetições | Descanso |
|---|---|---|---|---|
| 1 | Puxada Frontal | 3 | 10 - 12 | 60s |
| 2 | Remada Baixa | 3 | 10 - 12 | 60s |
| 3 | Rosca Direta (Halter/Cabo) | 3 | 10 - 12 | 45s |

*(Adicione os demais treinos A, B, C conforme a frequência)*

### 2. Checkpoints e Progressão
- **Check do Treino:** Concluir a ficha inteira do dia.
- **Check do Aparelho:** Marcar a execução de cada exercício na lista.
- **Check da Série:** Registrar cada série finalizada no aparelho.

### 3. Importação no Google Agenda
1. Baixe o arquivo `plano-de-treino.csv`.
2. No Google Agenda: **Configurações ⚙️ → Importar e exportar → Importar**.

---

## Regras Obrigatórias do CSV do Google Agenda

O arquivo `plano-de-treino.csv` deve conter **exclusivamente os treinos diários** (sem criar um evento para cada aparelho):

1. **Cabeçalho:** `Subject,Start Date,Start Time,End Date,End Time,Description`
2. **Formato de Data:** `MM/DD/YYYY`
3. **Formato de Hora:** `HH:MM AM/PM` (Ex: `07:00 AM`)
4. **Subject:** `🏋️ Treino A: Peito e Tríceps`
5. **Description:** Resume o treino e aparelhos em texto corrido entre aspas.  
   *Exemplo:* `"Treino A: Supino Reto (3x12), Crossover (3x12), Tríceps Pulley (3x12)"`
