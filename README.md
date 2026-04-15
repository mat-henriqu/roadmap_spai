# 🗺️ roadmap_spai

Repositório de acompanhamento do roadmap do **SPai Portal**.

Aqui, eu e os demais devs do time registramos as histórias planejadas e marcamos o progresso de cada entrega conforme avançamos no desenvolvimento.

---

## 📋 Como usar

1. Abra o arquivo [`todo.md`](./todo.md) — ele contém todos os épicos e histórias do roadmap.
2. Ao concluir uma tarefa de backend ou frontend, marque o checkbox correspondente:
   - `- [ ] BACK` → `- [x] BACK`
   - `- [ ] FRONT` → `- [x] FRONT`
3. Faça commit da alteração com uma mensagem descritiva, por exemplo:
   ```
   feat: marca História 1 BACK como concluída
   ```
4. Abra um Pull Request para que o time revise e aprove a atualização do progresso.

---

## 📁 Estrutura

| Arquivo | Descrição |
|---------|-----------|
| [`todo.md`](./todo.md) | Roadmap completo com épicos, histórias e checklist de progresso |
| [`README.md`](./README.md) | Este arquivo — instruções de uso do repositório |

---

## 🗂️ Épicos

| # | Épico | Histórias |
|---|-------|-----------|
| 🔵 1 | [Comunicações](./todo.md#-épico-1--comunicações) | 4 |
| 🟣 2 | [Mapeamento de Dados (Data Mapping)](./todo.md#-épico-2--mapeamento-de-dados-data-mapping) | 11 |

---

## 📊 Progresso geral

> Atualize manualmente esta tabela conforme as histórias forem concluídas.

| História | Épico | BACK | FRONT |
|----------|-------|------|-------|
| H1 · Edição de critérios de comunicação | Comunicações | ✅ | ⬜ |
| H2 · Inativação de comunicação | Comunicações | ✅ | — |
| H3 · Definição de comunicação padrão | Comunicações | ✅ | ⬜ |
| H4 · Priorização de critérios | Comunicações | ⬜ | ⬜ |
| H6 · Padronização de telas | Data Mapping | — | ✅ |
| H7 · Upload e configuração de Data Mapping | Data Mapping | ⬜ | ⬜ |
| H8 · Reutilização de configurações | Data Mapping | ⬜ | — |
| H9 · Marcação de campos importantes | Data Mapping | ✅ | ✅ |
| H10 · Validação de uso de campos | Data Mapping | ✅ | ✅ |
| H11 · Correção de visualização de máscaras | Data Mapping | — | ✅ |
| H12 · Criação de campos derivados | Data Mapping | ✅ | ✅ |
| H13 · Regras para uso de campos base | Data Mapping | ✅ | ✅ |
| H14 · Ajustes de API | Data Mapping | ⬜ | — |
| H15 · Exibição de erro ao layout sem sessões | Comunicações | ⬜ | ⬜ |
| H16 · Atualização do content-type FieldMapping | Data Mapping | — | ✅ |

> **Legenda:** ✅ Concluído · ⬜ Pendente · — Não se aplica
