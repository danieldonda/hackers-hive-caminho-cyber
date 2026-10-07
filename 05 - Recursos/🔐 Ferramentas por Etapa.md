---
titulo: Ferramentas por Etapa
tipo: referencia
tags:
  - tipo/referencia
  - recurso
  - ferramentas
  - caminho-cyber
aliases:
  - Ferramentas
---

# 🔐 Ferramentas por Etapa

⬅ [[🏠 HOME - Caminho Cyber]] · ⛔ [[⛔ O Que NÃO Estudar Agora]]

---

> [!important] A regra que evita 80% da dispersão
> Aprenda a ferramenta **dentro da etapa onde ela faz sentido**. Ferramenta antes de fundamento é decoreba: você aprende a clicar, não a decidir.

Ferramenta muda a cada dois anos. Fundamento dura a carreira. Por isso a lista abaixo é curta — e proposital.

---

## 🌐 Etapa 1 — Redes → [[1️⃣ Etapa 1 - Redes]]

| Ferramenta | Para quê | Prioridade |
|---|---|---|
| **Wireshark** | Ver o tráfego de verdade | ⭐⭐⭐ Essencial |
| **Nmap** | Descobrir hosts, portas e serviços | ⭐⭐⭐ Essencial |
| `ping`, `traceroute`/`tracert` | Testar conectividade e caminho | ⭐⭐⭐ |
| `nslookup` / `dig` | Consultar DNS | ⭐⭐⭐ |
| `netstat` / `ss` | Ver conexões e portas em escuta | ⭐⭐⭐ |
| `curl` | Requisições HTTP pela linha de comando | ⭐⭐ |
| **tcpdump** | Captura em servidor sem interface | ⭐⭐ |

**Ainda não:** ferramentas de ataque de rede, exploração, ferramentas de vendor.

---

## 💻 Etapa 2 — Sistemas Operacionais → [[2️⃣ Etapa 2 - Sistemas Operacionais]]

### Linux
| Ferramenta | Para quê |
|---|---|
| Terminal + `grep`, `find`, `awk`, `sed` | Encontrar qualquer coisa em qualquer lugar |
| `ps`, `top`, `htop` | Processos |
| `systemctl`, `journalctl` | Serviços e logs |
| `chmod`, `chown`, `ls -l` | Permissões |
| SSH | Acesso remoto e chaves |

### Windows
| Ferramenta | Para quê |
|---|---|
| **Event Viewer** | A fonte de evidência número um |
| **PowerShell** | Consultar e automatizar |
| **Sysinternals** (Process Explorer, Autoruns, TCPView) | Ver o que o Gerenciador de Tarefas não mostra |
| `services.msc`, `regedit` | Serviços e registro |

### Virtualização
| Ferramenta | Para quê |
|---|---|
| **VirtualBox** ou **VMware Player** | Seu laboratório inteiro |

**Ainda não:** automação avançada, ferramentas de administração corporativa, EDR.

---

## 🔐 Etapa 3 — Fundamentos → [[3️⃣ Etapa 3 - Fundamentos de Segurança]]

| Ferramenta | Para quê | Prioridade |
|---|---|---|
| **MITRE ATT&CK** (o site) | O mapa de táticas e técnicas | ⭐⭐⭐ Essencial |
| Analisador de cabeçalho de e-mail | Triagem de phishing | ⭐⭐⭐ |
| Serviços de reputação de IP/domínio/hash | Verificar indicadores | ⭐⭐⭐ |
| Utilitários de hash (`sha256sum`, `Get-FileHash`) | Integridade | ⭐⭐ |
| Gerenciador de senhas | Higiene pessoal — comece por você | ⭐⭐⭐ |
| Aplicativo de MFA | Idem | ⭐⭐⭐ |

**Ainda não:** SIEM, sandbox de malware, scanner de vulnerabilidade.

---

## 🎯 Etapa 4 — Por área → [[4️⃣ Etapa 4 - Especialização]]

| Área | Ferramentas centrais |
|---|---|
| [[🛡 SOC - Blue Team]] | SIEM (Wazuh, ELK, Splunk), EDR, plataforma de intel |
| [[🔬 DFIR - Forense e Resposta a Incidentes]] | Aquisição forense, análise de memória, suítes de artefato, timeline |
| [[🎯 Threat Hunting]] | **Sysmon**, plataforma de dados, linguagem de consulta, emulação de adversário |
| [[⚔ Pentest - Red Team]] | Nmap avançado, Burp/ZAP, Metasploit, ferramentas de AD |
| [[☁ Cloud Security]] | CLI do provedor, CSPM, Terraform, ferramentas de contêiner |
| [[📋 GRC - Governança, Risco e Conformidade]] | Planilha, matriz de risco, ferramenta de GRC, frameworks |

---

## Sobre distribuições de segurança (Kali, Parrot)

> [!warning] Instalar Kali não te torna pentester
> Kali é uma caixa de ferramentas para quem já sabe qual ferramenta pegar. Instalado no dia 1, ele vira um Linux estranho com 600 programas que você não entende.
>
> **Quando faz sentido:** Etapa 3 ou 4, como VM, depois que você já opera Linux com naturalidade.
>
> **Antes disso:** use Ubuntu ou Debian e instale o que precisar. Você aprende mais instalando cinco ferramentas do que recebendo seiscentas prontas.

---

## Escolha por critério, não por hype

Antes de aprender qualquer ferramenta nova, responda:

1. Ela pertence à etapa em que estou?
2. Ela resolve um problema que eu já entendo?
3. Ela aparece nas vagas da minha região?
4. Eu consigo praticar com ela hoje?

Menos de 3 "sim"? Anote em [[⛔ O Que NÃO Estudar Agora]] com uma data para revisitar.

---

**Relacionado:** [[🧪 Laboratório em Casa]] · [[🗺 Roadmap Visual]] · [[🌐 Fontes Confiáveis]] · [[📖 Glossário]]
