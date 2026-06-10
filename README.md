# amt01-squad2i ..> DATArd's 
Dashboard de Atrasos de Entregas - Armazenamento, Manipulação e Transformação de Dados

# 📦 Logistics Monitor Dashboard

Dashboard interativo para monitoramento de atrasos em entregas logísticas, desenvolvido para auxiliar gestores na identificação rápida de transportadoras problemáticas, regiões críticas e priorização de ações operacionais.

## 🎯 Propósito

Substituir planilhas extensas e relatórios manuais por uma ferramenta visual e intuitiva que permita:

- Identificar transportadoras com maior índice de atraso
- Visualizar regiões críticas do país
- Priorizar entregas mais problemáticas
- Acompanhar tendências operacionais
- Tomar decisões baseadas em dados em tempo real

## 🚀 Funcionalidades

- **Filtros dinâmicos**: por região, transportadora e busca textual
- **KPIs atualizados automaticamente**: total de entregas, atrasos, taxa de atraso e maior atraso
- **Gráficos interativos**:
  - Polar area: distribuição de atrasos por transportadora
  - Radar: comparação de atrasos entre regiões
  - Barras horizontais: ranking das 5 entregas mais críticas
  - Doughnut: proporção de entregas no prazo vs atrasadas
- **Tabela detalhada**: ordenada por maior atraso, com clique para detalhes
- **Insights automáticos**: análise textual descritiva baseada nos filtros aplicados
- **Modais explicativos**: cada gráfico e card possui explicação contextual

## 🛠️ Tecnologias utilizadas

- HTML5 + CSS3
- JavaScript (Vanilla)
- Chart.js

## 📊 Fonte de dados

Dataset fixo com 10 entregas distribuídas pelas regiões brasileiras, contendo:

- ID da entrega
- Cidade e região
- Transportadora responsável
- Prazo previsto (dias)
- Dias reais de entrega

Os cálculos de atraso, taxas e rankings são derivados exclusivamente desses dados.

## 🔍 Lógica de negócio

| Conceito | Descrição |
|----------|-----------|
| **Atraso** | `max(0, diasReais - prazo)` |
| **Taxa de atraso** | `(entregas com atraso / total de entregas) × 100` |
| **Priorização** | Ordenação decrescente por dias de atraso |
| **Ranking crítico** | Top 5 entregas com maior atraso |

## 🧪 Como executar localmente

1. Clone o repositório:

git clone https://github.com/yurijara97-cloud/amt01-squad2i.git
Acesse a pasta do projeto:

bash
cd amt01-squad2i
Abra o arquivo index.html em qualquer navegador moderno.

⚠️ Não é necessário servidor local ou dependências adicionais.

📁 Estrutura do projeto
text
/
├── index.html          # Estrutura principal do dashboard com <java script> incluso no html   # Lógica de negócio, gráficos e interatividade
├── estilo.css          # Estilos e layout responsivo
└── README.md           # Documentação do projeto
📸 Preview visual
Dashboard com layout clean e cartões coloridos

Filtros expansivos e responsivos

Gráficos interativos com tooltips e cliques

Tabela com status colorido (verde, laranja, vermelho)

🧠 Possíveis evoluções
Conexão com API real para dados dinâmicos

Exportação de relatórios (CSV/PDF)

Comparação entre períodos (mês a mês)

Gráfico de evolução temporal de atrasos

Alertas automáticos para transportadoras críticas

👥 Público-alvo
Gestores logísticos, analistas de operações e tomadores de decisão que precisam de visibilidade rápida sobre a performance de entregas.


