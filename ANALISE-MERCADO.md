# Análise de mercado e plano de evolução do perfil

**Data:** agosto/2026 · **Base:** vagas ativas no Indeed (Porto Alegre/RS e remoto Brasil), perfil público do GitHub e currículo do Indeed.

> **Revisão 2.** A primeira versão deste documento partiu do pressuposto — tirado do README —
> de que a frente de desenvolvimento no Silveiro era trabalho de dados (Oracle → Power BI).
> Não é: o dia a dia é **desenvolvimento de interfaces em Laravel com Filament**, e a parte
> de dados foi pontual e já encerrada. A recomendação de trilha mudou por causa disso.

Este documento não é uma lista de "aprenda mais coisas". É um diagnóstico do que o mercado
de fato pede para as vagas que você consegue disputar **hoje**, onde seu perfil já bate,
onde ele perde pontos, e em que ordem mexer nisso.

---

## 1. Metodologia

Foram lidas as descrições completas de dez vagas ativas em quatro recortes:

| Recorte | Vagas analisadas |
|---|---|
| **Web/PHP presencial RS** | Ecoplan Engenharia, Programador Web Moinhos de Vento (HuntWare) |
| **Web/fullstack remoto BR** | Hurb (Full Stack), Letras (Talentos em Tecnologia) |
| Dev júnior Python | Grupo AFL (São Leopoldo), Radix (remoto) |
| Dados júnior | Grupo Panvel, Aliare, MJV Innovation |
| Estágio TI POA (linha de base) | METTA — R$ 1.200 + VT + VR, 5h30/dia |

---

## 2. O que o mercado pede

| Requisito | Aparece em | Você tem? |
|---|---|---|
| **PHP** | 4 das 4 vagas web | ✅ é o seu dia a dia |
| **Laravel** | 2 de 2 vagas web de POA, nominalmente | ✅ **é o seu ativo mais forte** |
| **SQL / banco relacional** | praticamente todas | ✅ Oracle SQL |
| **API REST (criar e consumir)** | Ecoplan, Hurb, Letras, AFL, Radix | 🟡 tem no NeuroDrive (Flask), não em Laravel visível |
| **Git / Gitflow** | HuntWare, Hurb, AFL, Radix | ✅ mas sem histórico público que comprove |
| **Testes unitários e de integração** | Hurb (explícito), AFL, Radix | ❌ **lacuna clara** |
| **Cloud (AWS/Azure/GCP)** | 5 de 10 | ❌ **nenhuma menção** |
| **Docker** | Hurb, AFL, Aliare | ✅ já usa |
| **Front-end JS (React/Vue/Angular)** | Hurb, Letras, AFL, Radix | ❌ Filament/Livewire cobre seu caso, não as vagas deles |
| **Bootstrap / jQuery** | HuntWare | ❓ não declarado |
| **SOLID, clean architecture, design patterns** | Hurb | ❓ não declarado |
| **Integração com modelos de IA** | Ecoplan, Panvel, Dot Digital (RAG), vaga agentic remota | ✅ **tem, mas tirou do perfil** |
| **Python** | AFL, Radix, Ecoplan, Aliare, Panvel, MJV | ✅ NeuroDrive + automação |
| Power BI / pandas | Panvel, MJV | 🟡 experiência pontual, encerrada |
| Inglês | vagas remotas melhores | ❓ não declarado |

### Leitura dos dados

1. **Laravel é a sua carta mais forte e ela está escondida.** As duas vagas de PHP de Porto
   Alegre pedem Laravel pelo nome. Seu README, até agora, não citava PHP uma única vez.
   Isso é o oposto de um problema de qualificação: é qualificação jogada fora.
2. **Filament é um diferencial real, mas não é palavra-chave.** Nenhuma vaga do recorte
   escreve "Filament". Então ele não pode ser a manchete — a manchete é **Laravel**, e o
   Filament entra como a especialização que explica *o que* você constrói (painéis
   administrativos, CRUD complexo, RBAC) e *quão rápido*. Em entrevista, ele é ótimo
   assunto; num filtro de recrutador, ele é invisível. Os dois precisam aparecer, nessa ordem.
