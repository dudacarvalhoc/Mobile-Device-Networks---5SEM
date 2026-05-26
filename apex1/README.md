# 📡 APEX 1 — Projeto de Rede Wi-Fi Corporativa
 
**Disciplina:** Redes de Dispositivos Móveis
**Atividade:** APEX 1 — Individual
**Aluna:** Maria Eduarda de Carvalho Cortellini — RA `52420167`
**Ferramenta:** Cisco Packet Tracer
 
---
 
## 🎯 Objetivo
 
Projetar uma **rede Wi-Fi corporativa** segmentada por VLANs, com diferentes setores (Administrativo, Reuniões, Visitantes e IoT), aplicando boas práticas de **segurança, segmentação e escolha de canais wireless**.
 
---
 
## 🏗️ Arquitetura da rede
 
A rede foi estruturada com:
 
- **1 Roteador central** (Cisco 2911)
- **2 Switches** interligados em modo **trunk** (Cisco 2960)
- **Múltiplos Access Points** distribuídos pelos setores
- **Servidores dedicados** por VLAN
- **Dispositivos IoT** (sensores de movimento, fumaça e temperatura)
- **Dispositivos móveis** (smartphones e laptops)
---
 
## 📶 Configuração Wireless
 
| Item | Configuração | Justificativa |
|------|--------------|---------------|
| **Padrão principal** | 802.11n (2,4 GHz) | Maior alcance e compatibilidade |
| **Padrão alternativo** | 802.11ac (5 GHz) | Maior velocidade para reuniões |
| **Canais utilizados** | 1, 6 e 11 (2,4 GHz) | Não apresentam sobreposição entre si |
| **Tecnologia** | MIMO (Multiple Input Multiple Output) | Múltiplas antenas → maior taxa de transferência e confiabilidade |
 
---
 
## 🗂️ Segmentação por VLANs
 
| VLAN | Nome | Setor |
|------|------|-------|
| 🔵 **10** | Administrativo | PCs do setor administrativo |
| 🟢 **20** | Reuniões | Laptops da sala de reuniões |
| 🟡 **30** | Guest | Visitantes (smartphones) |
| 🟣 **40** | IoT | Sensores e dispositivos inteligentes |
 
A segmentação por VLANs melhora **desempenho, organização e segurança**, isolando o tráfego entre departamentos.
 
---
 
## 🔒 Segurança implementada
 
- 🔑 **WPA2** em todas as redes wireless
- 🚪 **Rede separada para visitantes** (VLAN 30)
- 🛡️ **ACL no roteador** bloqueando o acesso da VLAN Guest às VLANs internas
- 🧱 **Sub-interfaces no roteador** para roteamento entre VLANs
---
 
## 📡 Sobre a tecnologia MIMO
 
A tecnologia **MIMO (Multiple Input Multiple Output)** é utilizada em redes wireless modernas (802.11n/ac) e permite:
 
- 📈 Maior taxa de transferência
- 📶 Melhor confiabilidade do sinal
- ⚡ Eficiência no uso do espectro
- 🔁 Redução de perdas de pacote
- 🌐 Melhor desempenho com múltiplos dispositivos conectados
Essencial em redes corporativas como a proposta neste projeto.
 
---
 
## ⚠️ Problemas encontrados e soluções
 
| Problema | Solução |
|----------|---------|
| Configuração de VLANs | Ajustes nas configurações de **trunk** entre switches |
| Roteamento entre redes | Criação correta de **sub-interfaces no roteador** |
| Conexão wireless em laptops | Uso de **dispositivos móveis** (smartphones) para validação |
 
---
 
## 📦 Entregáveis
 
| Arquivo | Descrição |
|---------|-----------|
| 📄 `relatorio_final.pdf` | Relatório completo do projeto |
| 🌐 `projeto_rede_wifi.pkt` | Arquivo do Cisco Packet Tracer com a rede simulada |
 
---
 
## ▶️ Como abrir o projeto
 
1. Instale o [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
2. Abra o arquivo `projeto_rede_wifi.pkt`
3. Para testar a conectividade:
   - Use o modo de simulação para visualizar o tráfego entre VLANs
   - Teste pings entre dispositivos da mesma VLAN (deve funcionar)
   - Teste pings da VLAN Guest para VLANs internas (deve ser bloqueado pela ACL)
---
 
## 📁 Estrutura da pasta
 
```
apex1-redes-wifi-corporativa/
├── README.md
├── projeto_rede_wifi.pkt
└── docs/
    └── relatorio_final.pdf
```
