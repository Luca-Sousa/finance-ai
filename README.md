# 💰 Finance AI

Uma aplicação web de gestão financeira pessoal que oferece controle completo sobre receitas, gastos e investimentos através de uma interface moderna e intuitiva.

![Next.js](https://img.shields.io/badge/Next.js-14.2.16-black?style=for-the-badge&logo=next.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)
![Prisma](https://img.shields.io/badge/Prisma-5.21.1-2D3748?style=for-the-badge&logo=prisma)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Latest-316192?style=for-the-badge&logo=postgresql)

## Sobre o Projeto

O Finance AI é uma plataforma completa de gestão financeira que permite aos usuários monitorar suas finanças pessoais de forma organizada e visual. A aplicação oferece análises detalhadas dos gastos por categoria, acompanhamento de receitas e investimentos, além de gráficos interativos para melhor compreensão dos hábitos financeiros.

## ✨ Principais Recursos

### Dashboard Analítico
- Visão geral das finanças mensais com cards de resumo
- Gráficos de pizza para distribuição de gastos por categoria
- Análise de gastos por categoria com percentuais
- Histórico das últimas transações
- Filtros por período específico

### Gestão de Transações
- Sistema completo de CRUD para transações financeiras
- Categorização em: Moradia, Transporte, Alimentação, Entretenimento, Saúde, Utilidades, Salário, Educação e Outros
- Suporte a múltiplos métodos de pagamento: Cartão de Crédito/Débito, PIX, Transferência Bancária, Boleto e Dinheiro
- Classificação por tipo: Receitas, Gastos e Investimentos
- Interface de tabela com paginação e ordenação

### Sistema de Autenticação
- Login/cadastro integrado com Clerk
- Proteção de rotas e sessões seguras
- Interface de tema escuro
- Controle de acesso baseado em usuário

### Modelo Freemium
- **Plano Gratuito**: Limite de 10 transações por mês
- **Plano Premium**: Transações ilimitadas
- Integração com Stripe para processamento de pagamentos
- Sistema de webhooks para atualização automática de status

## 🛠️ Stack Tecnológica

**Frontend:**
- Next.js 14 (App Router)
- TypeScript
- Tailwind CSS
- Radix UI (componentes)
- React Hook Form + Zod
- Recharts (gráficos)
- Lucide React (ícones)

**Backend:**
- Next.js Server Actions
- Prisma ORM
- PostgreSQL
- Middleware de autenticação

**Serviços:**
- Clerk (autenticação)
- Stripe (pagamentos)
- Docker (desenvolvimento)

## 🎯 Arquitetura

O projeto utiliza a arquitetura App Router do Next.js 14, organizando as funcionalidades em:

- **Dashboard Principal** (`(home)`): Visualizações e análises financeiras
- **Transações** (`transactions`): CRUD completo de movimentações
- **Assinatura** (`subscription`): Gerenciamento de planos premium
- **API Routes**: Webhooks do Stripe e endpoints necessários
- **Componentes Reutilizáveis**: UI components baseados em Radix UI

O banco de dados é modelado com Prisma, utilizando PostgreSQL para persistência dos dados de transações e relacionamentos com usuários autenticados via Clerk.

---

**Desenvolvido por:** [Lucas Sousa](https://github.com/Luca-Sousa)
