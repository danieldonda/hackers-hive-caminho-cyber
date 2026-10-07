---
titulo: Etapa 2 — Sistemas Operacionais
tipo: conceito
etapa: 2
duracao: 3 semanas
tags:
  - tipo/conceito
  - etapa/sistemas
  - metodo
  - status/nao-iniciado
aliases:
  - Sistemas Operacionais
  - Etapa 2
---

# 2️⃣ Etapa 2 — Sistemas Operacionais

⬅ Anterior: [[1️⃣ Etapa 1 - Redes]] · ➡ Próxima: [[3️⃣ Etapa 3 - Fundamentos de Segurança]]

> **Pergunta desta etapa:** *Onde as coisas realmente acontecem?*
> **Duração sugerida:** 3 semanas (~6–8h/semana)

---

## Por que esta etapa

Ataques não acontecem no PowerPoint. Eles acontecem em **processos, serviços, contas, arquivos, memória e logs**.

Se você não entende o sistema operacional, toda análise vira dependência de ferramenta.

---

## Linux essencial

- [ ] estrutura de diretórios
- [ ] usuários e grupos
- [ ] permissões e `sudo`
- [ ] processos (`ps`, `top`)
- [ ] serviços (`systemctl`)
- [ ] logs (`journalctl`, `/var/log`)
- [ ] rede (`ip`, `ss`)
- [ ] SSH
- [ ] pipes e redirecionamento
- [ ] `grep`, `awk`, `sed`, `find`

### Teste de domínio
Em uma máquina Linux desconhecida, descubra em poucos minutos:

- quem está logado;
- quais serviços estão ativos;
- o que escuta na rede;
- quais processos consomem mais recursos;
- onde procurar evidência de autenticação.

---

## Windows essencial

- [ ] usuários e grupos
- [ ] UAC
- [ ] NTFS e permissões
- [ ] processos e serviços
- [ ] Event Viewer
- [ ] registro
- [ ] PowerShell
- [ ] Sysinternals
- [ ] noção de Active Directory

### Teste de domínio
Encontre eventos de logon, identifique processos ativos, serviços e conexões de rede sem instalar ferramenta de terceiros.

---

## 🧪 Laboratórios

1. instale uma VM Linux e uma Windows;
2. crie usuários com privilégios diferentes;
3. gere eventos de autenticação e encontre-os nos logs;
4. documente um baseline de processos, serviços, contas e portas;
5. compare o sistema antes e depois de instalar um aplicativo.

---

## ✅ Critério de saída

- opero Linux por terminal;
- entendo permissões em Linux e Windows;
- encontro processos e serviços;
- encontro logs de autenticação;
- uso PowerShell para consultas básicas;
- explico Active Directory em nível introdutório;
- tenho pelo menos um baseline documentado.

---

## ⛔ Não estude agora

- kernel internals profundos;
- desenvolvimento de drivers;
- administração avançada de datacenter;
- automação complexa;
- hardening completo de todos os benchmarks.

---

**Relacionado:** [[🔐 Ferramentas por Etapa]] · [[🧪 Laboratório em Casa]] · [[📅 Plano de 90 Dias]]
