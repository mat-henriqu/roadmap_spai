# 🗺️ Roadmap — SPai Portal

> 2 épicos · 14 histórias mapeadas

---

## Sumário

- [🔵 Épico 1 · Comunicações](#-épico-1--comunicações) — 4 histórias
- [🟣 Épico 2 · Mapeamento de Dados](#-épico-2--mapeamento-de-dados-data-mapping) — 9 histórias

---

## 🔵 Épico 1 · Comunicações

### História 1 · Edição de critérios de comunicação

> Permitir editar critérios já cadastrados em comunicações.

**Labels:** `Feature` `Backend` `Frontend`

**Tarefas:**

    - Implementar edição de critérios existentes
    - Garantir persistência das alterações no backend
    - Validar impacto em comunicações já associadas

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 2 · Inativação de comunicação

> Permitir inativar uma comunicação sem removê-la.

**Labels:** `Feature` `Backend`

**Tarefas:**

    - Criar flag de status (ativo/inativo)
    - Ajustar listagem para respeitar status
    - Impedir uso de comunicações inativas

**Progresso:**

- [ ] BACK

---

### História 3 · Definição de comunicação padrão

> Permitir definir uma comunicação como padrão.

**Labels:** `Feature` `Backend` `Frontend`

**Tarefas:**

    - Criar campo de "comunicação padrão"
    - Aplicar fallback automático

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 4 · Priorização de critérios

> Permitir definir prioridade entre critérios de comunicação.

**Labels:** `Feature` `Validação`

**Tarefas:**

    - Criar campo de prioridade
    - Validar conflitos entre critérios

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

## 🟣 Épico 2 · Mapeamento de Dados (Data Mapping)

### História 6 · Padronização de telas

> Padronizar UI/UX entre telas de mapeamento.

**Labels:** `UX/Design` `Frontend`

**Tarefas:**

    - Unificar estrutura (árvore vs breadcrumb)
    - Aplicar padrão visual único
    - Revisar navegação

**Progresso:**

- [x] FRONT

---

### História 7 · Upload e configuração de Data Mapping

> Melhorar o processo de upload de planilhas.

**Labels:** `Feature` `Backend` `Frontend`

**Tarefas:**

    - Permitir leitura de planilhas
    - Configurar vínculo com billing
    - Tornar configurações dinâmicas (não fixas)

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 8 · Reutilização de configurações

> Permitir copiar configurações entre versões de Data Mapping.

**Labels:** `Feature` `Backend`

**Tarefas:**

    - Criar função de clonagem (ex: V36 → V37)
    - Garantir consistência dos dados copiados

**Progresso:**

- [ ] BACK

---

### História 9 · Marcação de campos importantes (Field Mapping Report)

> Permitir marcar campos como importantes.

**Labels:** `Feature` `Frontend` `Backend`

**Tarefas:**

    - Adicionar flag (estrela/favorito)
    - Persistir no banco
    - Permitir seleção/deseleção

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 10 · Validação de uso de campos

> Evitar alterações inválidas em campos utilizados como favoritos.

**Labels:** `Validação` `Backend` `Frontend`

**Tarefas:**

    - Impedir remoção se usado em critérios
    - Validar dependências antes de alteração
    - Exibir mensagens de erro claras

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 11 · Correção de visualização de máscaras e campos

> Melhorar exibição de máscaras e campos no Data Mapping.

**Labels:** `UX/Design` `Frontend`

**Tarefas:**

    - Identificar corretamente campos de máscara
    - Separar visualmente: Data Mapping original, Campos criados e Máscaras
    - Ajustar filtros de visualização

**Progresso:**

- [ ] FRONT

---

### História 12 · Criação de campos derivados (Field Mapping)

> Permitir criação de novos campos com base em outros.

**Labels:** `Feature` `Frontend` `Backend`

**Tarefas:**

    - Criar campo dentro de um nó pai
    - Permitir seleção de função (máscara/formatação)
    - Permitir múltiplos parâmetros

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 13 · Regras para uso de campos base

> Garantir que apenas campos válidos sejam usados como base.

**Labels:** `Validação` `Backend` `Frontend`

**Regras de negócio:**

- Apenas campos originais do Data Mapping
- Não pode ser campo derivado (filho)
- Deve ser último nível da cadeia (sem filhos)

**Tarefas:**

    - Implementar validação no backend
    - Ajustar filtros no frontend
    - Atualizar endpoints necessários

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 14 · Ajustes de API (Backend)

> Adequar APIs para suportar novas regras.

**Labels:** `API` `Backend`

**Tarefas:**

    - Criar endpoint para Data Mapping original
    - Ajustar retorno de FieldMaps (com/sem máscara)
    - Garantir suporte a múltiplos parâmetros

**Progresso:**

- [ ] BACK
