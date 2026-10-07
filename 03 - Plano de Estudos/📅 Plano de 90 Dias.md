---
titulo: Plano de 90 Dias
tipo: checklist
tags:
  - tipo/checklist
  - plano
  - caminho-cyber
  - status/em-andamento
aliases:
  - Plano
  - 90 dias
---

# 📅 Plano de 90 Dias

⬅ [[🗺 Roadmap Visual]] · 🏠 [[🏠 HOME - Caminho Cyber]]

---

**Data de início:** ___/___/______
**Data prevista de término:** ___/___/______
**Horas por semana comprometidas:** ___

> [!info] Calibragem
> Este plano assume **6 a 8 horas semanais**. Com 4h/semana, some ~50% ao prazo. O que **não** se ajusta é a ordem.

Marque cada caixa conforme concluir. O que não foi feito não some — ele empurra a semana seguinte.

---

## 🌐 BLOCO 1 — REDES · Semanas 1 a 3
> Nota da etapa: [[1️⃣ Etapa 1 - Redes]]

### Semana 1 — O modelo mental
- [ ] Modelo OSI e TCP/IP: as camadas e a lógica da divisão
- [ ] Endereçamento IP, máscara, gateway, sub-rede
- [ ] IP público × privado · MAC address
- [ ] Switch, roteador, firewall: o que cada um decide
- [ ] 🧪 **Lab:** mapear a própria rede doméstica (dispositivos, IPs, portas)
- [ ] 📝 1 nota de estudo criada com [[📋 Template - Nota de Estudo]]
- [ ] 🔁 Revisão de domingo

### Semana 2 — Protocolos
- [ ] TCP × UDP e o handshake de 3 vias
- [ ] Portas e serviços: as 20 principais, de cor
- [ ] DNS e DHCP
- [ ] HTTP/HTTPS · NAT · VPN
- [ ] 🧪 **Lab:** capturar login em HTTP vs HTTPS no Wireshark e comparar
- [ ] 📝 1 nota de estudo
- [ ] 🔁 Revisão de domingo

### Semana 3 — Ver com os próprios olhos
- [ ] Wireshark: filtros e leitura de handshake
- [ ] Nmap: varredura de host, porta e serviço
- [ ] `ping`, `traceroute`, `nslookup`/`dig`, `netstat`/`ss`, `curl`
- [ ] 🧪 **Lab:** varrer VM própria e documentar cada serviço encontrado
- [ ] ✅ **Critério de saída da Etapa 1** conferido item a item
- [ ] 📈 Registrar marco em [[📈 Registro de Evolução]]

---

## 💻 BLOCO 2 — SISTEMAS OPERACIONAIS · Semanas 4 a 7
> Nota da etapa: [[2️⃣ Etapa 2 - Sistemas Operacionais]]

### Semana 4 — Linux: fundamentos
- [ ] Terminal: navegação, busca, pipes e redirecionamento
- [ ] Hierarquia de diretórios e o que mora em cada lugar
- [ ] Permissões: leitura de `rwx`, `chmod`, `chown`, SUID
- [ ] 🧪 **Lab:** instalar Linux do zero em VM
- [ ] 📝 1 nota · 🔁 Revisão

### Semana 5 — Linux: operação
- [ ] Usuários, grupos, `sudo`
- [ ] Processos e serviços (`ps`, `systemctl`)
- [ ] Logs: `/var/log` e `journalctl`
- [ ] SSH e hardening básico
- [ ] 🧪 **Lab:** 3 usuários com permissões distintas + teste do que cada um faz
- [ ] 📝 1 nota · 🔁 Revisão

### Semana 6 — Windows: fundamentos
- [ ] Usuários, grupos, UAC
- [ ] NTFS, ACLs, permissões efetivas
- [ ] Processos, serviços, Process Explorer
- [ ] Registro do Windows e chaves de execução automática
- [ ] 🧪 **Lab:** instalar Windows em VM e documentar o **baseline** (processos, serviços, portas, contas)
- [ ] 📝 1 nota · 🔁 Revisão

