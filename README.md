# 🏗️ **AGENTE CAD - Sistema de Análise Inteligente de Arquivos DXF**

## 📋 **VISÃO GERAL**

O **Agente CAD** é um sistema avançado de análise inteligente de arquivos DXF que utiliza Inteligência Artificial para identificar, classificar e processar elementos estruturais em projetos de engenharia civil.

### 🎯 **Principais Funcionalidades**

- **🔍 Análise Automática de DXF** - Identificação inteligente de elementos estruturais
- **🤖 IA Integrada** - Processamento com Gemini e modelos especializados
- **📊 Hierarquia Infinita** - Sistema de categorias escalável e flexível
- **🐳 Docker Ready** - Ambiente containerizado para desenvolvimento e produção
- **🔄 CI/CD Automatizado** - Pipeline completo de integração e deploy

---

## 🏗️ **ARQUITETURA DO SISTEMA**

### **Componentes Principais**

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   MCP Server    │    │   Database      │
│   (React/Vite)  │◄──►│   (Python)      │◄──►│   (Supabase)    │
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

### **Tecnologias Utilizadas**

- **Frontend:** React 18 + TypeScript + Vite
- **Backend:** Python FastAPI + MCP Protocol
- **Database:** PostgreSQL (Supabase)
- **IA:** Google Gemini + Modelos Especializados
- **Containerização:** Docker + Docker Compose
- **CI/CD:** GitHub Actions

---

## 🚀 **INSTALAÇÃO RÁPIDA**

### **1. Clone o Repositório**
```bash
git clone https://github.com/tititasf/AGENTE.CAD.git
cd AGENTE.CAD
```

### **2. Iniciar com Docker (Recomendado)**
```bash
# Windows
.\scripts\docker-dev.ps1 start

# Linux/Mac
./scripts/docker-dev.sh start
```

### **3. Acessar a Aplicação**
- **Aplicação Principal:** http://localhost:3000
- **Vite Dev Server:** http://localhost:5173
- **MCP Server:** http://localhost:3001
- **Nginx Proxy:** http://localhost:80

---

## 🐳 **SISTEMA DOCKER**

### **Comandos Principais**

```bash
# Iniciar ambiente
.\scripts\docker-dev.ps1 start

# Ver logs
.\scripts\docker-dev.ps1 logs

# Parar ambiente
.\scripts\docker-dev.ps1 stop

# Acessar shell
.\scripts\docker-dev.ps1 shell
```

### **Estrutura de Containers**

- **MCP Server** (Porta 3001) - Servidor de IA e processamento
- **Aplicação Principal** (Porta 3000) - Interface React
- **Nginx Proxy** (Porta 80) - Proxy reverso

---

## 🧠 **SISTEMA DE IA**

### **Modelos Integrados**

- **Gemini Pro** - Análise geral de arquivos DXF
- **Modelos Especializados** - Categorização por tipo de elemento
- **Sistema Hierárquico** - Categorias infinitas e flexíveis

### **Capacidades de IA**

- ✅ Identificação automática de pilares, vigas e lajes
- ✅ Classificação por tipo estrutural
- ✅ Análise de dimensões e propriedades
- ✅ Geração de relatórios inteligentes
- ✅ Sugestões de otimização

---

## 📊 **SISTEMA HIERÁRQUICO**

### **Arquitetura de Categorias**

```
NÍVEL 1: Estruturas Principais
├── NÍVEL 2: Pilares
│   ├── NÍVEL 3: Pilares Retangulares
│   └── NÍVEL 3: Pilares Circulares
├── NÍVEL 2: Vigas
│   ├── NÍVEL 3: Vigas Principais
│   └── NÍVEL 3: Vigas Secundárias
└── NÍVEL 2: Lajes
    ├── NÍVEL 3: Lajes Maciças
    └── NÍVEL 3: Lajes Nervuradas
```

### **Características**

- **Escalabilidade Infinita** - Níveis ilimitados
- **Isolamento Completo** - Cada categoria tem sua própria tabela
- **Flexibilidade Total** - Configuração independente por categoria
- **Performance Otimizada** - Consultas diretas por categoria

---

## 🔧 **DESENVOLVIMENTO**

### **Estrutura do Projeto**

```
agente-cad/
├── components/          # Componentes React
├── services/           # Serviços de API
├── hooks/             # Custom hooks
├── contexts/          # Contextos React
├── database/          # Scripts SQL e migrações
├── scripts/           # Scripts de automação
├── deploy/            # Configurações de deploy
├── docs/              # Documentação
└── test_data/         # Dados de teste
```

