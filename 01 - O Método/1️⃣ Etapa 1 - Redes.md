---
titulo: Etapa 1 — Redes
tipo: conceito
etapa: 1
duracao: 3 semanas
tags:
  - tipo/conceito
  - etapa/redes
  - metodo
  - status/nao-iniciado
aliases:
  - Redes
  - Etapa 1
---

# 1️⃣ Etapa 1 — Redes

⬅ [[🧠 O Método Caminho Cyber]] · ➡ [[2️⃣ Etapa 2 - Sistemas Operacionais]]

> **Pergunta desta etapa:** *Como as máquinas conversam?*
> **Duração sugerida:** 3 semanas (~6–8h/semana)

---

## Por que começar aqui

Quase todo ataque e quase toda defesa passam por uma rede. Antes de usar Nmap, Wireshark, SIEM ou qualquer ferramenta de segurança, você precisa entender **o que a ferramenta está mostrando**.

---

## O que estudar

- [ ] modelo TCP/IP e noção do modelo OSI
- [ ] IPv4, máscara e gateway
- [ ] sub-redes em nível prático
- [ ] ARP
- [ ] TCP × UDP
- [ ] portas e serviços
- [ ] DNS
- [ ] DHCP
- [ ] roteamento básico
- [ ] NAT
- [ ] HTTP/HTTPS
- [ ] ICMP
- [ ] captura de pacotes

### Teste de domínio
Você deve conseguir olhar uma conexão e responder:

1. quem iniciou?
2. para qual IP?
3. em qual porta?
4. usando qual protocolo?
5. o DNS participou?
6. houve resposta?

---

## Comandos que você precisa reconhecer

### Windows
```powershell
ipconfig /all
route print
arp -a
nslookup example.com
netstat -ano
Test-NetConnection example.com -Port 443
```

### Linux
```bash
ip a
ip route
ip neigh
dig example.com
ss -tulpen
ping -c 4 example.com
traceroute example.com
```

### Captura
```bash
tcpdump -i any -n
```

ou Wireshark.

---

## 🧪 Laboratórios

1. descubra IP, máscara, gateway e DNS da sua máquina;
2. faça uma resolução DNS e identifique o IP retornado;
3. capture uma navegação HTTPS e localize handshake/conexão;
4. compare TCP e UDP em tráfego real;
5. desenhe sua rede doméstica.

Use [[🧫 Template - Sessão de Laboratório]].

---

## ✅ Critério de saída

Só avance quando você conseguir:

- explicar IP/máscara/gateway sem decorar definição;
- diferenciar TCP e UDP com exemplos;
- explicar porta como ponto de serviço;
- acompanhar uma resolução DNS;
- ler uma captura simples;
- interpretar uma saída de `netstat`/`ss`;
- explicar o caminho cliente → rede → servidor.

---

## ⛔ Não estude agora

- BGP avançado;
- MPLS;
- redes de operadora;
- SD-WAN profunda;
- certificação completa de fabricante;
- tuning avançado de roteadores.

Você está construindo fundação para segurança, não virando engenheiro de telecom.

---

## Conexões

- próximo: [[2️⃣ Etapa 2 - Sistemas Operacionais]]
- ferramentas: [[🔐 Ferramentas por Etapa]]
- prática: [[🧪 Laboratório em Casa]]
- plano: [[📅 Plano de 90 Dias]]
