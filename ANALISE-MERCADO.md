# Análise de mercado e plano de evolução do perfil

**Data:** agosto/2026 · **Base:** vagas ativas no Indeed (Porto Alegre/RS e remoto Brasil), perfil público do GitHub e currículo do Indeed.

Este documento não é uma lista de "aprenda mais coisas". É um diagnóstico do que o mercado
de fato pede para as vagas que você consegue disputar **hoje**, onde seu perfil já bate,
onde ele perde pontos, e em que ordem mexer nisso.

---

## 1. Metodologia

Foram lidas as descrições completas de vagas ativas em três recortes:

| Recorte | Exemplos analisados |
|---|---|
| Dev júnior presencial/híbrido RS | Desenvolvedor Júnior (Grupo AFL, São Leopoldo) |
| Dados júnior RS | Analista de Dados I – Auditoria (Grupo Panvel, Eldorado do Sul) |
| Dev/dados júnior remoto BR | Radix, Aliare (Eng. de Dados Jr), MJV (Power BI + Python) |
| Estágio TI POA | METTA (COD 46158) — R$ 1.200 + VT + VR, 5h30/dia |

O recorte de estágio serve de linha de base: é o que você já faz. O foco da análise é a
**próxima** vaga, não a atual.

---

## 2. O que o mercado pede (frequência nas vagas lidas)

| Requisito | Aparece em | Você tem? |
|---|---|---|
| **Python** | quase todas | ✅ sim, com uso real |
| **SQL / banco relacional** | 4 de 6 | ✅ Oracle SQL no trabalho |
| **Cloud (AWS ou Azure), mesmo básico** | 4 de 6 | ❌ **nenhuma menção** |
| **ETL / pipeline de dados** | 3 de 6 | 🟡 faz na prática, não nomeia |
| **Git / GitHub** | citado explicitamente + pressuposto | 🟡 tem, mas não aparece na stack |
| **Framework web Python (Flask/Django/FastAPI)** | 2 de 6 + implícito | 🟡 Flask no NeuroDrive, subvalorizado |
| **API REST (consumir e construir)** | 2 de 6 | 🟡 tem via NeuroDrive/SSE, não explicitado |
| **Front-end moderno (React/Next/Angular + TS)** | 2 de 6 + 3 vagas fullstack/front | ❌ só HTML/CSS/JS |
| **Docker** | 2 de 6 (diferencial) | ✅ já usa |
| **Testes automatizados** | 2 de 6 | ❌ **lacuna clara** |
| **Power BI + DAX/Power Query (M)** | 2 de 6 | 🟡 usa Power BI, não cita DAX/M |
| **IA aplicada (RAG, agentes, LLM em processo)** | tendência forte em 2026 | 🟡 usou Gemini API, mas sem código público |
| **Inglês** | vagas remotas melhores exigem leitura/escrita | ❓ não declarado |

### Leitura dos dados

1. **Python + SQL é o seu ativo mais líquido.** As duas trilhas de maior volume (dados e
   back-end) partem exatamente daí. Você não precisa mudar de linguagem, precisa de
   profundidade demonstrável.
2. **Cloud é a lacuna mais cara.** É o único requisito frequente em que você tem zero
   sinal. Aparece em vaga de dev (AWS Lambda/RDS/ECS), de engenharia de dados (Azure,
   Databricks) e de BI (AWS/Azure). Custa pouco resolver no nível "fundamentos".
3. **Testes automatizados são a segunda lacuna.** Aparecem sempre como "diferencial",
   mas na prática é o que separa quem passa no teste técnico de júnior de quem não passa.
4. **Front-end moderno é o divisor entre as trilhas.** Se você não vai investir em
   React/Angular + TypeScript, aceite que vagas fullstack e front-end saem da sua lista —
   e pare de gastar espaço do perfil sinalizando web genérica.

---

## 3. Diagnóstico do perfil atual

### Forças reais (subaproveitadas)

- **Experiência remunerada em duas frentes** enquanto ainda está na graduação. Muita gente
  do seu nível compete só com projeto de faculdade.
- **NeuroDrive é um projeto forte e premiado** (3º lugar, A Jornada UniRitter 2026). Visão
  computacional + Flask + tempo real é acima da média do portfólio júnior típico.
- **Migração Oracle SQL → Power BI com pandas** é literalmente a descrição de meia dúzia de
  vagas de dados júnior. Hoje isso está no README como um bullet de 1 linha.
- **Segurança/IAM/LGPD em escritório de advocacia** é um diferencial de nicho: dado
  sensível, compliance, controle de acesso. Vale ouro em vaga de dados em jurídico, saúde
  ou financeiro — e é raríssimo em júnior.

