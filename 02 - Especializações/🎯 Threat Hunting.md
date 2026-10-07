---
titulo: Threat Hunting
tipo: conceito
tags:
  - tipo/conceito
  - area/hunting
  - etapa/especializacao
  - status/nao-iniciado
aliases:
  - Threat Hunting
  - Caça a Ameaças
  - Hunting
---

# 🎯 Threat Hunting

⬅ [[4️⃣ Etapa 4 - Especialização]] · 🏠 [[🏠 HOME - Caminho Cyber]]

> **Em uma frase:** procurar o atacante que **já está dentro** e que nenhum alerta apontou.

---

## O trabalho de verdade

O SOC é reativo: espera o alerta. O hunter é proativo: **assume que a defesa falhou** e vai procurar a prova disso.

O ciclo é sempre o mesmo:

```
1. HIPÓTESE     "Se um atacante usasse a técnica X, deixaria o rastro Y"
      ▼
2. DADOS        Onde esse rastro estaria? Tenho essa telemetria?
      ▼
3. BUSCA        Consultar, filtrar, comparar com o baseline
      ▼
4. ANÁLISE      Achei anomalia? É malicioso ou é normal daqui?
      ▼
5. RESULTADO    Achou → vira incidente (IR)
                Não achou → vira nova regra de detecção
```

> [!important] A parte que assusta
> **A maioria das caçadas não encontra nada.** E isso não é fracasso: cada caçada sem resultado vira uma detecção nova e reduz a superfície cega. Se você precisa de vitória para se manter motivado, esta área vai te frustrar.

---

## É para você se…

- ✅ Você tem curiosidade genuína e cria hipóteses sozinho
- ✅ Você tolera trabalhar sem resposta garantida
- ✅ Você conhece profundamente o que é "normal" em um ambiente
- ✅ Você gosta de dados, consultas e padrões

## Provavelmente não é se…

- ❌ Você precisa de tarefas com começo, meio e fim claros
- ❌ Ambiguidade te trava
- ❌ Você ainda não tem base sólida de SO e rede — aqui isso é pré-requisito duro

---

## O que estudar

### Base
- [ ] **MITRE ATT&CK a fundo** — não as táticas por cima, as **técnicas** e sub-técnicas
- [ ] **Baseline e anomalia** — como se define "normal" em um ambiente
- [ ] **Telemetria** — que dado existe, onde, com qual retenção e qual lacuna
- [ ] **Linguagens de consulta** — KQL, SPL, EQL ou equivalente do seu stack
- [ ] **Modelos de hunting** — orientado a hipótese, a inteligência e a análise de dados
- [ ] **Técnicas de evasão** — living off the land, ofuscação, persistência silenciosa
- [ ] **Análise de C2** — beaconing, jitter, DNS tunneling
- [ ] Noções de **estatística e análise de dados** — frequência, outlier, agrupamento

### Ferramentas
| Tipo | Exemplos para estudar |
|---|---|
| Plataforma de dados | Elastic, Splunk, plataformas de log de nuvem |
| Telemetria de endpoint | Sysmon (essencial), EDR |
| Frameworks | MITRE ATT&CK, ferramentas de emulação de adversário |
| Análise | Jupyter/Python para tratar volume de dados |

> [!tip] Se for estudar uma coisa só, estude **Sysmon**
> Sysmon bem configurado é a diferença entre caçar com lanterna e caçar no escuro.

---

## 🧪 Projetos que provam sua capacidade

1. **Instale Sysmon** em um lab e colete tudo em um SIEM
2. **Emule 5 técnicas do ATT&CK** e cace cada uma sem olhar o que fez
3. **Escreva 5 hipóteses de caça** no formato completo: hipótese → dado → consulta → resultado
4. **Documente uma caçada que não achou nada** — e mostre qual detecção nasceu dela

---

## Progressão de carreira

Threat Hunting quase nunca é entrada. O caminho comum:

```
Analista de SOC → Analista N2/N3 → Threat Hunter → Detection Engineer
                                          │
                                          ▼
                              Liderança de Detecção / Threat Intel
```

Ponto de partida quase obrigatório: [[🛡 SOC - Blue Team]].

---

## Pré-requisitos deste caminho

| Vem de | Por quê |
|---|---|
| [[2️⃣ Etapa 2 - Sistemas Operacionais]] | Sem baseline de SO, tudo parece suspeito ou nada parece |
| [[1️⃣ Etapa 1 - Redes]] | Beaconing e exfiltração só aparecem para quem entende tráfego |
| [[3️⃣ Etapa 3 - Fundamentos de Segurança]] | ATT&CK é a linguagem da área |
| [[🛡 SOC - Blue Team]] | Experiência prévia de triagem é praticamente obrigatória |

---

**Relacionado:** [[🔬 DFIR - Forense e Resposta a Incidentes]] · [[🛡 SOC - Blue Team]] · [[🧰 Projetos Práticos]] · [[🌐 Fontes Confiáveis]]
