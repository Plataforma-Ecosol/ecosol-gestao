# Plataforma ES Niterói · Gestão (Scrum)

Este repositório guarda o backlog e as sprints da Plataforma ES Niterói. O quadro fica no GitHub Project **Plataforma ES Niterói (SCRUM)** da organização Plataforma-Ecosol. Ele substitui o quadro do Trello, que ficou só como histórico.

## Fluxo das issues

**Product Backlog** → **Sprint Backlog** → **Em Andamento** → **Code Review** → **Teste / QA** → **Concluído**

- O Product Backlog fica ordenado por prioridade. O que está no topo entra primeiro na próxima sprint.
- Na Sprint Planning, puxe issues do topo do backlog até ~15 a 20 pontos e preencha o campo **Sprint**.
- Cada pessoa trabalha em no máximo 2 issues "Em Andamento" ao mesmo tempo.
- Ao abrir o PR, escreva `Closes Plataforma-Ecosol/ecosol-gestao#N` na descrição. O PR aparece ligado à issue e ela vai para Code Review. No merge, a issue fecha e vai para Concluído.
- **Fora do escopo:** ideias que o PRD deixa fora do MVP (login público, autocadastro, localização de coletivo). Voltam ao backlog só se um Spike aprovar.
- **Informações do Projeto:** DoR, DoD, cerimônias, links e decisões ficam como issues abertas nessa coluna, com a etiqueta `Informações`.

## Sprints

As sprints são o campo de iteração **Sprint** do Project (2 semanas cada).

- Não é preciso renomear nem arquivar colunas. O histórico de cada sprint é um filtro: `sprint:"Sprint 1" status:Concluído`.
- A view **Sprint atual** usa o filtro `sprint:@current`.
- Ao fim da sprint, o que não foi concluído passa para a próxima: filtre `sprint:@previous -status:Concluído` e mude o campo Sprint em lote.
- Para criar novas sprints: Settings do Project › Sprint › Add iteration.

Calendário: MVP (22/07 a 21/09/2026), Sprint 1 (28/09 a 09/10), Sprint 2 (13/10 a 23/10), Sprint 3 (26/10 a 06/11), Sprints 4 a 6 (09/11 a 18/12). Feriados considerados: 12/10, 02/11 e 20/11.

## Padrão do título

`[Épico] Título · N pts`

O épico também fica no campo **Épico** e os pontos no campo **Pontos**, para filtrar e somar no quadro.

## Etiquetas

- `História de usuário` (verde)
- `Tarefa técnica` (azul)
- `Spike` (roxo): pesquisa ou decisão
- `Bug` (vermelho)
- `Bloqueado` (laranja): impedimento
- `Alta prioridade` (amarelo)

## Story points

Escala Fibonacci: 1, 2, 3, 5, 8. Issue com mais de 8 pontos deve ser quebrada.

## Repositórios

- Backend: https://github.com/Plataforma-Ecosol/ecosol-backend
- Frontend: https://github.com/Plataforma-Ecosol/ecosol-frontend
- Infra: https://github.com/Plataforma-Ecosol/ecosol-infra