### Onde o perfil perde pontos

#### Já corrigido no README

1. ~~**Posicionamento diluído.**~~ O título abria com "Estagiário de TI", ancorando a
   percepção no help desk — o teto salarial mais baixo entre tudo que você faz. Agora abre
   como dev Python/Dados. **Falta replicar no LinkedIn**, que é onde o recrutador olha primeiro.
2. ~~**Projeto sem link.**~~ O "InfoJobs Bot" estava listado sem repositório; foi removido.
3. ~~**Certificações desequilibradas.**~~ As três não técnicas (Atendimento ao Cliente,
   Assistentes Administrativos, Outlook na Web) saíram — viravam ruído em vaga de dados e
   reforçavam a leitura "perfil administrativo".
4. ~~**Inconsistência de datas.**~~ Padronizado em dez/2025 na experiência, coerente com o
   "desde 2025" do texto e com o currículo do Indeed.

#### Ainda em aberto

5. **Portfólio de um projeto só.** Com a saída do bot, sobra o NeuroDrive — que é forte, mas
   é um projeto acadêmico de visão computacional, não o formato que vaga de dados avalia
   (pipeline reproduzível: entrada, transformação, saída, teste). **Isso torna o
   projeto-âncora da seção 5 a prioridade número um do portfólio, não mais um "extra".**
6. **Só duas certificações, ambas introdutórias.** Com o corte, restaram a de IA (UniRitter,
   160h) e a de Análise de Dados (LinkedIn Learning). A tabela ficou honesta, mas curta —
   razão a mais para o AZ-900 e o PL-300 saírem do papel: são as duas que o mercado
   reconhece de verdade.
7. **Zero sinal de teste, cloud e API pública.** Três das quatro coisas mais pedidas.
8. **Sem versão em inglês.** Fecha a porta das vagas remotas mais bem pagas antes da
   primeira conversa.

---

## 4. Escolha de trilha

Você hoje sinaliza três coisas ao mesmo tempo: suporte/infra, segurança e dados. Perfil
júnior que sinaliza três trilhas é lido como não tendo nenhuma.

| Trilha | Aderência atual | Volume de vagas | Veredito |
|---|---|---|---|
| **Dados / Analytics Engineer** | alta — é o que você já faz e o que os projetos suportam | alto | ✅ **principal** |
| **Back-end Python (API)** | média-alta — Flask do NeuroDrive é a ponte | alto | ✅ **secundária** (mesmo portfólio serve) |
| Suporte / Segurança / Infra | alta na prática, baixa no portfólio | médio, teto menor | 🔻 vira **diferencial**, não manchete |
| Fullstack / Front-end | baixa | alto | ❌ descartar por ora |

**Recomendação:** consolidar em **Python para dados**, com back-end Python como trilha
adjacente. É a única combinação em que sua experiência atual, seu projeto premiado e as
vagas abertas apontam para o mesmo lugar — e as duas compartilham 80% do que você precisa
estudar (SQL, API, Docker, testes, cloud). Segurança/LGPD deixa de ser trilha e passa a ser
sua história de diferenciação: *"faço dados em ambiente com dado sensível e sei por quê"*.

---

## 5. Plano de 90 dias

Ordenado por retorno sobre esforço, não por dificuldade.

### Semanas 1–2 — Arrumar a vitrine (custo ~zero, retorno imediato)
- [x] Reposicionar o título do README para a trilha escolhida. **Falta o LinkedIn.**
- [x] Bot removido do README (estava sem link). Se um dia publicar o repositório, ele volta.
- [ ] Conferir se `neurodrive` está **público** e com README próprio contendo: problema,
      GIF/print do dashboard rodando, como executar em 3 comandos, e o resultado (o 3º lugar).
- [x] Certificações não técnicas removidas.
- [x] Data de início padronizada em dez/2025. **Confira se o LinkedIn e o Indeed batem.**
- [ ] Fixar (pin) os repositórios certos no perfil do GitHub.

### Semanas 3–6 — Fechar a lacuna de cloud e testes
- [ ] **AZ-900** (Azure Fundamentals) ou **AWS Cloud Practitioner**. É barato, é rápido, e
      resolve o requisito que aparece em 4 de 6 vagas. Azure tem leve vantagem: casa com
      Power BI, Databricks e com o ecossistema Microsoft dos clientes daqui.
- [ ] **pytest** no NeuroDrive: mesmo 10 testes cobrindo o cálculo de velocidade já muda a
      conversa numa entrevista. Adicionar badge de CI (GitHub Actions) no repositório.

