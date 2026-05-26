# 📶 Atividade 08 — Estudo de Caso: Rede Wi-Fi Corporativa
 
**Disciplina:** Redes de Dispositivos Móveis
**Aula:** 8 — Estudo de Caso
**Grupo:** CTRL + ALT + DELAS
**Ferramenta:** Cisco Packet Tracer
 
## 👥 Integrantes
 
| Nome | RA |
|------|-----|
| Beatriz Antunes | 52420663 |
| Daniele Tavares | 52420099 |
| Giovanna Fogaça | 52421068 |
| Karen Arwen | 52420075 |
| Luiz Franzon | 52421183 |
| Maria Eduarda Cortellini | 52420167 |
 
---
 
## 🏢 Contexto
 
Planejamento de uma rede Wi-Fi corporativa para a empresa fictícia **Connect Corp Soluções Empresariais**, que atende cerca de **600 pessoas por dia** entre colaboradores, clientes e visitantes.
 
### Ambientes da empresa
 
- 🛎️ Recepção
- 💼 Escritórios administrativos
- 🤝 Salas de reunião
- 🎤 Auditório principal (até 200 pessoas)
- ☕ Área de convivência
---
 
## 🎯 Objetivo
 
Projetar uma rede Wi-Fi corporativa baseada no padrão **Wi-Fi 6 (802.11ax)** que ofereça:
 
- 🚀 Alta capacidade de conexões simultâneas
- 📡 Cobertura completa em todos os ambientes
- 🔄 Mobilidade entre áreas (roaming)
- 🔒 Segurança para usuários internos e visitantes
- ⚖️ Estabilidade e bom desempenho
---
 
## 👥 Perfil de usuários
 
Estimativa de **440 usuários simultâneos** em pico de uso, distribuídos assim:
 
| Ambiente | Usuários | Dispositivos predominantes |
|----------|----------|----------------------------|
| Recepção | 30 | 📱 Smartphones |
| Escritórios administrativos | 120 | 💻 Notebooks |
| Salas de reunião | 50 | 💻 Notebooks |
| Auditório principal | 200 | 📱 Smartphones |
| Área de convivência | 40 | 📱 Smartphones |
| **Total** | **440** | |
 
---
 
## 📡 Planejamento de Access Points
 
**Total: 11 APs** distribuídos estrategicamente conforme densidade de usuários:
 
| Ambiente | Quantidade de APs | Justificativa |
|----------|-------------------|---------------|
| Recepção | 1 | Baixa densidade de usuários |
| Escritórios administrativos | 2 | Um para cada escritório |
| Salas de reunião | 2 | Uma para cada sala |
| **Auditório principal** | **5** | **Alta densidade — 200 usuários** |
| Área de convivência | 1 | Uso esporádico |
 
### 🎯 Estratégia de cobertura
- Distribuição baseada nas áreas de maior concentração
- Evita zonas de sombra
- **Sobreposição moderada** de sinal para permitir roaming sem interferências excessivas
---
 
## 🔧 Tecnologias e padrões
 
### Wi-Fi 6 (802.11ax)
 
| Benefício | O que entrega |
|-----------|---------------|
| 🚀 Alta capacidade | Suporte a muitos dispositivos simultâneos |
| ⚡ Baixa latência | Ideal para videoconferências |
| 📈 Melhor desempenho | Eficiente em ambientes densos como o auditório |
| 🎛️ Gerenciamento de dispositivos | Múltiplas conexões sem perda de qualidade |
 
---
 
## 💼 Necessidades atendidas
 
A rede suportará:
- 🌐 Navegação na internet
- 🏢 Acesso a sistemas internos
- 📧 E-mails
- 🎥 Videoconferências
- 📁 Compartilhamento de arquivos
- 📺 Streaming em eventos e apresentações
---
 
## 🔒 Segurança — Duas redes separadas
 
### 🏢 Rede Corporativa
- Uso exclusivo de colaboradores
- Autenticação **WPA3**
- Acesso a sistemas internos
### 👥 Rede de Visitantes
- Apenas internet
- **Isolada** da rede corporativa
- Controle de acesso simplificado
---
 
## 🏗️ Infraestrutura
 
- 1 roteador principal
- Switches de distribuição
- 11 access points
- Dispositivos clientes via Wi-Fi
- Organização por setores no Cisco Packet Tracer
---
 
## 🔄 Mobilidade e Roaming
 
A rede foi planejada para garantir **transição de conexão sem interrupções perceptíveis** entre os APs, com **sobreposição controlada de sinal** que permite roaming eficiente entre os ambientes.
 
---
 
## 📦 Entregáveis
 
| Arquivo | Descrição |
|---------|-----------|
| 📄 `estudo_de_caso.pdf` | Documento completo do estudo de caso |
| 🌐 `projeto_rede_corporativa.pkt` | Simulação no Cisco Packet Tracer |
 
---
 
## ▶️ Como abrir o projeto
 
1. Instale o [Cisco Packet Tracer](https://www.netacad.com/courses/packet-tracer)
2. Abra o arquivo `.pkt`
3. Explore a topologia organizada por setores
---
 
## 📁 Estrutura da pasta
 
```
atividade-08-rede-corporativa-wifi6/
├── README.md
├── projeto_rede_corporativa.pkt
└── docs/
    └── estudo_de_caso.pdf
```
