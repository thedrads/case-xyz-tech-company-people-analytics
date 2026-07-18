# Case XYZ Tech Company — People Analytics

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-F9AB00?logo=googlecolab&logoColor=white)](https://colab.research.google.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Status](https://img.shields.io/badge/status-conclu%C3%ADdo-success)](#status-do-projeto)

Análise acadêmica de **People Analytics** aplicada ao processo de recrutamento e seleção da XYZ Tech Company. O projeto utiliza Python, pandas e visualizações para calcular indicadores, comparar cargos e propor ações gerenciais baseadas em dados.

## Visão geral

O case analisa 10 vagas distribuídas entre três cargos:

- Desenvolvedor Back-End;
- Analista de Dados;
- UX Designer.

As perguntas centrais são:

1. Qual é o tempo médio de contratação da empresa?
2. Qual é o percentual de vagas preenchidas dentro do prazo?
3. Qual cargo apresenta o menor tempo médio?
4. Qual cargo apresenta a maior taxa de atraso?
5. Que ações podem melhorar o cumprimento dos prazos sem comprometer a qualidade?

## Principais resultados

| Indicador | Resultado |
|---|---:|
| Tempo médio de contratação | **91,4 dias** |
| Vagas preenchidas dentro do prazo | **40%** |
| Vagas atrasadas | **60%** |
| Menor tempo médio | **Desenvolvedor Back-End — 64,33 dias** |
| Maior taxa de atraso | **Desenvolvedor Back-End — 100%** |
| Maior tempo médio | **UX Designer — 116,5 dias** |
| Melhor cumprimento do prazo | **Analista de Dados — 66,67%** |

O principal achado é que **velocidade e cumprimento de prazo são dimensões diferentes**. Desenvolvedor Back-End apresentou a menor duração média, mas todas as vagas ficaram atrasadas em relação ao planejamento.

## Estrutura do repositório

```text
.
├── .github/
│   ├── ISSUE_TEMPLATE/
│   ├── pull_request_template.md
│   └── workflows/
├── data/
│   └── processed/
│       └── resultados_case_xyz_tech_company.csv
├── docs/
│   └── metodologia.md
├── notebooks/
│   └── case_xyz_tech_company_people_analytics.ipynb
├── .gitignore
├── CITATION.cff
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
├── requirements.txt
└── SECURITY.md
```

## Como executar

### Google Colab

1. Abra o notebook em `notebooks/`.
2. Faça upload no Google Colab ou abra pelo GitHub.
3. Execute `Tempo de execução > Executar tudo`.
4. Confirme que todas as células finalizam sem erros.

### Ambiente local

```bash
git clone https://github.com/thedrads/case-xyz-tech-company-people-analytics.git
cd case-xyz-tech-company-people-analytics
python -m venv .venv
source .venv/bin/activate  # Linux/macOS
pip install -r requirements.txt
jupyter notebook
```

No Windows, ative o ambiente com:

```powershell
.venv\Scripts\activate
```

## Tecnologias

- Python 3.12;
- pandas;
- Matplotlib;
- Seaborn;
- Plotly;
- Google Colab;
- Jupyter Notebook.

## Metodologia

A análise segue as etapas:

1. transcrição e estruturação do dataset;
2. validação de qualidade dos dados;
3. conversão e validação de datas;
4. criação de variáveis derivadas;
5. cálculo de indicadores gerais e por cargo;
6. visualizações estáticas e interativas;
7. verificação independente dos cálculos;
8. interpretação gerencial e recomendações.

Detalhes adicionais estão em [`docs/metodologia.md`](docs/metodologia.md).

## Limitações

O dataset possui apenas 10 vagas e não contém informações sobre etapas do processo, candidatos, remuneração, recusas, senioridade, qualidade da contratação ou retenção. Assim, as causas dos resultados são apresentadas como hipóteses, não como conclusões causais.

## Status do projeto

**Concluído.** O notebook foi executado integralmente em uma sessão reiniciada do Google Colab, sem erros, e os principais resultados foram validados por método independente.

## Contexto acadêmico

Projeto desenvolvido para a disciplina **People Analytics e IA na Gestão de Talentos**, com base no Case XYZ Tech Company disponibilizado no material oficial da aula.

## Autor

**Fábio Ferreira de Andrade**  
GitHub: [@thedrads](https://github.com/thedrads)

## Licença

Distribuído sob a licença MIT. Consulte [`LICENSE`](LICENSE).