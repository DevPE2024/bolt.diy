# 📋 Prioridades do Projeto Bolt.diy

## 🐳 Docker Compose - Configuração Prioritária

### Serviço a ser executado:
```bash
docker-compose up --build app-dev
```

**Justificativa:** O serviço `app-dev` é configurado para desenvolvimento com:
- Hot-reload habilitado
- Volumes mapeados para desenvolvimento em tempo real
- Porta 5173 exposta para acesso local
- Variáveis de ambiente configuradas para desenvolvimento

### Configuração atual:
- **Imagem:** `bolt-ai:development`
- **Container:** `boltdiy-app-dev-1`
- **URL Local:** http://localhost:5173/
- **URL Network:** http://172.20.0.2:5173/

---

## 🏢 Logo da Empresa

### Requisitos:
- [ ] **Implementar logo da empresa** na interface principal
- [ ] Posicionamento estratégico no header/navbar
- [ ] Versões para tema claro e escuro
- [ ] Formato SVG para melhor escalabilidade
- [ ] Responsividade em diferentes tamanhos de tela

### Localização dos assets:
```
public/
├── logo.svg
├── logo-dark.png
├── logo-light.png
├── logo-dark-styled.png
└── logo-light-styled.png
```

---

## 🤖 LiteLLM - Integração Prioritária

### Objetivos:
- [ ] **Configurar LiteLLM** como proxy unificado para múltiplas APIs de IA
- [ ] Simplificar gerenciamento de diferentes provedores (OpenAI, Anthropic, etc.)
- [ ] Implementar rate limiting e load balancing
- [ ] Monitoramento e logging centralizado

### APIs suportadas atualmente:
- GROQ_API_KEY
- OPENAI_API_KEY
- ANTHROPIC_API_KEY
- GOOGLE_GENERATIVE_AI_API_KEY
- HuggingFace_API_KEY
- TOGETHER_API_KEY
- OLLAMA_API_BASE_URL

### Benefícios esperados:
1. **Unificação:** Uma única interface para todas as APIs
2. **Fallback:** Redundância automática entre provedores
3. **Otimização:** Roteamento inteligente baseado em custo/performance
4. **Monitoramento:** Métricas centralizadas de uso e performance

---

## 🎯 Próximos Passos

1. **Imediato:**
   - Manter aplicação rodando via Docker
   - Verificar estabilidade do container

2. **Curto Prazo:**
   - Implementar logo da empresa
   - Configurar LiteLLM

3. **Médio Prazo:**
   - Otimizar performance da aplicação
   - Implementar testes automatizados

---

## 📝 Notas Técnicas

- **Ambiente:** Desenvolvimento (app-dev)
- **Framework:** Remix + Vite
- **Container Runtime:** Docker Desktop
- **Network:** boltdiy_default
- **Status:** ✅ Ativo e funcionando

---

*Última atualização: $(Get-Date -Format "dd/MM/yyyy HH:mm")*