### Semana 7 — Windows: visibilidade
- [ ] Event Viewer e os IDs que importam (4624, 4625, 4672…)
- [ ] PowerShell: consultas básicas ao sistema
- [ ] Active Directory: domínio, OU, GPO, noções de Kerberos
- [ ] 🧪 **Lab:** provocar eventos (logon falho, serviço parado) e localizá-los nos logs
- [ ] ✅ **Critério de saída da Etapa 2** conferido
- [ ] 📈 Registrar marco

---

## 🔐 BLOCO 3 — FUNDAMENTOS DE SEGURANÇA · Semanas 8 a 10
> Nota da etapa: [[3️⃣ Etapa 3 - Fundamentos de Segurança]]

### Semana 8 — O vocabulário do risco
- [ ] Tríade CIA e seus conflitos práticos
- [ ] Ameaça × vulnerabilidade × risco
- [ ] Ativo, superfície de ataque, impacto × probabilidade
- [ ] Defesa em profundidade
- [ ] 🧪 **Lab:** análise de risco de um sistema que você usa todo dia
- [ ] 📝 1 nota · 🔁 Revisão

### Semana 9 — Identidade e criptografia
- [ ] AAA, fatores de autenticação, MFA
- [ ] Menor privilégio, segregação de funções, RBAC
- [ ] Criptografia simétrica × assimétrica · hash · certificados e PKI
- [ ] 🧪 **Lab:** MFA em 3 serviços + experimento de hash (alterar 1 byte, comparar)
- [ ] 📝 1 nota · 🔁 Revisão

### Semana 10 — Ameaças e evidências
- [ ] Tipos de malware · engenharia social · phishing
- [ ] Ataques comuns: força bruta, credential stuffing, MITM, injeção, DoS
- [ ] Kill Chain e **MITRE ATT&CK** · IOC e IOA
- [ ] Log como evidência · controles preventivos, detectivos, corretivos
- [ ] 🧪 **Lab:** dissecar um phishing real + mapear um incidente público no ATT&CK
- [ ] ✅ **Critério de saída da Etapa 3** conferido
- [ ] 📈 Registrar marco

---

## 🎯 BLOCO 4 — ESPECIALIZAÇÃO · Semanas 11 e 12
> Nota da etapa: [[4️⃣ Etapa 4 - Especialização]]

### Semana 11 — Exploração
- [ ] Ler [[🛡 SOC - Blue Team]] · anotar atrai/repele
- [ ] Ler [[🔬 DFIR - Forense e Resposta a Incidentes]] · anotar
- [ ] Ler [[🎯 Threat Hunting]] · anotar
- [ ] Ler [[⚔ Pentest - Red Team]] · anotar
- [ ] Ler [[☁ Cloud Security]] · anotar
- [ ] Ler [[📋 GRC - Governança, Risco e Conformidade]] · anotar
- [ ] Ler 3 vagas reais de cada área
- [ ] Falar com 2 profissionais da área

### Semana 12 — Decisão e lançamento
- [ ] Eliminar 3 áreas, com motivo escrito
- [ ] 1 laboratório introdutório em cada uma das 3 finalistas
- [ ] **Escolher.** Registrar a escolha e o porquê
- [ ] Ler [[🎓 Certificações - Quando Pensar Nisso]] com a área já definida
- [ ] Montar o plano dos próximos 90 dias na área escolhida
- [ ] Publicar o primeiro item de portfólio → [[💼 Portfólio e Presença Profissional]]

---

## 🏁 Fechamento

- [ ] Tenho um plano de estudo definido e escrito
- [ ] Sei o que **não** vou estudar agora
- [ ] Tenho laboratório funcionando
- [ ] Tenho pelo menos 12 notas próprias
- [ ] Tenho ao menos 1 item público de portfólio
- [ ] Sei qual é o meu próximo passo — e a data dele

> [!quote]
> **Você não precisa saber tudo. Precisa saber o próximo passo.**
> Em 90 dias, você deixou de perguntar "por onde começo?" e passou a perguntar "qual é o próximo?". Essa é a virada.

---

**Relacionado:** [[🗓 Semana Modelo]] · [[✅ Checklist de Progresso]] · [[📈 Registro de Evolução]] · [[⛔ O Que NÃO Estudar Agora]]
