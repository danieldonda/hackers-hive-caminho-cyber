---
titulo: Etapa 3 — Fundamentos de Segurança
tipo: conceito
etapa: 3
duracao: 3 semanas
tags:
  - tipo/conceito
  - etapa/fundamentos
  - metodo
  - status/nao-iniciado
aliases:
  - Fundamentos
  - Etapa 3
---

# 3️⃣ Etapa 3 — Fundamentos de Segurança

⬅ Anterior: [[2️⃣ Etapa 2 - Sistemas Operacionais]] · ➡ Próxima: [[4️⃣ Etapa 4 - Especialização]]

> **Pergunta desta etapa:** *O que eu estou protegendo, de quê, e como sei que fui atacado?*
> **Duração sugerida:** 3 semanas (~6–8h/semana)

---

## Por que esta etapa

Até aqui você aprendeu **como as coisas funcionam**. Agora você aprende **como elas quebram** — e, mais importante, como pensar sobre isso.

Esta é a etapa que separa o técnico do profissional de segurança. Técnico acha problema. Profissional de segurança sabe dizer **qual problema importa, por quê, e o que fazer a respeito**.

---

## O que estudar (nesta ordem)

### Bloco A — O vocabulário do risco (semana 1)

- [ ] **Tríade CIA** — Confidencialidade, Integridade, Disponibilidade (e por que às vezes elas se contradizem)
- [ ] **Ameaça × Vulnerabilidade × Risco** — a distinção mais mal usada da área
- [ ] **Ativo e superfície de ataque** — o que você tem, e por onde ele pode ser atingido
- [ ] **Impacto e probabilidade** — como se prioriza no mundo real
- [ ] **Defesa em profundidade** — por que uma camada nunca basta
- [ ] **Modelagem de ameaças (introdução)** — pensar como quem quer entrar

> 🎯 **Teste de domínio:** pegue um sistema que você usa (seu e-mail, seu banco) e descreva 3 ameaças, 3 vulnerabilidades possíveis e o risco resultante de cada combinação.

### Bloco B — Identidade e acesso (semana 2)

- [ ] **AAA** — Autenticação, Autorização, Contabilização
- [ ] **Fatores de autenticação** — algo que você sabe, tem, é; por que MFA muda o jogo
- [ ] **Menor privilégio e segregação de funções** — o controle mais barato e mais ignorado
- [ ] **Modelos de controle de acesso** — RBAC, ABAC, e o que sua empresa provavelmente usa
- [ ] **Criptografia** — simétrica vs. assimétrica, para que serve cada uma
- [ ] **Hash** — o que é, por que **não é** criptografia, para que serve (senhas, integridade)
- [ ] **Certificados e PKI** — o que o cadeado do navegador realmente garante

> 🎯 **Teste de domínio:** explique por que armazenar senha com hash + salt é diferente de "criptografar a senha".

### Bloco C — Ameaças, ataques e evidências (semana 3)

- [ ] **Tipos de malware** — vírus, worm, trojan, ransomware, infostealer, RAT
- [ ] **Engenharia social** — phishing, pretexting, e por que o humano é o vetor preferido
- [ ] **Ataques comuns** — força bruta, credential stuffing, man-in-the-middle, injeção, DoS
- [ ] **Cadeia de ataque** — Cyber Kill Chain e **MITRE ATT&CK** (táticas e técnicas)
- [ ] **IOC e IOA** — indicadores de comprometimento e de ataque
- [ ] **Log como evidência** — o que registrar, por quanto tempo, e como preservar
- [ ] **Controles preventivos, detectivos e corretivos** — a classificação que organiza tudo

> 🎯 **Teste de domínio:** pegue um ataque de ransomware noticiado e mapeie as fases dele no MITRE ATT&CK.

---

## 🧪 Laboratórios obrigatórios

| # | Laboratório | O que prova |
|---|---|---|
| 1 | Analisar um e-mail de phishing real (dos seus próprios spams): cabeçalhos, links, pretexto | Você identifica o vetor mais comum de verdade |
| 2 | Gerar hashes de arquivos, alterar um byte, comparar os hashes | Você entende integridade na prática |
| 3 | Configurar MFA em três serviços seus e documentar o que mudou no fluxo de login | Você vive o controle antes de recomendá-lo |
| 4 | Escolher um incidente público e escrever uma linha do tempo do ataque | Você raciocina como analista |

Registro: [[🧫 Template - Sessão de Laboratório]]

---

## ✅ Critério de saída — só avance se

- [ ] Explico a tríade CIA com exemplos reais de cada pilar
- [ ] Diferencio ameaça, vulnerabilidade e risco sem hesitar
- [ ] Explico criptografia simétrica, assimétrica e hash — e quando usar cada um
- [ ] Conheço as principais táticas do MITRE ATT&CK e sei para que serve o framework
- [ ] Identifico um phishing analisando cabeçalhos e não só "achando estranho"
- [ ] Digo, diante de um cenário, qual controle aplicar e por quê
- [ ] Sei que evidência procurar quando suspeito de comprometimento

---

## ⛔ Nesta etapa, NÃO estude

- Análise de malware / engenharia reversa (é especialização inteira)
- Desenvolvimento de exploits
- Normas completas (ISO 27001, NIST CSF na íntegra) — conheça o nome, não decore o texto
- Ferramentas de SIEM específicas — vem na especialização

Contexto: [[⛔ O Que NÃO Estudar Agora]]

---

## 🔗 Esta etapa alimenta todas as áreas

| Área | O que ela puxa daqui |
|---|---|
| [[🛡 SOC - Blue Team]] | IOC, ATT&CK, análise de log |
| [[🔬 DFIR - Forense e Resposta a Incidentes]] | Evidência, cadeia de custódia, linha do tempo |
| [[🎯 Threat Hunting]] | Hipótese baseada em técnica ATT&CK |
| [[⚔ Pentest - Red Team]] | Superfície de ataque, cadeia de ataque |
| [[☁ Cloud Security]] | Identidade, menor privilégio, criptografia |
| [[📋 GRC - Governança, Risco e Conformidade]] | Risco, controle, impacto × probabilidade |

Por isso ela é a **última etapa comum**: é o tronco de onde saem todos os galhos.

---

## 🤖 Prompts de IA para esta etapa

```
Me apresente um cenário corporativo com uma falha de segurança embutida. 
Me peça para identificar: o ativo, a ameaça, a vulnerabilidade, o risco 
e o controle recomendado. Depois avalie minha resposta como um gestor 
de segurança avaliaria.
```

Mais em [[🤖 Prompts de IA - Seu Tutor 24h]].

---

**Relacionado:** [[📖 Glossário]] · [[🔐 Ferramentas por Etapa]] · [[4️⃣ Etapa 4 - Especialização]] · [[🗺 Roadmap Visual]]
