# Metodologia da análise

## Objetivo

Avaliar a eficiência e o cumprimento de prazo do processo de recrutamento e seleção da XYZ Tech Company.

## Fonte dos dados

O dataset foi transcrito da tabela oficial do Case XYZ Tech Company, disponibilizada no material da disciplina. Cada linha representa uma vaga e contém:

- identificador da vaga;
- cargo;
- data de abertura;
- data esperada para contratação;
- data efetiva da contratação.

## Premissas

- Os intervalos são calculados em dias corridos.
- Uma vaga é classificada como dentro do prazo quando a contratação ocorre na data esperada ou antes.
- Cada vaga possui o mesmo peso nos cálculos.
- Explicações causais são tratadas como hipóteses quando não há variáveis suficientes para comprová-las.

## Regras de cálculo

### Tempo de contratação

```text
Data de contratação - Data de abertura
```

### Desvio do prazo

```text
Data de contratação - Data esperada
```

- resultado positivo: atraso;
- resultado igual a zero: contratação na data prevista;
- resultado negativo: antecipação.

### Percentual dentro do prazo

```text
Vagas dentro do prazo / Total de vagas × 100
```

### Taxa de atraso por cargo

```text
Vagas atrasadas do cargo / Total de vagas do cargo × 100
```

## Etapas executadas

1. Estruturação do dataset.
2. Verificação de valores ausentes, duplicidades e inconsistências.
3. Conversão explícita das datas para `datetime`.
4. Validação cronológica dos registros.
5. Criação das variáveis derivadas.
6. Cálculo dos indicadores gerais.
7. Agrupamento e comparação por cargo.
8. Construção de gráficos estáticos e interativos.
9. Recalculo independente dos indicadores.
10. Consolidação das respostas gerenciais.

## Limitações

O dataset possui apenas 10 vagas e três cargos. Não há informações sobre candidatos, etapas, senioridade, salários, recusas de proposta, aprovadores, desempenho ou retenção. Portanto, o projeto identifica padrões descritivos, mas não estabelece causalidade.

## Maturidade analítica

- **Descritiva:** mostra tempos, percentuais e atrasos.
- **Diagnóstica inicial:** identifica onde os problemas se concentram.
- **Prescritiva:** propõe ações de melhoria.
- **Preditiva:** não aplicada, devido ao volume e à variedade insuficientes de dados.