### **Comandos de Desenvolvimento**

```bash
# Instalar dependências
npm install

# Executar em desenvolvimento
npm run dev

# Executar testes
npm test

# Build para produção
npm run build
```

---

## 🧪 **TESTES**

### **Executar Testes**

```bash
# Testes unitários
npm test

# Testes de integração
npm run test:integration

# Testes E2E
npm run test:e2e
```

### **Cobertura de Testes**

- ✅ Testes unitários para componentes React
- ✅ Testes de integração para APIs
- ✅ Testes E2E para fluxos completos
- ✅ Testes de performance

---

## 🚀 **DEPLOY**

### **Ambiente de Desenvolvimento**

```bash
# Iniciar com Docker
.\scripts\docker-dev.ps1 start

# Ou manualmente
npm run dev
```

### **Ambiente de Produção**

```bash
# Deploy com Docker
docker-compose -f docker-compose.prod.yml up -d

# Ou build manual
npm run build
npm start
```

---

## 📈 **MONITORAMENTO**

### **Logs e Métricas**

- **Logs Estruturados** - Sistema de logging avançado
- **Métricas de Performance** - Monitoramento em tempo real
- **Alertas Automáticos** - Notificações de problemas
- **Dashboard de Saúde** - Interface de monitoramento

### **Health Checks**

```bash
# Verificar saúde da aplicação
curl http://localhost:3000/health

# Verificar saúde do MCP
curl http://localhost:3001/health
```

---

## 🔒 **SEGURANÇA**

### **Medidas Implementadas**

- ✅ **Autenticação JWT** - Tokens seguros
- ✅ **Validação de Entrada** - Sanitização de dados
- ✅ **HTTPS Forçado** - Comunicação criptografada
- ✅ **Rate Limiting** - Proteção contra ataques
- ✅ **Logs de Auditoria** - Rastreamento de ações

---

## 🤝 **CONTRIBUIÇÃO**

### **Como Contribuir**

1. **Fork o projeto**
2. **Crie uma branch** (`git checkout -b feature/nova-funcionalidade`)
3. **Commit suas mudanças** (`git commit -am 'Adiciona nova funcionalidade'`)
4. **Push para a branch** (`git push origin feature/nova-funcionalidade`)
5. **Abra um Pull Request**

### **Padrões de Código**

- **TypeScript** - Tipagem forte
- **ESLint** - Linting automático
- **Prettier** - Formatação consistente
- **Husky** - Hooks de pre-commit

---

## 📚 **DOCUMENTAÇÃO**

### **Documentos Disponíveis**

- [📋 Documentação Técnica](docs/DOCUMENTO_TECNICO_COMPLETO.md)
- [🐳 Guia Docker](DOCKER_README.md)
- [🏗️ Arquitetura do Banco](docs/ARQUITETURA_BANCO_HIERARQUICO.md)
- [🔄 Sistema de Refresh](REFRESH_AUTOMATICO_README.md)

---

## 🐛 **TROUBLESHOOTING**

### **Problemas Comuns**

#### **Docker não inicia**
```bash
# Verificar se Docker está rodando
docker info

# Reiniciar Docker Desktop
# Windows: Docker Desktop > Restart
# Linux: sudo systemctl restart docker
```

#### **Portas já em uso**
```bash
# Verificar portas
netstat -tulpn | grep :3000
netstat -tulpn | grep :3001

# Parar serviços conflitantes
# Ou alterar portas no docker-compose.dev.yml
```

#### **Erro de dependências**
```bash
# Limpar cache
npm cache clean --force

# Reinstalar dependências
rm -rf node_modules package-lock.json
npm install
```

---

## 📞 **SUPORTE**

### **Canais de Ajuda**

- **Issues GitHub** - [Reportar bugs](https://github.com/tititasf/AGENTE.CAD/issues)
- **Discussions** - [Discussões e dúvidas](https://github.com/tititasf/AGENTE.CAD/discussions)
- **Documentação** - [Guia completo](docs/)

---

## 📄 **LICENÇA**

Este projeto está licenciado sob a **MIT License** - veja o arquivo [LICENSE](LICENSE) para detalhes.

---

## 🎉 **AGRADECIMENTOS**

- **Google Gemini** - Pelo poder de IA
- **Supabase** - Pela infraestrutura de banco
- **React Team** - Pela excelente framework
- **Docker** - Pela containerização

---

**Desenvolvido com ❤️ pela equipe Agente CAD**

*Versão: 1.0.0 | Última atualização: 04/08/2025*