### Semanas 7–12 — Um projeto que fale a língua das vagas
- [ ] **Projeto-âncora: pipeline de dados end-to-end.** Fonte pública (dados abertos de
      Porto Alegre, ANP, Receita Federal) → extração em Python → tratamento com pandas →
      carga em PostgreSQL → dashboard (Power BI ou Streamlit) → tudo em Docker Compose →
      agendamento → testes → README com o gráfico de resultado. Esse único projeto marca
      simultaneamente: Python, SQL, ETL, Docker, testes e visualização.
- [ ] **PL-300** (Power BI Data Analyst) se a trilha de dados se confirmar — foi citada
      nominalmente como diferencial na vaga da MJV.
- [ ] Escrever um estudo de caso (sanitizado, sem dado do cliente) da migração Oracle →
      Power BI: volume, tempo antes/depois, o que automatizou. Vale mais que um projeto novo.

### Contínuo
- [ ] Inglês técnico — leitura e escrita. Sem isso, o mercado remoto que paga bem fica fora.
- [ ] Números em tudo. "80+ usuários" você já tem. Falta: quantos relatórios migrados,
      quantas horas/mês economizadas, quantos endpoints administrados.

---

## 6. O que mexer no perfil, por ordem de impacto

| # | Ação | Esforço | Impacto |
|---|---|---|---|
| ✅ | Título/posicionamento: de "Estagiário de TI" para dev Python/Dados | feito | 🔥🔥🔥 |
| ✅ | Resolver o projeto sem link (removido) | feito | 🔥🔥🔥 |
| ✅ | Explicitar Git, Flask, API REST, ETL na stack (você já usa) | feito | 🔥🔥 |
| 1 | Replicar o novo posicionamento no LinkedIn | 20 min | 🔥🔥🔥 |
| 2 | Quantificar as entregas do trabalho atual | 30 min | 🔥🔥 |
| 3 | Certificação cloud (AZ-900) | 3–4 semanas | 🔥🔥🔥 |
| 4 | Testes + CI no NeuroDrive | 1 semana | 🔥🔥 |
| 5 | Projeto pipeline end-to-end (agora é o único caminho para um 2º projeto) | 4–6 semanas | 🔥🔥🔥 |
| 6 | Versão em inglês do README | 1h | 🔥 |

---

## 7. Vagas do recorte que já dá para disputar hoje

Ordenadas por aderência ao perfil atual:

1. [Analista de Dados I com foco em Auditoria — Grupo Panvel](https://to.indeed.com/aadhzzybvl4k)
   — pede exatamente Python/pandas + SQL + Power BI + noções de ETL, aceita superior em
   andamento e ainda valoriza IA aplicada. **É a vaga mais aderente do recorte**, e o viés
   de auditoria/controle conversa direto com sua vivência de compliance e LGPD.
   Ponto de atenção: presencial em Eldorado do Sul.
2. [Pessoa Desenvolvedora (Power BI + Python) — MJV Innovation](https://to.indeed.com/aalyds9lr7nm)
   — remoto, é a versão sênior do que você já faz. Hoje falta DAX/M avançado e Databricks;
   é a vaga-alvo para daqui a 6–12 meses.
3. [Profissional Desenvolvedor de Software Júnior — Radix](https://to.indeed.com/aa664rsq69w4)
   — remoto, exige só conhecimento **básico** de Python, Git e APIs REST, e cita Flask e
   dashboards como diferencial. A barreira é Angular. Boa relação esforço/retorno.
4. [Desenvolvedor Junior — Grupo AFL](https://to.indeed.com/aafnbsgyw9vr)
   — São Leopoldo, pede 1–3 anos e Python + Next.js. Fica viável quando o tempo de casa
   fechar 1 ano; o gap real é front-end.
5. [Engenheiro de dados Junior — Aliare](https://to.indeed.com/aa7rcpmkksjc)
   — remoto, Python + SQL + cloud básica + Docker (que você já tem). O gap é ferramenta de
   ETL (Pentaho/Talend) e cloud. **Depois do projeto-âncora e do AZ-900, esta entra no radar.**

Referência de piso local: [ESTÁGIO - TI (METTA)](https://to.indeed.com/aaxkxdnvytpr) paga
R$ 1.200 por 5h30/dia para fazer suporte, acessos e "projetos de automação". Você já está
acima disso — use como argumento na próxima negociação, não como alvo.

---

## 8. Resumo em três frases

Seu problema não é falta de habilidade, é **posicionamento e evidência**: você faz trabalho
de dados e se apresenta como suporte, e faz Python sério mas mostra pouco código público.
As duas lacunas técnicas que valem dinheiro agora são **cloud** e **testes automatizados**.
Um único projeto de pipeline end-to-end, bem documentado, cobre metade da lista de
requisitos das vagas que você quer.
