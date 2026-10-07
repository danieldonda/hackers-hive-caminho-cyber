---
titulo: Glossário
tipo: referencia
tags:
  - tipo/referencia
  - recurso
  - caminho-cyber
aliases:
  - Glossário
  - Termos
---

# 📖 Glossário

⬅ [[🏠 HOME - Caminho Cyber]]

---

O vocabulário mínimo. Cada termo traz a etapa em que ele aparece — use isso para saber se você precisa dele **agora**.

---

## 🌐 Redes — `#etapa/redes`
> Nota completa: [[1️⃣ Etapa 1 - Redes]]

| Termo | Definição |
|---|---|
| **Endereço IP** | Identificador de um dispositivo em uma rede. Público (visível na internet) ou privado (interno). |
| **Máscara de rede** | Define qual parte do IP é rede e qual é host. É o que separa "vizinhos" de "estrangeiros". |
| **Porta** | Número que identifica um serviço em um host. 80 = HTTP, 443 = HTTPS, 22 = SSH. |
| **TCP** | Protocolo confiável e orientado a conexão. Confirma entrega. |
| **UDP** | Protocolo rápido e sem garantia. Não confirma nada. |
| **Handshake de 3 vias** | SYN → SYN-ACK → ACK. Como uma conexão TCP começa. |
| **DNS** | Traduz nome (site.com) em IP. Alvo frequente de ataque. |
| **DHCP** | Distribui IPs automaticamente na rede. |
| **NAT** | Traduz endereços privados em um público. É por isso que sua casa inteira sai com um IP só. |
| **Gateway** | A porta de saída da sua rede para outras redes. |
| **Firewall** | Filtra tráfego conforme regras. |
| **Proxy** | Intermediário entre cliente e servidor. |
| **VPN** | Túnel criptografado sobre rede não confiável. |
| **TLS** | Protocolo que criptografa o tráfego. O "S" do HTTPS. |
| **Pacote** | A unidade de dado que trafega na rede. |

---

## 💻 Sistemas — `#etapa/sistemas`
> Nota completa: [[2️⃣ Etapa 2 - Sistemas Operacionais]]

| Termo | Definição |
|---|---|
| **Processo** | Programa em execução. Tem PID e processo pai. |
| **Serviço / daemon** | Processo que roda em segundo plano, geralmente desde o boot. |
| **Permissão** | Quem pode ler, escrever ou executar. `rwx` no Linux, ACL no Windows. |
| **SUID** | Bit que faz um programa executar com o privilégio do dono. Alvo clássico de escalação. |
| **Registro do Windows** | Banco hierárquico de configuração. Onde malware costuma criar persistência. |
| **Event Viewer** | Visualizador de logs do Windows. A principal fonte de evidência. |
| **Active Directory** | Serviço de diretório da Microsoft. O coração da rede corporativa. |
| **GPO** | Política de grupo. Aplica configuração em massa no domínio. |
| **Baseline** | O retrato do que é normal em um sistema. Sem ele, nada parece anormal. |
| **Persistência** | Mecanismo que garante que o atacante volte após reinicialização. |
| **Escalação de privilégio** | Sair de usuário comum para administrador/root. |
| **Sysmon** | Ferramenta que amplia enormemente a telemetria do Windows. |

---

## 🔐 Segurança — `#etapa/fundamentos`
> Nota completa: [[3️⃣ Etapa 3 - Fundamentos de Segurança]]

