---
titulo: Projetos Práticos
tipo: pratica
tags:
  - tipo/pratica
  - laboratorio
  - portfolio
  - caminho-cyber
aliases:
  - Projetos
---

# 🧰 Projetos Práticos

⬅ [[🧪 Laboratório em Casa]] · 💼 [[💼 Portfólio e Presença Profissional]]

---

12 projetos, em ordem de dificuldade. Cada um resolve dois problemas ao mesmo tempo: **fixa o aprendizado** e **vira item de portfólio**.

> [!tip] Como escolher
> Faça os 6 primeiros na ordem, durante as etapas 1 a 3. Os 6 últimos, depois de escolher a área em [[4️⃣ Etapa 4 - Especialização]].

---

## 🟢 Nível 1 — Fundamentos (etapas 1 a 3)

### 1. Mapa da minha rede
**Etapa:** [[1️⃣ Etapa 1 - Redes]] · **Tempo:** 3h

Documente sua rede doméstica: diagrama, inventário de dispositivos, portas abertas, riscos identificados e recomendações.

**Entrega:** documento com diagrama + tabela de dispositivos + 5 recomendações de segurança.
**Prova que você sabe:** enxergar uma rede e traduzir isso em risco.

### 2. Anatomia de uma conexão HTTPS
**Etapa:** [[1️⃣ Etapa 1 - Redes]] · **Tempo:** 4h

Capture no Wireshark o acesso a um site. Documente cada etapa: DNS → TCP → TLS → HTTP. Explique o que um atacante veria em cada ponto.

**Entrega:** write-up com prints e narrativa pacote a pacote.
**Prova que você sabe:** ler tráfego, não só capturá-lo.

### 3. Baseline de uma máquina
**Etapa:** [[2️⃣ Etapa 2 - Sistemas Operacionais]] · **Tempo:** 5h

Documente o estado normal de uma VM limpa: processos, serviços, portas, contas, tarefas agendadas, chaves de execução automática. Depois instale software qualquer e compare o que mudou.

**Entrega:** documento de baseline + relatório de diferenças.
**Prova que você sabe:** distinguir normal de anormal — a base de toda detecção.

### 4. Laboratório de permissões
**Etapa:** [[2️⃣ Etapa 2 - Sistemas Operacionais]] · **Tempo:** 4h

Crie 4 usuários com níveis diferentes em Linux e Windows. Teste sistematicamente o que cada um consegue e não consegue fazer. Documente onde o menor privilégio falha por má configuração.

**Entrega:** matriz de permissões testada e comentada.
**Prova que você sabe:** controle de acesso na prática.

### 5. Dissecando um phishing
**Etapa:** [[3️⃣ Etapa 3 - Fundamentos de Segurança]] · **Tempo:** 3h

Pegue um phishing real da sua caixa de spam. Analise cabeçalhos, SPF/DKIM/DMARC, o domínio, o link (sem clicar), o pretexto psicológico usado.

**Entrega:** relatório de análise com IOCs extraídos.
**Prova que você sabe:** analisar o vetor de ataque mais comum do mundo.

### 6. Linha do tempo de um incidente real
**Etapa:** [[3️⃣ Etapa 3 - Fundamentos de Segurança]] · **Tempo:** 5h

Escolha um incidente público bem documentado. Reconstrua a linha do tempo e mapeie cada fase no MITRE ATT&CK. Aponte quais controles teriam interrompido a cadeia — e onde.

**Entrega:** timeline + matriz ATT&CK + análise de controles.
**Prova que você sabe:** raciocinar como analista, não como espectador.

---

## 🟡 Nível 2 — Especialização

### 7. SIEM em casa
**Área:** [[🛡 SOC - Blue Team]] · **Tempo:** 10h
Wazuh ou ELK em uma VM, agentes em duas máquinas, dashboards funcionando, 5 regras de detecção próprias criadas e testadas.

### 8. Investigação forense completa
**Área:** [[🔬 DFIR - Forense e Resposta a Incidentes]] · **Tempo:** 12h
Comprometa sua VM de forma controlada. Depois investigue do zero: linha do tempo, artefatos, conclusão. Escreva dois relatórios — um técnico e um executivo de uma página.

### 9. Cinco caçadas documentadas
**Área:** [[🎯 Threat Hunting]] · **Tempo:** 10h
Sysmon instalado, telemetria centralizada, 5 hipóteses de caça no formato completo (hipótese → dado → consulta → resultado). Inclua uma que **não achou nada** e mostre a detecção que nasceu dela.

### 10. Laboratório de Active Directory
**Área:** [[⚔ Pentest - Red Team]] · **Tempo:** 15h
Controlador de domínio + 2 clientes, com configurações fracas propositais. Ataque, documente e escreva o relatório profissional com CVSS e recomendações.

### 11. Ambiente em nuvem: do inseguro ao seguro
**Área:** [[☁ Cloud Security]] · **Tempo:** 10h
Suba um ambiente inseguro de propósito, rode uma ferramenta de postura, corrija tudo, documente o antes e o depois. **Configure alerta de custo antes de começar.**

### 12. Programa de segurança de uma empresa fictícia
**Área:** [[📋 GRC - Governança, Risco e Conformidade]] · **Tempo:** 12h
Matriz com 20 riscos avaliados, política de segurança, avaliação de maturidade por framework e plano de ação priorizado.

> Estes projetos são excelentes para [[💼 Portfólio e Presença Profissional]]: são documentos, e documento se mostra.

---

## Como transformar projeto em portfólio

Todo projeto vira, no mínimo:

1. **Um repositório no GitHub** com README explicando o quê, o porquê e o como
2. **Um write-up** usando [[📝 Template - Write-up]]
3. **Um post no LinkedIn** — curto, com o aprendizado principal, não o passo a passo

> [!important] O erro que anula o projeto
> Fazer e não documentar. Um projeto não documentado existe só na sua cabeça — e cabeça não aparece em processo seletivo.

---

## Meu controle

| # | Projeto | Início | Fim | Documentado |
|---|---|---|---|---|
| 1 | Mapa da rede |  |  | [ ] |
| 2 | Anatomia HTTPS |  |  | [ ] |
| 3 | Baseline |  |  | [ ] |
| 4 | Permissões |  |  | [ ] |
| 5 | Phishing |  |  | [ ] |
| 6 | Timeline |  |  | [ ] |
| 7–12 | Projeto da área |  |  | [ ] |

---

**Relacionado:** [[🧪 Laboratório em Casa]] · [[💼 Portfólio e Presença Profissional]] · [[📝 Template - Write-up]] · [[✅ Checklist de Progresso]]
