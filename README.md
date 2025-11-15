# 🎭 Gerador de Poemas com IA e Feedback

Sistema educacional que gera poemas usando IA, permite feedback do usuário e refina automaticamente os prompts.

## 📁 Estrutura

```
gerador-de-poema/
├── sistema_gerador_poemas.ipynb    ⭐ NOTEBOOK PRINCIPAL
├── docs/                           (documentação)
├── requirements.txt
└── README.md
```

## 🚀 Quick Start

```bash
# 1. Instalar
pip install -r requirements.txt

# 2. Configurar API (opcional - funciona com demo)
$env:LLM_API_KEY = "sua_chave"

# 3. Executar
jupyter notebook notebooks/sistema_gerador_poemas.ipynb
```

## 📚 O Notebook tem 9 Seções

1. Título e Objetivos
2. Imports e Configuração
3. Modelo de Conversação (teoria)
4-5. Funções de IA (Grupo 1)
6. Feedback e Refinamento (Grupo 3)
7. Interface (Grupo 2)
8. Execuções Comentadas (Todos)
9. Notas para Relatório (Todos)

## 📖 Documentação

Veja a pasta `docs/` para:
- `INICIO_AQUI.md` - Guia completo de início
- `README_EXECUCOES.md` - Como documentar as execuções
- `TEMPLATE_RELATORIO.md` - Template do relatório
- `STATUS_FINAL.txt` - Checklist para entrega

## ✨ Funcionalidades

✅ Geração de poemas com IA  
✅ Novo Chat vs Chat Contínuo  
✅ Feedback e refinamento automático  
✅ Interface interativa (widgets)  
✅ Modo demo (sem API real)
- **Responsabilidades**:
  - Pesquisar e testar modelos gratuitos (OpenAI, HuggingFace, Cohere)
  - Implementar função `generate_poem(prompt, tipo) -> dict`
  - Configurar parâmetros ideais para cada tipo de poema
  - Sistema de fallback entre modelos

### Grupo 2: Interface do Usuário  
- **Arquivos**: `grupo2_interface/*.py`
- **Responsabilidades**:
  - Criar widgets interativos com ipywidgets
  - Implementar entrada de prompts e seleção de tipos
  - Exibir poemas de forma elegante
  - Coletar feedback do usuário (rating + comentários)
  - Controlar fluxo de interação

### Grupo 3: Sistema de Feedback
- **Arquivos**: `grupo3_feedback/*.py`  
- **Responsabilidades**:
  - Coletar e estruturar feedback
  - Analisar padrões nos comentários
  - Implementar algoritmos de melhoria de prompts
  - Manter histórico de evoluções
  - Métricas de qualidade

## 🔗 Como os Grupos se Integram

```
[Interface do Usuário] 
        ↓ prompt
[Grupo 1: Gerar Poema] 
        ↓ poema
[Interface: Mostrar + Coletar Feedback]
        ↓ feedback
[Grupo 3: Analisar e Melhorar Prompt]
        ↓ prompt melhorado
[Grupo 1: Gerar Novo Poema] → ciclo continua
```

**Arquivo Principal de Integração**: `notebooks/main_notebook.ipynb`
- Importa funções de todos os grupos
- Orquestra o fluxo completo
- Mantém estado da sessão
- Interface unificada

## 📦 Dependências Principais

- `jupyter` / `ipywidgets` - Interface interativa
- `requests` - Chamadas para APIs
- `pandas` - Manipulação de dados de feedback  
- `json` - Armazenamento de históricos
- `openai` / `transformers` - APIs de IA (conforme modelo escolhido)

## 📁 Dados Gerados

- `data/feedback_history.json` - Histórico de todos os feedbacks
- `data/prompt_history.json` - Evolução dos prompts
- `data/model_comparison.csv` - Comparação de modelos testados
- `data/session_data.json` - Dados da sessão atual

## 🎯 Entregáveis

1. **Sistema Funcional**: Notebook executável no Kaggle
2. **Execuções Comentadas**: 10+ exemplos com análises detalhadas
3. **Relatório Técnico**: Documentação completa em `docs/`
4. **Código Limpo**: Comentado e estruturado para fácil manutenção

## 🏃‍♂️ Próximos Passos

1. **Semana 1**: Cada grupo implementa seus módulos básicos
2. **Semana 2**: Integração inicial no notebook principal  
3. **Semana 3**: Testes, refinamento e documentação
4. **Entrega**: Sistema completo funcionando + relatório