3. **Você tem a trinca rara que a Ecoplan pede: PHP + Python + IA.** Laravel (trabalho),
   Python (NeuroDrive, automação) e integração com LLM (Gemini API). Junior que marca as três
   é incomum. Só que a evidência da terceira saiu do perfil junto com o bot.
4. **Cloud e testes seguem sendo as duas lacunas caras**, agora com um agravante: a Hurb pede
   testes unitários *e* de integração no corpo dos requisitos, não como diferencial.
5. **Front-end JS deixou de ser "descartável" e virou uma escolha consciente.** Filament e
   Livewire resolvem interface reativa sem React — legítimo, e é assim que você trabalha.
   Mas as vagas remotas boas (Hurb, Letras, AFL, Radix) pedem React/Angular. React é o
   desbloqueador, não uma obrigação imediata.

---

## 3. Diagnóstico do perfil

### Forças reais

- **Experiência remunerada em Laravel enquanto ainda está na graduação.** Isso já responde ao
  requisito principal das duas vagas de PHP de POA. Muita gente do seu nível só tem projeto
  de faculdade.
- **Filament/TALL stack**: você entrega painel administrativo funcionando rápido. Para empresa
  pequena ou consultoria, isso é exatamente o perfil que resolve problema.
- **NeuroDrive é forte e premiado** (3º lugar, A Jornada UniRitter 2026). Prova Python real,
  não só "fiz um curso".
- **Segurança/IAM/LGPD em escritório de advocacia**: dado sensível, controle de acesso e
  compliance. Raríssimo em júnior, e casa com quem constrói painel administrativo — quem já
  fez IAM entende permissionamento antes de precisar apanhar.
- **Python + PHP na mesma pessoa.** Metade das vagas do recorte cita uma ou outra; a Ecoplan
  cita as duas.

### Já corrigido no README

- ~~Título ancorado em "Estagiário de TI"~~ → agora abre pela stack de desenvolvimento.
- ~~Certificações não técnicas~~ → removidas (viravam ruído).
- ~~Datas inconsistentes~~ → padronizado em dez/2025.
- ~~"InfoJobs Bot" listado sem repositório~~ → removido. **Ver ressalva abaixo.**

### Ainda em aberto

1. **A saída do bot custou mais caro do que parecia.** Ele era a sua única evidência pública
   de "integração com modelos de IA" — requisito citado pela Ecoplan, pela Panvel e pelas
   vagas de RAG/agentes. Sem ele, o portfólio também caiu para **um projeto só**. Publicar o
   repositório (ou construir uma integração LLM pequena dentro de um app Laravel) recupera as
   duas coisas de uma vez.
2. **Zero código Laravel público.** Você é avaliado exatamente naquilo que não dá para ver.
   É o buraco número um do perfil hoje.
3. **Sem testes, sem cloud.** As duas lacunas transversais a todas as trilhas.
4. **Front-end declarado como "HTML/CSS/JS"**, que é ao mesmo tempo vago e subestimado — não
   diz nem que você trabalha com Tailwind/Livewire via Filament, nem marca React.
5. **Sem versão em inglês.** Fecha as vagas remotas mais bem pagas antes da conversa.
6. **Sem números.** "80+ usuários" você já tem. Faltam: quantos painéis/telas entregues,
   quantos módulos, quantos processos automatizados.

---

## 4. Escolha de trilha

| Trilha | Aderência atual | Volume de vagas | Veredito |
|---|---|---|---|
| **Dev Web PHP/Laravel (full-stack)** | alta — é o trabalho remunerado que você faz hoje | alto em POA, presencial | ✅ **principal** |
| **Back-end Python (API)** | média-alta — Flask do NeuroDrive é a ponte | alto, muito remoto | ✅ **secundária** |
| Full-stack com React/Vue | baixa hoje | alto e melhor pago no remoto | 🎯 **alvo de 6–12 meses** |
| Dados / BI | baixa — experiência pontual e encerrada | alto | 🔻 vira **linha de currículo**, não trilha |
| Suporte / Segurança / Infra | alta na prática, baixa no portfólio | médio, teto menor | 🔻 vira **diferencial**, não manchete |

