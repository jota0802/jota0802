<h1>João Franco</h1>

**Software Engineer · Front-end Developer**

Engenheiro de software na **Guardline**, no front-end de uma plataforma de onboarding digital e
verificação de identidade (KYC/KYB): jornadas de captura de documento e biometria, design system e
back-office de análise de casos. Svelte e TypeScript no front, e Go quando a mudança precisa das duas
pontas. Fora do horário, gosto de sistemas em que a regra sensível mora no banco — RPC transacional,
Row Level Security e trigger — e não na interface.

<div>
  <a href="https://www.linkedin.com/in/jo%C3%A3o-franco" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-000000?style=flat&logo=linkedin&logoColor=white" alt="Perfil no LinkedIn"></a>
  <a href="mailto:jvfranco08@gmail.com"><img src="https://img.shields.io/badge/E--mail-000000?style=flat&logo=gmail&logoColor=EA4335" alt="Enviar e-mail"></a>
  <a href="https://joaof-dev-showcase.netlify.app" target="_blank"><img src="https://img.shields.io/badge/Portf%C3%B3lio-000000?style=flat&logo=netlify&logoColor=00C7B7" alt="Portfólio online"></a>
</div>

---

## Projetos

**[The Fate](https://github.com/jota0802/The-Fate)** · *privado* — Plataforma de estudo gamificada:
o professor monta planos com jornadas e tasks, o aluno progride com verificação por checkbox,
screenshot ou pergunta autocorrigida, em turmas com código de matrícula.
A verificação não vive no front: é uma fronteira de confiança no banco, com RPCs `SECURITY DEFINER`
de `search_path` fixo, a resposta correta negada por GRANT de coluna e trigger role-aware que
congela o gabarito contra o aluno sem travar a autoria do professor.
`Next.js 16` `React 19` `TypeScript` `Supabase/RLS` `plpgsql` `Tailwind 4`

**[Clif Arena](https://clifarena-web.vercel.app)** · *no ar, repo privado* — Gestão de arena
esportiva multi-tenant: modalidades, quadras, agendas, inscrições, lista de espera, check-in e
mensalidades, com API e front deployados de forma independente. Projeto em parceria com outro
desenvolvedor. Endureci o isolamento por clube carimbando o `clubeId` também no SET do update, não
só no WHERE, e uma revisão adversarial minha fechou dois P0 de autenticação.
`NestJS 10` `Prisma 6` `PostgreSQL` `JWT + Google OAuth` `Stripe` `Next.js 14`

**[Valida Biometria](https://validabiometria.com.br)** · *no ar, repo privado* — Validação de
identidade por biometria facial para PMEs: match facial, prova de vida, OCR e validação de
documento. Entrei como segundo desenvolvedor, responsável pelo front-end e pelo design system — o
núcleo biométrico e a infraestrutura são de autoria de outro desenvolvedor. Fiz o componente de
gráficos do back-office e destravei a captura no mobile trocando o preview 4K por 1080p e removendo
o `backdrop-filter: blur` sobre o vídeo, que derrubava o FPS.
`Angular 20 (signals)` `TypeScript` `SCSS` `Docker`

**Site de análise esportiva com bolão** · *privado, para um criador de conteúdo* — Vitrine de vídeos,
palpites de placar que viram pontos, ranking, painel administrativo e PWA instalável. Duas coisas
feitas na mão: a pontuação virou uma função `plpgsql` all-or-nothing com lock pessimista da linha do
jogo, no lugar de um loop de updates na aplicação que deixava ranking meio-pontuado em caso de
timeout; e o chaveamento de mata-mata desenha os conectores como paths SVG medidos por refs, com
`ResizeObserver`, em vez de biblioteca.
`Next.js 15` `Server Actions` `Supabase/RLS` `plpgsql` `Vitest` `Playwright`

**[Cantina FIAP](https://github.com/jota0802/fiap-mdi-cp2-cantina-app)** · *público* — Monorepo
cliente-servidor de pedidos: API REST com autenticação própria e app Expo com cache offline e QR
code de retirada. O contrato não vive em dois lugares — `packages/shared` exporta os schemas Zod
usados tanto na validação das rotas quanto na tipagem do app, com typecheck strict nos três
workspaces.
`pnpm workspaces` `Hono 4` `Drizzle` `Zod` `Expo 54` `React Native 0.81`

**[Smart Gym](https://github.com/jota0802/SmartGym)** · *público* — Estação de treino que identifica
o aluno por cartão RFID lido em Arduino, conta as repetições do exercício por visão computacional e
grava cada sessão em banco local.
`Python` `MediaPipe Pose` `OpenCV` `SQLite` `Arduino/UART`

Também: [Luz da Fé](https://velasluzdafe.com.br) (loja de velas, Next 16 estático),
[JotaTrack](https://github.com/jota0802/JotaTrack) (app nativo de macOS de tempo de uso, Swift +
SwiftUI) e um sistema de rastreamento de maletas com mapa e aprovação de transferência
(React 19 + Supabase, repositório do cliente).

---

## Tecnologias

#### Linguagens e core
![TypeScript](https://img.shields.io/badge/TypeScript-000000?style=flat&logo=typescript&logoColor=3178C6)
![JavaScript](https://img.shields.io/badge/JavaScript-000000?style=flat&logo=javascript&logoColor=F7DF1E)
![Go](https://img.shields.io/badge/Go-000000?style=flat&logo=go&logoColor=00ADD8)
![Python](https://img.shields.io/badge/Python-000000?style=flat&logo=python&logoColor=3776AB)
![Swift](https://img.shields.io/badge/Swift-000000?style=flat&logo=swift&logoColor=F05138)
![Node.js](https://img.shields.io/badge/Node.js-000000?style=flat&logo=nodedotjs&logoColor=339933)
![HTML5](https://img.shields.io/badge/HTML5-000000?style=flat&logo=html5&logoColor=E34F26)
![CSS](https://img.shields.io/badge/CSS-000000?style=flat&logo=css&logoColor=1572B6)
![Sass](https://img.shields.io/badge/Sass-000000?style=flat&logo=sass&logoColor=CC6699)

#### Frameworks e bibliotecas
![Svelte](https://img.shields.io/badge/Svelte-000000?style=flat&logo=svelte&logoColor=FF3E00)
![React](https://img.shields.io/badge/React-000000?style=flat&logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-000000?style=flat&logo=angular&logoColor=DD0031)
![React Native](https://img.shields.io/badge/React%20Native-000000?style=flat&logo=expo&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-000000?style=flat&logo=nestjs&logoColor=E0234E)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-000000?style=flat&logo=tailwindcss&logoColor=06B6D4)

#### Dados e back-end
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-000000?style=flat&logo=postgresql&logoColor=4169E1)
![Supabase](https://img.shields.io/badge/Supabase-000000?style=flat&logo=supabase&logoColor=3FCF8E)
![Prisma](https://img.shields.io/badge/Prisma-000000?style=flat&logo=prisma&logoColor=5A67D8)
![Drizzle](https://img.shields.io/badge/Drizzle-000000?style=flat&logo=drizzle&logoColor=C5F74F)
![Docker](https://img.shields.io/badge/Docker-000000?style=flat&logo=docker&logoColor=2496ED)

#### Testes e ferramentas
![Vitest](https://img.shields.io/badge/Vitest-000000?style=flat&logo=vitest&logoColor=6E9F18)
![Playwright](https://img.shields.io/badge/Playwright-000000?style=flat&logo=playwright&logoColor=2EAD33)
![Git](https://img.shields.io/badge/Git-000000?style=flat&logo=git&logoColor=F05032)
![Vite](https://img.shields.io/badge/Vite-000000?style=flat&logo=vite&logoColor=646CFF)
![Figma](https://img.shields.io/badge/Figma-000000?style=flat&logo=figma&logoColor=F24E1E)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-000000?style=flat&logo=netlify&logoColor=00C7B7)
![Claude](https://img.shields.io/badge/Claude-000000?style=flat&logo=anthropic&logoColor=white)

---

## GitHub em números

<div>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=jota0802&show_icons=true&include_all_commits=true&hide_border=true&bg_color=00000000&title_color=E5E5E5&text_color=A3A3A3&icon_color=FFFFFF&ring_color=79C0FF">
    <img src="https://github-readme-stats.vercel.app/api?username=jota0802&show_icons=true&include_all_commits=true&hide_border=true&bg_color=00000000&title_color=1F2328&text_color=59636E&icon_color=0969DA&ring_color=0969DA" width="420" height="165" alt="Estatísticas do GitHub de jota0802: estrelas, commits, pull requests, issues e contribuições">
  </picture>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs?username=jota0802&layout=compact&langs_count=6&hide_border=true&bg_color=00000000&title_color=E5E5E5&text_color=A3A3A3">
    <img src="https://github-readme-stats.vercel.app/api/top-langs?username=jota0802&layout=compact&langs_count=6&hide_border=true&bg_color=00000000&title_color=1F2328&text_color=59636E" width="320" height="165" alt="Linguagens mais usadas nos repositórios de jota0802">
  </picture>
</div>