| Termo | Definição |
|---|---|
| **CIA** | Confidencialidade, Integridade, Disponibilidade. Os três pilares. |
| **Ameaça** | Algo que pode causar dano (um ransomware, um insider). |
| **Vulnerabilidade** | A fraqueza que a ameaça explora (senha fraca, sistema sem patch). |
| **Risco** | A combinação: probabilidade × impacto. É o que se prioriza. |
| **Ativo** | O que tem valor e precisa ser protegido. |
| **Superfície de ataque** | Todos os pontos por onde se pode entrar. |
| **AAA** | Autenticação (quem é você), Autorização (o que pode fazer), Contabilização (o que fez). |
| **MFA** | Múltiplos fatores de autenticação. Quebra a maioria dos ataques de credencial. |
| **Menor privilégio** | Cada um tem só o acesso necessário. O controle mais barato e mais ignorado. |
| **Hash** | Função de mão única. Verifica integridade e guarda senha. **Não é criptografia.** |
| **Criptografia simétrica** | Mesma chave para cifrar e decifrar. Rápida. |
| **Criptografia assimétrica** | Par de chaves: pública e privada. Base dos certificados. |
| **Certificado digital** | Documento que vincula uma identidade a uma chave pública. |
| **IOC** | Indicador de comprometimento. Um rastro do ataque (hash, IP, domínio). |
| **IOA** | Indicador de ataque. Um comportamento em curso. |
| **MITRE ATT&CK** | Catálogo de táticas e técnicas de adversários. A linguagem comum da defesa. |
| **Kill Chain** | Modelo das fases de um ataque, do reconhecimento à ação final. |
| **Defesa em profundidade** | Múltiplas camadas — porque uma sempre falha. |
| **Zero Trust** | "Nunca confie, sempre verifique." Não existe rede interna confiável. |

---

## 🦠 Ameaças

| Termo | Definição |
|---|---|
| **Malware** | Software malicioso — termo guarda-chuva. |
| **Ransomware** | Cifra os dados e cobra resgate. |
| **Trojan** | Se disfarça de programa legítimo. |
| **Worm** | Se propaga sozinho pela rede. |
| **Infostealer** | Rouba credenciais e dados do navegador. |
| **RAT** | Ferramenta de acesso remoto usada por atacante. |
| **Phishing** | Engano por mensagem para obter credencial ou execução. |
| **Engenharia social** | Manipular pessoas em vez de sistemas. |
| **C2** | Command and Control. A infraestrutura que comanda a máquina comprometida. |
| **Exfiltração** | Retirada não autorizada de dados. |
| **Zero-day** | Vulnerabilidade sem correção disponível. |
| **Força bruta** | Tentar credenciais até acertar. |
| **Credential stuffing** | Reusar credenciais vazadas em outros serviços. |

---

## 🏢 Operação e carreira

| Termo | Definição |
|---|---|
| **SOC** | Centro de operações de segurança. Monitora e responde. → [[🛡 SOC - Blue Team]] |
| **SIEM** | Plataforma que centraliza logs e correlaciona eventos. |
| **EDR / XDR** | Detecção e resposta em endpoint (e além dele). |
| **DFIR** | Forense digital e resposta a incidentes. → [[🔬 DFIR - Forense e Resposta a Incidentes]] |
| **Threat Hunting** | Busca proativa por ameaças sem alerta. → [[🎯 Threat Hunting]] |
| **Pentest** | Teste de intrusão autorizado. → [[⚔ Pentest - Red Team]] |
| **Red Team / Blue Team / Purple Team** | Ataque / defesa / os dois colaborando. |
| **GRC** | Governança, risco e conformidade. → [[📋 GRC - Governança, Risco e Conformidade]] |
| **CVE** | Identificador público de uma vulnerabilidade conhecida. |
| **CVSS** | Pontuação de severidade de uma vulnerabilidade (0 a 10). |
| **LGPD** | Lei Geral de Proteção de Dados Pessoais. |
| **Falso positivo** | Alerta que não era ataque. A maior parte do trabalho de um SOC. |
| **Falso negativo** | Ataque que não gerou alerta. O que tira o sono. |
| **Triagem** | Decidir rapidamente o que merece investigação. |

---

## Adicione os seus

| Termo | Onde encontrei | Minha definição |
|---|---|---|
|  |  |  |
|  |  |  |

> [!tip] Como usar o glossário para estudar
> Cubra a coluna da direita e explique cada termo em voz alta. O que você não conseguir explicar, marque com `#duvida` e resolva na revisão de domingo.

---

**Relacionado:** [[🧠 O Método Caminho Cyber]] · [[🔐 Ferramentas por Etapa]] · [[🌐 Fontes Confiáveis]] · [[🏷 Mapa de Tags]]