**Recomendação:** consolidar em **PHP/Laravel**, com **Python** como segunda linguagem
declarada. É a única leitura em que o trabalho que você faz hoje, seu projeto premiado e as
vagas abertas apontam para o mesmo lugar. As duas compartilham quase tudo do que falta
estudar (API REST, testes, Docker, cloud), então nenhum esforço é jogado fora.

Segurança/LGPD deixa de ser trilha e vira sua história de diferenciação: *"construo painel
administrativo em ambiente com dado sensível e sei por que cada permissão existe"*.

---

## 5. Plano de 90 dias

### Semanas 1–2 — Arrumar a vitrine (custo ~zero)
- [x] Reposicionar o título do README para a trilha real. **Falta replicar no LinkedIn e no Indeed** — seu currículo do Indeed ainda diz "Python, PHP, Selenium" sem citar Laravel.
- [x] Tirar as certificações não técnicas.
- [x] Padronizar a data de início (dez/2025).
- [x] Colocar PHP, Laravel e Filament na stack, com a frente de desenvolvimento em primeiro lugar.
- [ ] Conferir se `neurodrive` está **público**, com README próprio: problema, GIF do dashboard, como rodar em 3 comandos, e o 3º lugar.
- [ ] Fixar (pin) os repositórios certos no perfil do GitHub.
- [ ] Decidir o destino do bot de candidatura: publicar o repositório recupera a evidência de IA.

### Semanas 3–6 — Um projeto Laravel público (a prioridade máxima)
- [ ] **Projeto-âncora: app Laravel + Filament público.** Escolha um domínio simples e real
      (controle de chamados, gestão de contratos, agenda de prazos). O que ele precisa ter,
      porque é isso que as vagas pedem:
      - painel Filament com CRUD, filtros e **controle de permissões por papel** (usa sua vivência de IAM);
      - **uma API REST** exposta com autenticação via Sanctum — marca o requisito da Ecoplan, da Hurb e da Letras;
      - **testes com Pest/PHPUnit**, mesmo que sejam 15 — marca o requisito explícito da Hurb;
      - `docker-compose` para subir em um comando;
      - README com print do painel e o problema que resolve.
      Esse único projeto marca de uma vez: PHP, Laravel, SQL, API REST, testes, Docker e Git.
- [ ] Bônus alto retorno: uma tela do app que chame um LLM (resumo, classificação, extração
      de texto de documento). Fecha o requisito de IA da Ecoplan **dentro** do projeto Laravel.

### Semanas 7–12 — Fechar as lacunas transversais
- [ ] **AZ-900** (Azure Fundamentals) ou **AWS Cloud Practitioner** — resolve o requisito que
      aparece em 5 de 10 vagas, e é barato e rápido.
- [ ] Deploy do projeto-âncora em nuvem, com o link no README. Vale mais que o certificado.
- [ ] Estudar **SOLID e design patterns** aplicados a Laravel (service classes, repositories,
      form requests). É requisito literal da Hurb e assunto garantido de entrevista.
- [ ] Só depois disso, **React** — é o que destrava as vagas remotas melhores. Antes disso, não.

### Contínuo
- [ ] Inglês técnico, leitura e escrita.
- [ ] Números em tudo: painéis entregues, módulos, usuários atendidos, processos automatizados.

---

## 6. O que mexer no perfil, por ordem de impacto

