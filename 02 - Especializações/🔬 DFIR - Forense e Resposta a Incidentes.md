---
titulo: DFIR — Forense Digital e Resposta a Incidentes
tipo: conceito
tags:
  - tipo/conceito
  - area/dfir
  - etapa/especializacao
  - status/nao-iniciado
aliases:
  - DFIR
  - Forense
  - Resposta a Incidentes
---

# 🔬 DFIR — Forense Digital e Resposta a Incidentes

⬅ [[4️⃣ Etapa 4 - Especialização]] · 🏠 [[🏠 HOME - Caminho Cyber]]

> **Em uma frase:** quando o pior já aconteceu, descobrir exatamente o que aconteceu, como, por onde, desde quando — e garantir que acabou.

---

## O trabalho de verdade

DFIR são duas disciplinas coladas:

- **IR (Resposta a Incidentes):** conter, erradicar e recuperar. É corrida contra o relógio, sob pressão, com o negócio parado e executivos perguntando de hora em hora.
- **DF (Forense Digital):** reconstruir a história a partir de evidências. É paciência, método e rigor — porque o resultado pode ir para um tribunal.

Um caso típico:
- alerta escalado do [[🛡 SOC - Blue Team]] ou notificação externa;
- preservação de evidência (imagem de disco, dump de memória, coleta de logs);
- análise: o que executou, quando, com qual conta, o que acessou, para onde enviou;
- construção da linha do tempo;
- contenção e erradicação;
- relatório — técnico e executivo.

> [!warning] Não é glamouroso
> É muita leitura de log, muita hora sem achar nada, e muito relatório. Quem gosta, gosta *muito*. Quem não gosta, descobre rápido.

---

## É para você se…

- ✅ Você é obsessivo com detalhe e não desiste de uma pista
- ✅ Você funciona bem sob pressão real
- ✅ Você escreve bem — relatório é metade do trabalho
- ✅ Investigação te dá prazer, mesmo quando é lenta

## Provavelmente não é se…

- ❌ Você precisa de resultado rápido para se manter motivado
- ❌ Trabalho fora de horário é impeditivo
- ❌ Documentar te parece burocracia

---

## O que estudar

### Base
- [ ] **Metodologia de resposta** — preparação, identificação, contenção, erradicação, recuperação, lições aprendidas
- [ ] **Ordem de volatilidade** — o que coletar primeiro e por quê
- [ ] **Cadeia de custódia** — como a evidência mantém validade
- [ ] **Forense de memória** — o que só existe na RAM
- [ ] **Forense de disco** — sistemas de arquivos, artefatos, arquivos deletados
- [ ] **Artefatos do Windows** — Prefetch, Amcache/Shimcache, Jump Lists, MFT, USN Journal, Registro
- [ ] **Artefatos do Linux** — logs de autenticação, bash history, timestamps, cron
- [ ] **Construção de linha do tempo (timeline)** — a técnica central da área
- [ ] **Análise de malware — nível triagem** (não reversing profundo)

### Ferramentas para estudar
| Finalidade | Ferramentas |
|---|---|
| Aquisição | Ferramentas de imagem forense e dump de memória |
| Memória | Frameworks de análise de memória (ex.: Volatility) |
| Disco/artefatos | Suítes forenses open source e utilitários de artefato do Windows |
| Timeline | Ferramentas de super timeline |
| Triagem de malware | Sandbox local, análise estática básica |

---

## 🧪 Projetos que provam sua capacidade

1. **Analise uma imagem forense pública de treino** e escreva o laudo completo
2. **Comprometa a sua própria VM** (de forma controlada), depois investigue-a do zero como se não soubesse o que fez
3. **Construa uma timeline** de um incidente simulado, do acesso inicial à exfiltração
4. **Escreva dois relatórios do mesmo caso**: um técnico e um executivo de uma página

---

## Progressão de carreira

```
Analista SOC N2/N3 → Analista de IR → Consultor DFIR → Líder de IR
                            │
                            ▼
                   Threat Hunting · Detection Engineering
```

DFIR raramente é primeiro emprego. O caminho usual passa por [[🛡 SOC - Blue Team]].

---

## Certificações (depois de decidir)

Ordem usual: fundamentos → certificação de resposta a incidentes → forense de host → forense de memória/avançada. Contexto: [[🎓 Certificações - Quando Pensar Nisso]]

---

## Pré-requisitos deste caminho

| Vem de | Por quê |
|---|---|
| [[2️⃣ Etapa 2 - Sistemas Operacionais]] | **Crítico.** Forense é conhecimento profundo de SO |
| [[3️⃣ Etapa 3 - Fundamentos de Segurança]] | Evidência, IOC, cadeia de ataque |
| [[1️⃣ Etapa 1 - Redes]] | Rastrear exfiltração e comunicação com C2 |

---

**Relacionado:** [[🛡 SOC - Blue Team]] · [[🎯 Threat Hunting]] · [[🧰 Projetos Práticos]] · [[📖 Glossário]]
