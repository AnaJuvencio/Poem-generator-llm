# Gerador de Poemas com IA e Feedback

Sistema completo de geração de poemas usando IA com interface Gradio moderna e sistema avançado de feedback inteligente.

## Estrutura Atualizada

```
Poem-generator-llm/
├── notebooks/
│   └── sistema_gerador_poemas.ipynb    
├── docs/                               
├── requirements.txt
└── README.md
```

## Sistema Integrado Completo

**Arquivo Principal:** `notebooks/sistema_gerador_poemas.ipynb`

### Funcionalidades Implementadas:

**Grupo 1 - Integração com IA**
- API Google Gemini 2.5 Pro integrada
- Geração de poemas personalizados
- Controle de criatividade e temperatura
- Sistema de chat contínuo vs novo chat

**Grupo 2 - Interface Moderna** 
- Interface Gradio responsiva e elegante
- Coleta estruturada de refinamentos
- Sistema de abas intuitivo
- CSS personalizado e UX otimizada

**Grupo 3 - Sistema Avançado de Feedback**
- **7 funções especializadas** implementadas:
  1. `validar_refinamento()` - Validação inteligente
  2. `detectar_conflitos()` - Detecção automática de conflitos
  3. `priorizar_refinamentos()` - Ordem otimizada (Remover → Editar → Adicionar)
  4. `gerar_prompt_refinamento()` - Templates especializados
  5. `avaliar_refinamento()` - Avaliação automática de resultados
  6. `sugerir_refinamentos()` - Sugestões inteligentes
  7. `processar_refinamentos()` - Pipeline completo integrado

## Fluxo de Integração Otimizado

```
[Usuário insere tema e configurações]
        ↓
[Sistema gera poema via Gemini API]
        ↓
[Interface exibe resultado + opções de refinamento]
        ↓ (se refinamentos solicitados)
[Sistema Avançado do Grupo 3]:
  • Valida refinamentos
  • Detecta conflitos
  • Prioriza ordem (Remover → Editar → Adicionar)
  • Gera prompts especializados
  • Aplica refinamentos
  • Avalia resultados
        ↓
[Poema refinado apresentado ao usuário]
```

## Tecnologias Utilizadas

- **Frontend**: Gradio 5.40.0 (interface web moderna)
- **IA**: Google Gemini 2.5 Pro API
- **Backend**: Python com processamento inteligente
- **Análise**: difflib, collections.Counter para métricas
- **Ambiente**: Jupyter Notebooks

## Documentação Completa

Consulte a pasta `docs/` para:
- `TEMPLATE_RELATORIO.md` - Template para relatório final
- `README_EXECUCOES.md` - Como documentar execuções
- `SUMARIO_VISUAL.txt` - Visão geral completa do projeto

## Como Usar o Sistema

### **Geração Básica:**
1. Execute o notebook `sistema_gerador_poemas.ipynb`
2. Digite um tema na interface Gradio
3. Configure estilo, tamanho e criatividade
4. Clique "Gerar Poema"

### **Refinamentos Avançados:**
1. Após gerar um poema, clique "Adicionar Refinamentos"
2. Para cada refinamento:
   - **Ação**: Adicionar, Editar ou Remover
   - **Alvo**: Especifique a parte (ex: "primeira estrofe")
   - **Novo Conteúdo**: Texto de substituição
3. Clique "Aplicar Refinamentos"
4. O sistema automaticamente:
   - Valida se o alvo existe
   - Detecta conflitos entre refinamentos
   - Aplica na ordem otimizada
   - Avalia se funcionou corretamente

## Dependências

Ver `requirements.txt` para lista completa:
- `gradio==5.40.0` - Interface web moderna
- `google-genai` - API Google Gemini
- `difflib` - Análise de diferenças para avaliação
- `collections` - Contadores para análise de texto

## Características Avançadas

### **Sistema de Validação Inteligente**
- Verifica se alvos de refinamento existem no poema
- Detecta refinamentos contraditórios automaticamente
- Sugere resoluções para conflitos encontrados

### **Templates Especializados**
- Prompts otimizados para cada tipo de refinamento
- Instruções específicas para preservar estilo original
- Máxima efetividade na aplicação de mudanças

### **Avaliação Automática**
- Métricas de sucesso por tipo de operação
- Análise de diferenças antes/depois
- Feedback em tempo real sobre efetividade

### **Interface Responsiva**
- Design moderno com CSS personalizado
- Sistema de abas intuitivo
- Estados visuais claros para cada etapa

## 🎯 Status do Projeto

✅ **SISTEMA COMPLETO E FUNCIONAL**
- ✅ Integração API Gemini configurada
- ✅ Interface Gradio moderna implementada
- ✅ Sistema avançado de feedback (7 funções)
- ✅ Pipeline completo de refinamentos
- ✅ Validação e detecção de conflitos
- ✅ Templates especializados por tipo
- ✅ Avaliação automática de resultados
- ✅ Documentação completa


**Desenvolvido por:** Grupos 1, 2 e 3  
**Tecnologia Principal:** Google Gemini 2.5 Pro + Gradio  
**Status:** Pronto para uso e demonstração