| # | Ação | Esforço | Impacto |
|---|---|---|---|
| ✅ | Título/posicionamento pela stack real (PHP/Laravel + Python) | feito | 🔥🔥🔥 |
| ✅ | PHP, Laravel e Filament na stack; frente de dev em primeiro lugar | feito | 🔥🔥🔥 |
| ✅ | Certificações não técnicas fora; datas padronizadas | feito | 🔥🔥 |
| 1 | Replicar o posicionamento no LinkedIn **e no Indeed** (que ainda não cita Laravel) | 30 min | 🔥🔥🔥 |
| 2 | Projeto Laravel + Filament público com API, testes e Docker | 3–4 semanas | 🔥🔥🔥 |
| 3 | Recuperar a evidência de IA (publicar o bot ou integrar LLM no projeto) | 1 dia – 1 semana | 🔥🔥 |
| 4 | Quantificar as entregas do trabalho atual | 30 min | 🔥🔥 |
| 5 | Certificação cloud (AZ-900) + deploy do projeto | 3–4 semanas | 🔥🔥 |
| 6 | SOLID / design patterns em Laravel | contínuo | 🔥🔥 |
| 7 | Versão em inglês do README | 1h | 🔥 |
| 8 | React | 2–3 meses | 🔥🔥 (destrava o remoto) |

---

## 7. Vagas do recorte, por aderência

1. [DESENVOLVEDOR DE SISTEMAS — Ecoplan Engenharia](https://to.indeed.com/aamdg2pctc7h)
   — **a vaga mais aderente do levantamento inteiro.** Pede Laravel, APIs REST, PHP **e**
   Python, e cita integração com modelos de IA como desejável. É literalmente a sua trinca.
   Não exige tempo de experiência no texto. Porto Alegre, presencial.
   ⚠️ Contrato **PJ** — sem CLT, sem 13º, sem férias; a faixa precisa compensar isso, e
   avalie a compatibilidade com o estágio e a faculdade.
2. [PROGRAMADOR WEB — Moinhos de Vento (HuntWare)](https://to.indeed.com/aahn6njzrpyh)
   — Laravel, PHP, MVC, SQL, Git, Bootstrap e jQuery. Stack quase idêntica à sua; a barreira é
   o "~3 anos de experiência" e o ensino superior completo. Vale candidatar mesmo assim: em
   vaga marcada como urgente, stack certa costuma valer mais que o tempo pedido.
   ⚠️ Também **PJ e presencial**.
3. [Talentos em Tecnologia — Letras](https://to.indeed.com/aa44222hsj4h)
   — banco de talentos **remoto que aceita estágio e júnior**, com PHP, Python, SQL e API no
   time de back-end. Custo de candidatura é quase zero e o retorno é assimétrico. Faça hoje.
4. [TI | Desenvolvedor(a) Full Stack — Hurb](https://to.indeed.com/aaxh28zjyw4f)
   — remoto, aceita PHP e abre para júnior. Gaps: ReactJS, testes unitários/integração e
   SOLID/clean architecture. É o alvo natural depois do projeto-âncora.
5. [Desenvolvedor Junior — Grupo AFL](https://to.indeed.com/aafnbsgyw9vr)
   — São Leopoldo, Python + Next.js, 1–3 anos. Entra no radar quando o tempo de casa fechar
   1 ano e o front moderno sair do zero.
6. [Profissional Desenvolvedor de Software Júnior — Radix](https://to.indeed.com/aa664rsq69w4)
   — remoto, exige Python **básico**, Git e noções de API. A barreira é Angular.

Referência de piso local: [ESTÁGIO - TI (METTA)](https://to.indeed.com/aaxkxdnvytpr) paga
R$ 1.200 por 5h30/dia para suporte e "projetos de automação". Você faz Laravel — está bem
acima disso. Use como argumento na próxima negociação, não como alvo.

---

## 8. Resumo em três frases

Seu problema nunca foi qualificação: era o perfil descrever a pessoa errada — você entrega
Laravel e o README falava de suporte e de dados. Corrigido o posicionamento, o buraco que
sobra é **evidência**: nenhuma linha de PHP pública, nenhum teste, nenhuma cloud. Um único
app Laravel + Filament no ar, com API, testes e Docker, resolve simultaneamente a maior parte
dos requisitos das vagas que você quer — e a mais aderente delas, a da Ecoplan, já está aberta.
