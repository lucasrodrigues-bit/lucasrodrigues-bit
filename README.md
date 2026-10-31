<h1 align="center">Lucas Deiró Rodrigues</h1>

<p align="center">
  🚀 <b>Desenvolvedor Full Stack</b> · 📚 Ciência da Computação (UNIT) · 📍 Aracaju - SE<br>
  <i>Foco em sistemas com alta integridade, arquitetura limpa e software em produção real.</i>
</p>

<p align="center">
  <a href="https://linkedin.com/in/lucas-deiró-rodrigues-b6176137b">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:lucasdeiror@gmail.com">
    <img src="https://img.shields.io/badge/Email-lucasdeiror%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

---

## 🧠 Sobre mim

Construo software voltado para o mundo real, com foco obsessivo em **estabilidade operacional, integridade e regras de negócio sólidas**. Já mantenho um sistema proprietário em uso diário por uma operação de varejo e estou desenvolvendo a infraestrutura de um SaaS multi-tenant.

* 💼 **Estagiário de Suporte Técnico N1** no **Senac Sergipe**.
* 🎓 **Residência de Software (UNIT)**: Atuação prática em times ágeis multidisciplinares, liderança de front-end, versionamento rigoroso e entrega contínua.
* 🛠️ **Engenharia com Spec-Driven Development (SDD)**: Utilizo inteligência artificial de ponta no meu fluxo de trabalho não para terceirizar o raciocínio, mas como acelerador de execução estritamente guiado por especificações formais (`spec → design → tasks`), sempre auditando a arquitetura, segurança e integridade do código gerado.
* ☕ **Trilha Java & Fundamentos**: Aprofundo ativamente **Core Java (JDK 21/25)** e **Clean Architecture** (estruturas de dados, streams, generics, tratamento funcional de exceções e concorrência) antes de delegar abstrações para o ecossistema Spring Boot.

---

## 🛠️ Tecnologias & Competências

| Camada | Stack & Ferramentas |
| :--- | :--- |
| **Linguagens** | TypeScript, Java (JDK 21/25), JavaScript, SQL, Python |
| **Front-end** | React, Next.js (App Router), Vite, Tailwind CSS, shadcn/ui, Design Systems |
| **Back-end** | Node.js (Serverless & Fastify), Server Actions, REST APIs, Clean Architecture |
| **Bancos de Dados** | PostgreSQL (RLS, PL/pgSQL, Triggers, Constraints), Supabase, MySQL, Redis |
| **Testes & Qualidade** | Vitest, Playwright, pgTAP (testes no banco), PGlite, pytest |
| **DevOps & Métodos** | Git/GitHub (PRs, Code Review), Docker, Vercel, Linux, Spec-Driven Development |

---

## 📂 Projetos em Destaque

### 💎 Produção & Engenharia de Impacto

* **Gestão Gabi Modas** *(Proprietário · Em Produção Real)*
  Sistema completo de gestão comercial para varejo de moda, desenhado para operação ágil de balcão mobile e split-screen desktop.
  * **Engenharia & Concorrência:** Vendas atômicas protegidas por trava de concorrência (`comLock` transacional), impedindo que acessos simultâneos vendam a mesma peça.
  * **Finanças & Negócio:** Controle de fiado parcelado em até 12x com abatimento inteligente (FIFO), fluxo de caixa, controle de estoque por grade, etiquetas e relatórios em PDF/CSV.
  * **Segurança:** RBAC no servidor com verificação de papéis por requisição, sessão em cookies `httpOnly`, rate limiting e isolamento de schema (`loja`).
  * **Stack:** React 19, Vite, Tailwind v4, Node.js serverless na Vercel e PostgreSQL (Supabase).

* **Nexo — Sistema Operacional** *(Em Desenvolvimento)*
  SaaS multi-tenant focado em eliminar a ociosidade operacional e o capital morto em pequenos comércios (barbearias, varejo e petshops).
  * **Isolamento Rígido:** Multi-tenancy respaldado por políticas de Row Level Security (RLS) no PostgreSQL e RBAC granular.
  * **Tolerância a Falhas Comprovada:** Mutação de caixa e estoque blindada por funções atômicas em PL/pgSQL; viabilidade comprovada com **95 testes pgTAP**, teste de concorrência simultânea (20 vendas para 10 peças sem saldo negativo) e estresse com 300.000 transações.
  * **Arquitetura:** Modular Hexagonal Lite (domínio 100% desacoplado de frameworks e UI) com Next.js 16, React 19, Supabase e Vitest.

---

### 🎓 Experiência Acadêmica & Projetos de Residência

* **MarcaSE (Residência de Software I - UNIT)**: Sistema de agendamento e gestão para clínicas médicas com múltiplos perfis de acesso (médicos, financeiro, recepção, pacientes) e dashboards de métricas. Atuei como **líder técnico do time de front-end** (React, Next.js, TypeScript e Supabase).
* **Plataforma de ODR (Residência de Software II - UNIT)**: Engenharia de back-end para plataforma multi-tenant de Resolução Online de Disputas (ODR), construída com Node.js, Fastify, TypeScript, cache com Redis, autenticação JWT e orquestração de IA.
* **Mix-Software**: SaaS de agendamento com regras de integridade cronológica via constraints espaciais no PostgreSQL para prevenção de no-show e dupla reserva em nível de banco de dados.

---

### 🧪 Portfólio de Fundamentos & Core Java

* **[Dashboard de Localização e Clima](https://github.com/lucasrodrigues-bit/consumo-api-dashboard-localizacao)** *(Java Puro)*
  * Agregação e orquestração de múltiplas APIs REST públicas (clima, câmbio, feriados nacionais e geolocalização) a partir de CEP, IP ou cidade.
  * Implementado com `java.net.http.HttpClient` nativo do JDK, Gson e mapeamento em camadas (DTOs → Domain Models), com suporte a consultas paralelas assíncronas.
* **[Sistema de Estoque CLI](https://github.com/lucasrodrigues-bit/sistema-de-estoque)** *(Java 25 Puro)*
  * Aplicação de console para fixação rigorosa dos pilares de **Core Java**: *Collections Framework*, Generics, Streams API, Records, Optionals e hierarquia de exceções de domínio customizadas, estruturado sob os preceitos de Clean Architecture (camada `core` 100% isolada).
* **DealsBot** *(Python)*
  * Serviço assíncrono para monitoramento contínuo de promoções em e-commerces (RSS/APIs), filtragem por parâmetros de desconto, enriquecimento contextual via LLM e disparo automatizado de alertas via Telegram com APScheduler e Supabase.

---

## 🎯 Foco e Próximos Passos

* Aprofundamento no ecossistema **Java corporativo e Spring Boot** (Spring Data JPA, Spring Security, Flyway).
* Evolução da esteira de automação do Nexo até a validação comercial com os primeiros estabelecimentos parceiros.

---

## 📊 Estatísticas do GitHub

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=lucasrodrigues-bit&theme=tokyonight&starting_year=2025&cache_seconds=3600" alt="GitHub Streak" />
</p>
