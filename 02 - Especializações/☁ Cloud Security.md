---
titulo: Cloud Security
tipo: conceito
tags:
  - tipo/conceito
  - area/cloud
  - etapa/especializacao
  - status/nao-iniciado
aliases:
  - Cloud
  - Segurança em Nuvem
---

# ☁ Cloud Security

⬅ [[4️⃣ Etapa 4 - Especialização]] · 🏠 [[🏠 HOME - Caminho Cyber]]

> **Em uma frase:** proteger o que não está mais no seu datacenter — onde a rede é software, o perímetro é identidade e um clique errado expõe tudo para a internet.

---

## O trabalho de verdade

Na nuvem, a maioria dos incidentes não vem de exploit sofisticado. Vem de **configuração**: um bucket público, uma chave de acesso vazada no GitHub, uma permissão excessivamente ampla que ninguém revisou.

O dia a dia envolve:
- revisar arquitetura e desenhar controles antes de o ambiente subir;
- governar identidade e permissões (IAM) — o novo perímetro;
- caçar configuração insegura com ferramentas de postura (CSPM);
- integrar segurança no pipeline de CI/CD;
- monitorar logs de nuvem e responder a alertas.

> [!important] O conceito que organiza tudo: **responsabilidade compartilhada**
> O provedor protege a nuvem. **Você** protege o que coloca nela. Quase todo incidente famoso de nuvem está do lado do cliente da linha divisória.

---

## É para você se…

- ✅ Você gosta de arquitetura e de pensar sistemas inteiros
- ✅ Automação te atrai mais que operação manual
- ✅ Você não tem preguiça de ler documentação
- ✅ Você quer uma área com demanda alta e oferta baixa de profissionais

## Provavelmente não é se…

- ❌ Você quer trabalho "mão na massa" de investigação
- ❌ Ler documentação extensa te desmotiva
- ❌ Você ainda não tem base de rede — aqui isso trava tudo

---

## O que estudar

### Base
- [ ] **Modelo de responsabilidade compartilhada** — IaaS, PaaS, SaaS
- [ ] **IAM** — usuários, papéis, políticas, federação, menor privilégio na nuvem
- [ ] **Rede em nuvem** — VPC/VNet, sub-redes, security groups, endpoints privados
- [ ] **Armazenamento** — controle de acesso, criptografia em repouso, exposição pública
- [ ] **Logging e monitoração** — trilhas de auditoria, logs de fluxo, serviços de detecção nativos
- [ ] **Criptografia e gestão de chaves** — KMS, segredos, rotação
- [ ] **CSPM** — postura, benchmarks, correção de desvio
- [ ] **Contêineres e Kubernetes** — segurança de imagem, runtime, RBAC do cluster
- [ ] **IaC** — Terraform, e análise de segurança do código de infraestrutura
- [ ] **DevSecOps** — segurança dentro do pipeline

> [!tip] Escolha **um** provedor e vá fundo
> AWS, Azure ou GCP. Os conceitos são transferíveis; os detalhes não. Aprender três pela metade é a versão nuvem da dispersão descrita em [[⛔ O Que NÃO Estudar Agora]].
>
> Critério simples: **veja as vagas da sua região**. Estude o provedor que aparece mais.

---

## 🧪 Projetos que provam sua capacidade

1. **Conta gratuita** no provedor escolhido — com alerta de custo configurado desde o primeiro minuto
2. **Ambiente inseguro de propósito** → rode uma ferramenta de postura → corrija tudo → documente antes/depois
3. **Infraestrutura como código** — suba um ambiente com Terraform aplicando boas práticas de segurança
4. **Pipeline com verificação de segurança** — CI/CD que bloqueia deploy inseguro
5. **Detecção na nuvem** — habilite os serviços nativos de log e detecção e provoque um alerta

> [!danger] Cuidado com a conta
> Configure limite e alerta de gasto **antes** de qualquer laboratório. Recurso esquecido ligado é o erro mais caro (literalmente) de quem estuda nuvem.

---

## Progressão de carreira

```
Analista de Segurança em Nuvem → Engenheiro de Segurança em Nuvem
                                          │
                                          ▼
                          Arquiteto de Segurança em Nuvem
                                          │
                                          ▼
                                    DevSecOps / Platform Security
```

Vantagem real: é a área com melhor relação demanda/oferta hoje. Quem vem de infraestrutura ou desenvolvimento tem atalho natural aqui.

---

## Pré-requisitos deste caminho

| Vem de | Por quê |
|---|---|
| [[1️⃣ Etapa 1 - Redes]] | VPC, sub-rede e roteamento são rede clássica em outra roupa |
| [[2️⃣ Etapa 2 - Sistemas Operacionais]] | Linux é a base de quase todo workload em nuvem |
| [[3️⃣ Etapa 3 - Fundamentos de Segurança]] | Identidade, menor privilégio e criptografia são o coração da área |

---

**Relacionado:** [[⚔ Pentest - Red Team]] · [[📋 GRC - Governança, Risco e Conformidade]] · [[🧰 Projetos Práticos]] · [[🔐 Ferramentas por Etapa]]
