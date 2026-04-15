# 🗺️ Roadmap — SPai Portal

> 2 épicos · 16 histórias mapeadas

---

## Sumário

- [🔵 Épico 1 · Comunicações](#-épico-1--comunicações) — 5 histórias
- [🟣 Épico 2 · Mapeamento de Dados](#-épico-2--mapeamento-de-dados-data-mapping) — 11 histórias

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

- [X] BACK
- [x] FRONT

---

### História 2 · Inativação de comunicação

> Permitir inativar uma comunicação sem removê-la.

**Labels:** `Feature` `Backend`

**Tarefas:**

    - Criar flag de status (ativo/inativo)
    - Ajustar listagem para respeitar status
    - Impedir uso de comunicações inativas

**Progresso:**

- [X] BACK
- [x] FRONT

---

### História 3 · Definição de comunicação padrão

> Permitir definir uma comunicação como padrão.

**Labels:** `Feature` `Backend` `Frontend`

**Tarefas:**

    - Criar campo de "comunicação padrão"
    - Aplicar fallback automático

**Progresso:**

- [X] BACK
- [x] FRONT

---

### História 4 · Priorização de critérios

> Permitir definir prioridade entre critérios de comunicação.

**Labels:** `Feature` `Validação`

**Tarefas:**

    - Criar campo de prioridade
    - Validar conflitos entre critérios

**Progresso:**

- [x] BACK
- [x] FRONT

---

### História 5 · Refinamento da edição de critérios

> Melhorar a experiência e a persistência da edição de critérios na tela de comunicações.

**Labels:** `Feature` `Frontend` `UX/Design`

**Tarefas:**

    - Remover botão global de salvar durante a edição
    - Remover ícone de lixeira no modo de edição
    - Usar PUT para atualização de critério existente (ícone de check)
    - Usar PATCH para inclusão de novo critério em edição (ícone de plus)
    - Garantir que o PATCH de inclusão envie apenas o novo critério
    - Reorganizar layout dos campos (Campo em linha separada + Operador/Valor/Prioridade abaixo)
    - Melhorar destaque visual dos botões de ação (check/plus)
    - Exibir feedback de erro quando houver falha nas chamadas de API
    - Feedback visual indicando detalhes sobre prioridade

**Progresso:**

- [x] FRONT

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

- [X] BACK
- [X] FRONT

---

### História 10 · Validação de uso de campos

> Evitar alterações inválidas em campos utilizados como favoritos.

**Labels:** `Validação` `Backend` `Frontend`

**Tarefas:**

    - Impedir remoção se usado em critérios
    - Validar dependências antes de alteração
    - Exibir mensagens de erro claras

**Progresso:**

- [X] BACK
- [X] FRONT

---

### História 11 · Correção de visualização de máscaras e campos

> Melhorar exibição de máscaras e campos no Data Mapping.

**Labels:** `UX/Design` `Frontend`

**Tarefas:**

    - Identificar corretamente campos de máscara
    - Separar visualmente: Data Mapping original, Campos criados e Máscaras
    - Ajustar filtros de visualização

**Progresso:**

- [x] FRONT

---

### História 12 · Criação de campos derivados (Field Mapping)

> Permitir criação de novos campos com base em outros.

**Labels:** `Feature` `Frontend` `Backend`

**Tarefas:**

    - Criar campo dentro de um nó pai
    - Permitir seleção de função (máscara/formatação)
    - Permitir múltiplos parâmetros

**Progresso:**

- [X] BACK
- [X] FRONT

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

- [X] BACK
- [X] FRONT

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

---

### História 15 · Exibição de erro ao layout sem sessões na tela de comunicações

> Se o layout não tiver sessões configuradas, o frontend deve exibir um erro na tela de comunicações.

**Labels:** `Validação` `Frontend`

**Tarefas:**

    - Verificar se o layout possui sessões configuradas ao carregar a tela de comunicações
    - Exibir mensagem de erro clara quando nenhuma sessão estiver configurada
    - Bloquear ações dependentes de sessão enquanto o erro estiver ativo

**Progresso:**

- [ ] BACK
- [ ] FRONT

---

### História 16 · Atualização do content-type nas requisições de FieldMapping

> Adaptar o frontend para enviar requisições ao endpoint de FieldMapping usando `application/json` em vez de `multipart/form-data`, conforme atualização do backend.

**Labels:** `Feature` `Frontend`

**Tarefas:**

    - Atualizar as chamadas de POST e PUT de FieldMapping para enviar o corpo como JSON
    - Remover o uso de FormData nessas requisições
    - Validar que os dados enviados continuam corretos após a mudança de formato

**Progresso:**

- [x] FRONT
