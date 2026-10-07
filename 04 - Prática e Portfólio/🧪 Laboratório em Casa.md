---
titulo: Laboratório em Casa
tipo: pratica
tags:
  - tipo/pratica
  - laboratorio
  - caminho-cyber
aliases:
  - Lab
  - Home Lab
---

# 🧪 Laboratório em Casa

⬅ [[🏠 HOME - Caminho Cyber]] · 🧰 [[🧰 Projetos Práticos]]

---

> [!quote]
> Você não aprende segurança lendo sobre segurança. Aprende quebrando coisas suas e consertando depois.

O laboratório é onde a teoria vira habilidade. E ele precisa existir **desde a semana 1** — não depois que você "estiver pronto".

---

## O mínimo viável

| Recurso | Mínimo | Confortável |
|---|---|---|
| RAM | 8 GB | 16 GB |
| Disco livre | 100 GB | 250 GB (SSD) |
| Processador | 4 núcleos com virtualização | 6+ núcleos |
| Internet | qualquer | qualquer |

Não tem isso? Comece pelas plataformas online — várias oferecem máquinas prontas no navegador, de graça. Não deixe o hardware virar desculpa.

---

## Montagem em 4 passos

### 1. Virtualizador
Escolha um: **VirtualBox** (gratuito, multiplataforma) ou **VMware Workstation Player** (gratuito para uso pessoal). Em Windows Pro, o **Hyper-V** já vem embutido.

### 2. As máquinas base

| VM | Para quê | Quando criar |
|---|---|---|
| **Linux (Ubuntu ou Debian)** | Estudo de SO, servidor alvo, ferramentas | Semana 4 |
| **Windows (avaliação)** | Estudo de SO, Event Viewer, PowerShell | Semana 6 |
| **Kali ou Parrot** | Ferramentas de análise e teste | Semana 3 (opcional) |
| **Windows Server** | Active Directory | Etapa 4, se seguir AD |

### 3. A rede do laboratório

> [!danger] Regra de ouro: seu lab é uma ilha
> Configure as VMs em **rede interna** ou **host-only**. Máquina vulnerável exposta à sua rede doméstica — ou à internet — é um problema real, não um exercício.

```
   [ Seu computador (host) ]
             │
   ┌─────────┴──────────┐
   │  Rede interna do lab │   ← isolada da sua rede doméstica
   └─────────┬──────────┘
     ┌───────┼────────┬────────────┐
   [Linux] [Windows] [Kali] [Alvo vulnerável]
```

### 4. Snapshots — o hábito que salva horas
Tire um snapshot **antes** de cada laboratório. Quebrou? Restaura em 30 segundos. Sem snapshot, cada erro custa uma reinstalação — e é aí que a desistência começa.

---

## Laboratório por etapa

### Etapa 1 · Redes → [[1️⃣ Etapa 1 - Redes]]
- Mapear a rede doméstica: quantos dispositivos, quais portas
- Capturar tráfego no Wireshark e identificar protocolos
- Comparar login em HTTP e HTTPS na captura
- Varrer a própria VM com Nmap e interpretar cada linha

### Etapa 2 · Sistemas → [[2️⃣ Etapa 2 - Sistemas Operacionais]]
- Instalar Linux e Windows do zero
- Criar usuários com permissões distintas e testar limites
- Documentar o **baseline** de uma máquina limpa
- Provocar eventos e localizá-los nos logs

### Etapa 3 · Fundamentos → [[3️⃣ Etapa 3 - Fundamentos de Segurança]]
- Dissecar um phishing real dos seus spams
- Experimento de hash e integridade
- Configurar MFA e documentar a mudança no fluxo
- Escrever a linha do tempo de um incidente público

### Etapa 4 · Por área → [[4️⃣ Etapa 4 - Especialização]]
Cada nota de área traz sua própria lista. Veja [[🧰 Projetos Práticos]].

---

## Plataformas online (complemento, não substituto)

Existem plataformas gratuitas com trilhas guiadas, máquinas vulneráveis e aplicações web propositalmente inseguras. São excelentes para começar sem infraestrutura.

**Mas monte o seu lab também.** Na plataforma, alguém já preparou tudo. No seu lab, você quebra, conserta e entende *por que* quebrou — e é isso que você vai fazer no trabalho.

---

## ⚖ Ética e legalidade — leia isto duas vezes

> [!danger] Sem autorização = crime
> No Brasil, invasão de dispositivo informático é crime tipificado. Não existe "eu só testei", não existe "era para ajudar", não existe "não causei dano".
>
> **Só teste:**
> - suas próprias máquinas e sua própria rede;
> - plataformas criadas para treino;
> - ambientes com **autorização formal e por escrito**.
>
> **Nunca teste:** o site da sua empresa (sem contrato), o sistema da sua faculdade, o Wi-Fi do vizinho, o app de alguém.
>
> Sua reputação na área leva anos para construir e um teste não autorizado para destruir.

---

## Como registrar cada sessão

Toda sessão de laboratório vira uma nota. Use [[🧫 Template - Sessão de Laboratório]].

Motivo: laboratório sem registro vira lembrança vaga em duas semanas. Com registro, vira portfólio → [[💼 Portfólio e Presença Profissional]].

---

## Checklist de montagem

- [ ] Virtualizador instalado
- [ ] VM Linux funcionando
- [ ] VM Windows funcionando
- [ ] Rede do lab isolada da rede doméstica
- [ ] Snapshots configurados
- [ ] Conta criada em uma plataforma de treino
- [ ] Primeira sessão registrada

---

**Relacionado:** [[🧰 Projetos Práticos]] · [[🔐 Ferramentas por Etapa]] · [[🧫 Template - Sessão de Laboratório]] · [[🗓 Semana Modelo]]
