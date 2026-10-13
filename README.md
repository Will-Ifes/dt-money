# DT Money · transações

Interface para registrar entradas e saídas, pesquisar transações e acompanhar saldo.

## Contexto e objetivo

Projeto de estudo da trilha Ignite da Rocketseat: React, TypeScript, context selectors, Axios, React Hook Form, Zod, Radix e styled-components.

## Funcionalidades presentes

- Consulta e criação de transações.
- Pesquisa textual com ordenação por data.
- Resumo de entradas, saídas e saldo.
- Formulário em modal.

## Por dentro do código

| Código | O que observar |
| --- | --- |
| [`src/contexts/TransactionsContext.tsx`](src/contexts/TransactionsContext.tsx) | API e estado. |
| [`src/hooks/useSummary.ts`](src/hooks/useSummary.ts) | Cálculo do resumo. |
| [`src/components/NewTransactionMondal/index.tsx`](src/components/NewTransactionMondal/index.tsx) | Formulário. |
| [`src/lib/axios.ts`](src/lib/axios.ts) | Configuração da API. |

## Executar localmente

Requer Node.js e npm compatíveis com as dependências versionadas.

```bash
git clone https://github.com/Will-Ifes/dt-money.git
cd dt-money
npm install
npm run dev
```

Abra o endereço informado pelo servidor no terminal.

Em outro terminal, execute `npm run dev:server`. A API de demonstração usa JSON Server na porta 3333 e os registros de `server.json`.

## Comandos disponíveis

| Comando | Script versionado |
| --- | --- |
| `npm run dev` | `vite` |
| `npm run dev:server` | `npx json-server server.json -p 3333 -w -d 500` |
| `npm run lint` | `eslint src --ext .tsx,.ts` |
| `npm run lint:fix` | `eslint src --ext .tsx,.ts --fix` |
| `npm run build` | `tsc && vite build` |
| `npm run preview` | `vite preview` |

Os comandos refletem o `package.json`. A existência de um script não comprova execução bem-sucedida no ambiente atual.

## Escopo e evolução

A API é uma simulação local, sem autenticação ou infraestrutura financeira. Tratamento de falhas e testes de cálculo são evoluções possíveis.

---

Mantido por **Will Oliveira** · [Perfil](https://github.com/Will-Ifes) · [LinkedIn](https://www.linkedin.com/in/wildemberg-de-jesus-oliveira/)
