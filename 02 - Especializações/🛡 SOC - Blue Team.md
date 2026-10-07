---
titulo: SOC — Blue Team
tipo: conceito
tags:
  - tipo/conceito
  - area/soc
  - etapa/especializacao
  - status/nao-iniciado
aliases:
  - SOC
  - Blue Team
  - Analista de SOC
---

# 🛡 SOC — Blue Team

⬅ [[4️⃣ Etapa 4 - Especialização]] · 🏠 [[🏠 HOME - Caminho Cyber]]

> **Em uma frase:** vigiar o ambiente em tempo real, decidir o que é ataque e agir antes que vire incidente.

---

## O trabalho de verdade

Você recebe alertas. Muitos. A maioria é falso positivo. Seu trabalho é **triar**: olhar cada um, decidir se é ruído ou ameaça, investigar o que merece investigação, escalar o que passa do seu nível e documentar tudo.

Um dia típico de analista N1:
- fila de alertas do SIEM;
- investigação de logons suspeitos, e-mails reportados, alertas de EDR;
- consulta a fontes de inteligência para checar um IP, hash ou domínio;
- registro em ticket, com evidência e justificativa;
- passagem de plantão.

> [!info] Por que é a porta de entrada mais comum
> É a área com mais vagas júnior no Brasil, tem processo estruturado (você aprende com método, não sozinho) e forma uma base que serve para **todas** as outras áreas.

---

## É para você se…

- ✅ Você aguenta rotina e volume sem perder atenção
- ✅ Você gosta de investigar coisas pequenas até o fim
- ✅ Você trabalha bem sob procedimento e escala de plantão
- ✅ Você quer entrar rápido no mercado

## Provavelmente não é se…

- ❌ Rotina repetitiva te destrói
- ❌ Você odeia a ideia de escala noturna ou fim de semana
- ❌ Você quer autonomia total desde o primeiro dia

---

## O que estudar (depois das etapas 1 a 3)

### Base
- [ ] Análise de logs — Windows Event Log, Syslog, logs de firewall, proxy, DNS
- [ ] **SIEM** — conceito, ingestão, correlação, regras, casos de uso
- [ ] **EDR/XDR** — o que detecta, o que registra, como se investiga por ele
- [ ] **MITRE ATT&CK** aplicado à detecção
- [ ] Triagem de e-mail — cabeçalhos, SPF/DKIM/DMARC, análise de anexo e URL
- [ ] Threat intelligence básica — IOC, reputação, feeds

### Ferramentas (aprenda **uma** de cada tipo)
| Tipo | Opções gratuitas para estudar |
|---|---|
| SIEM | Wazuh, Elastic Stack (ELK), Splunk Free |
| Análise de e-mail | Ferramentas de análise de cabeçalho, sandbox pública |
| Reputação/IOC | Serviços públicos de reputação de IP, domínio e hash |
| EDR | Versões community/trial de EDR conhecidos |

### Habilidades não técnicas (subestimadas e decisivas)
- [ ] Escrever com clareza — seu ticket é lido por quem vai decidir
- [ ] Comunicar urgência sem alarmismo
- [ ] Passar plantão sem perder contexto

---

## 🧪 Projetos que provam sua capacidade

1. **Monte um SIEM em casa** — Wazuh em uma VM, agentes em duas máquinas, dashboards funcionando
2. **Crie 5 regras de detecção** — logon fora do horário, múltiplas falhas de autenticação, execução de PowerShell codificado, criação de conta administrativa, desativação de log
3. **Simule e detecte** — gere o evento, veja o alerta disparar, escreva o relatório de triagem
4. **Documente 10 triagens** — como se fossem tickets reais, com evidência e conclusão

Formato de registro: [[🧫 Template - Sessão de Laboratório]] · Portfólio: [[💼 Portfólio e Presença Profissional]]

---

## Progressão de carreira

```
Analista N1 → Analista N2 → Analista N3 / Líder de turno
     │              │                    │
     │              ▼                    ▼
     │        Threat Hunting        Coordenação de SOC
     ▼
    DFIR
```

Caminhos naturais a partir daqui: [[🔬 DFIR - Forense e Resposta a Incidentes]] · [[🎯 Threat Hunting]]

---

## Certificações (só depois de decidir)

Ordem que costuma fazer sentido: fundamentos de segurança (nível Security+) → certificação de analista defensivo (nível Blue Team / SOC analyst) → especialização em SIEM do fornecedor que você usa.

Contexto: [[🎓 Certificações - Quando Pensar Nisso]]

---

## Pré-requisitos deste caminho

| Vem de | Por quê |
|---|---|
| [[1️⃣ Etapa 1 - Redes]] | Metade dos alertas é sobre tráfego |
| [[2️⃣ Etapa 2 - Sistemas Operacionais]] | A outra metade é sobre processos, contas e logons |
| [[3️⃣ Etapa 3 - Fundamentos de Segurança]] | IOC, ATT&CK e priorização de risco |

---

**Relacionado:** [[🎯 Threat Hunting]] · [[🔬 DFIR - Forense e Resposta a Incidentes]] · [[🧰 Projetos Práticos]] · [[🔐 Ferramentas por Etapa]]
