<!-- .github/copilot-instructions.md -->

# Instruções do Copilot para ZzPowerTech

Mantenha as orientações objetivas e práticas. Foque no que um agente de IA precisa saber para ser produtivo neste repositório.

- Visão geral do projeto

  - Este repositório é um portfólio/coletânea de projetos com foco em web full-stack e IoT (ver `README.md`). Tecnologias citadas: Angular, Next.js, React (frontend); NestJS/Node.js/Express (backend); PostgreSQL/Supabase/Prisma; Docker.
  - Espere projetos mistos (apps web, scripts IoT, integrações com hardware). Nem todos os componentes podem existir ainda — descubra os arquivos antes de editar.

- Fluxos de trabalho do desenvolvedor (por onde começar)

  - Leia `README.md` para entender o escopo e os contatos do autor.
  - Para construir/rodar algo, busque por `package.json`, `Dockerfile` ou configs específicas do framework (`nest`, `angular.json`, `next.config.js`). Se não existir, pergunte qual componente deve ser criado.

- Padrões e convenções

  - Prefira mudanças pequenas e incrementais, com testes quando aplicável. No backend, priorize TypeScript e siga padrões do NestJS se houver projeto Nest.
  - Ao usar Postgres, utilize Prisma (mencionado no README). Procure `prisma/schema.prisma` antes de criar migrações.
  - Mantenha código de IoT separado de serviços web — use pastas como `iot/` ou `hardware/` ao adicionar scripts para dispositivos.

- Integrações e dependências externas

  - Integrações comuns: Supabase (auth+db), PostgreSQL, serviços Dockerizados, dispositivos Raspberry Pi/Arduino. Nunca versione segredos; use variáveis de ambiente.

- Ao editar arquivos

  - Faça uma busca no repositório para evitar duplicações. Aplique mudanças conservadoras e comente brevemente a intenção quando útil.
  - Ao criar novos serviços, inclua um README mínimo e scripts de inicialização no `package.json`.

- O que NÃO fazer

  - Não invente CI, credenciais de DB ou endpoints externos. Solicite detalhes de infraestrutura quando faltarem.
  - Não refatore subsistemas grandes sem testes e sem alinhamento prévio.

- Exemplos rápidos deste repo
  - `README.md`: contém a visão geral do autor/stack e deve ser preservado ao atualizar metadados.

Se algo estiver ambíguo ou faltar arquivo essencial para uma mudança segura, peça esclarecimentos ao dono do repositório antes de prosseguir.
