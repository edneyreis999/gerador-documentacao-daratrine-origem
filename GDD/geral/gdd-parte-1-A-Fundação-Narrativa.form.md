# Parte I: A Fundação Narrativa - Definindo o Núcleo do Seu Jogo

<!-- Persona: Throllim Cinza‑Memória | Estilo técnico, conciso e pragmático.
     Não crie o GDD agora — este arquivo é um TEMPLATE pronto para preenchimento. -->

- Público‑alvo: O narrative Design chefe do jogo.
- Escopo: Somente a Parte I do documento fonte em `pesquisas/GDD Narrativo/Plano de GDD Narrativo para RPG Maker.docx`.
- Regra de progresso: `Progresso (%) = (itens marcados / total) × 100`.
- Como contar: some todas as caixas `[ ]` deste documento (total) e quantas foram marcadas `[x]`.
- Pesos por seção (opcional): Logline (25%), Premissa (25%), Temas (30%), Tom (20%).

Resumo de Progresso (preencher manualmente): Concluído __/__ (__%).

---

## 1.1. A Logline: A História em uma Sentença

Objetivo: sintetizar a essência da trama em uma única frase com protagonista, objetivo, conflito/obstáculo e contraste.

Resultado esperado: uma logline clara, acionável e testável como diretriz para decisões futuras.

Campos

 - Logline v1 (1 frase): Um garoto talentoso e mimado quer jogar futebol rúnico para sentir liberdade e aprovação, mas o pai‑general o pune e o retira do time; se ceder, perde autonomia; se desafiar, arrisca casa e amigos.
- Logline v2 (opcional): Um jovem talentoso busca liberdade e aprovação jogando futebol rúnico, mas o pai‑general o expõe com punições públicas e o afasta do time; obedecer custa autonomia; desafiar pode custar lar e pertencimento.
 - Notas de intenção (1–2 bullets): <!-- O que não pode faltar no jogo à luz da logline -->
   - [rascunho] Começa sem objetivo claro; o conflito com o pai dispara a mudança.
   - [rascunho] Tema semente: liberdade × dever (ganhar liberdade sem virar puro egoísmo).
   - [rascunho] Interesse romântico no time reforça motivação e risco social (sem nomes próprios).

Critérios de Aceitação

- 1 frase (recomendado ≤ 35 palavras), verbos ativos, sem nomes próprios.
- Declara protagonista por atributo (não por nome), objetivo claro e obstáculo concreto.
- Indica risco/contraste que pressiona a ação do jogador.
- Evita lore excessivo e generalidades; pode ser validada por leitura em voz alta em ≤ 10s.

Checklist

- [x] 1 frase, ≤ 35 palavras.
- [x] Protagonista descrito por atributo (sem nome próprio).
- [x] Objetivo claro com verbo ativo.
- [x] Obstáculo/antagonismo explícito.
- [x] Risco/contraste perceptível.
- [x] Sem voz passiva/lore/acréscimos supérfluos.
- [x] Variante (v2) criada e comparada (opcional).

Progresso da seção (preencher): __/__ (__%).

---

## 1.2. A Premissa: A Tese da História

Objetivo: formular a tese causal que sustenta o enredo (causa → efeito), distinguindo o que a história afirma do que ela apenas narra.

Resultado esperado: 2–3 frases que expressam tese, forças em conflito, risco central e uma escolha matricial para o jogador (E‑C‑R).

Campos

- Premissa (2–3 frases): <!-- Evite sequência de eventos; foque em tese e causalidade -->
- Forças em conflito (bullets): <!-- Ex.: "Dever × Liberdade", "Ordem × Caos" -->
- Risco central (1 frase): <!-- O que se perde se nada mudar? -->
- Escolha matricial (E‑C‑R):
  - Escolha: <!-- O que o jogador escolhe? -->
  - Consequência imediata: <!-- Estado resultante no curto prazo -->
  - Retorno (callback): <!-- Onde e quando essa escolha retorna? -->
- Rastreabilidade MZ (opcional): <!-- Mapear flags ex.: S101_EscolhaFeita, V011_Afeicao +=/‑= -->

Critérios de Aceitação

- Distingue tese de enredo; não é lista cronológica de eventos.
- Declara causalidade explícita (se/então/mas/portanto) e risco central verificável.
- Contém ao menos uma instância E‑C‑R plausível para gameplay.
- Define como rastrear a escolha no MZ (Switch/Variável) quando aplicável.

Checklist

- [ ] Premissa escrita em 2–3 frases focadas na tese.
- [ ] Causalidade explícita (se/então/mas/portanto).
- [ ] Risco central definido e testável.
- [ ] 1 E‑C‑R formalizada (Escolha, Consequência, Retorno).
- [ ] Mapeamento de flags MZ (S###/V###) definido (opcional mas recomendado).

Progresso da seção (preencher): __/__ (__%).

---

## 1.3. Os Temas: A Alma da História

Objetivo: selecionar 2–4 temas e mostrar como cada um se manifesta nos principais vetores do jogo.

Resultado esperado: lista curta de temas com manifestações exemplificadas por vetor (diálogo, quests, mundo, ambiental) e contratemas claros.

Instruções
<!-- Para cada tema, preencha 2–3 manifestações distribuídas entre os vetores. Evite nomes próprios; use exemplos genéricos. -->

Tema 1

- Declaração do tema: <!-- Ex.: "Custo da ambição" -->
- Contratema (antítese): <!-- Ex.: "Valor da renúncia" -->
- Manifestações por vetor:
  - Diálogo: <!-- Ex.: NPC exige preço pela ajuda -->
  - Quests: <!-- Ex.: escolha entre lucro rápido × confiança -->
  - Mundo: <!-- Ex.: área próspera com consequências visíveis -->
  - Ambiental: <!-- Ex.: trilha tensa em áreas ricas -->

Tema 2

- Declaração do tema:
- Contratema (antítese):
- Manifestações por vetor:
  - Diálogo:
  - Quests:
  - Mundo:
  - Ambiental:

Tema 3 (opcional)

- Declaração do tema:
- Contratema (antítese):
- Manifestações por vetor:
  - Diálogo:
  - Que
  - Mundo:
  - Ambiental:

Rastreabilidade MZ (opcional)

- Sinalizações sugeridas: `V010_Tema1_Presenca`, `V011_Tema2_Presenca` (0–100), `S120_Tema1_QuestChave`.
- Uso recomendado: checagens condicionais em eventos para reforçar tema quando variável ≥ limiar.

Critérios de Aceitação

- 2–4 temas com contratemas correspondentes.
- Ao menos 2 manifestações por tema, distribuídas entre vetores.
- Exemplos concretos e genéricos (sem nomes próprios), alinhados à premissa.
- Opcional: mapeamento de rastreabilidade via Switches/Variáveis.

Checklist

- [ ] 2–4 temas definidos.
- [ ] Contratema para cada tema.
- [ ] ≥ 2 manifestações por tema (em vetores distintos quando possível).
- [ ] Exemplos claros e genéricos.
- [ ] (Opcional) Flags MZ planejadas para monitoramento.

Progresso da seção (preencher): __/__ (__%).

---

## 1.4. O Tom: A Voz e a Atmosfera da História

Objetivo: definir a voz, a atmosfera emocional e a cadência que guiarão diálogos, narração e ambientação.

Resultado esperado: 3–5 descritores de tom com diretrizes de linguagem, ritmo e tradução prática para assets.

Campos

- Descritores de tom (3–5): <!-- Ex.: "sério", "sarcástico contido", "melancólico" -->
- Paleta emocional (bullets): <!-- Emoções foco por capítulo/área, se houver -->
- Diretrizes de linguagem: <!-- Dicção, figuras de linguagem permitidas/proibidas, nível de formalidade -->
- Ritmo e cadência: <!-- Frases curtas/longas; pausas; variação -->
- Não‑fazer (red lines): <!-- Termos proibidos, humor fora de tom, etc. -->
- Referências (opcional): <!-- 2–3 comparáveis de tom em mídia/jogos -->
- Tradução prática no MZ (opcional): <!-- Ex.: BGM X para áreas Y; SFX discretos; paleta de cores na UI -->

Critérios de Aceitação

- 3–5 descritores que guiem escrita e ambientação de forma consistente.
- Diretrizes transformáveis em regras de revisão (checáveis por checklist).
- (Opcional) Mapeamento claro de tom → assets/eventos no MZ.

Checklist

- [ ] 3–5 descritores definidos.
- [ ] Diretrizes de linguagem objetivas.
- [ ] Ritmo/cadência exemplificados.
- [ ] Lista de não‑fazer documentada.
- [ ] (Opcional) Exemplos comparáveis referenciados.
- [ ] (Opcional) Regras de tradução para MZ (BGM/SFX/UI).

Progresso da seção (preencher): __/__ (__%).

---

Resumo de Progresso Final (preencher manualmente)

- Concluído __/__ (__%).
- Regra: `Progresso (%) = (itens marcados / total) × 100`.

<!-- Fim do TEMPLATE — Parte I: A Fundação Narrativa -->
