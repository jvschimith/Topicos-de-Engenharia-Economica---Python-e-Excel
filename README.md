# Engenharia Econômica com Python e Excel

**Modelos financeiros explicados, calculados e comparados em notebooks Jupyter e planilhas.**

Este repositório reúne estudos aplicados de Engenharia Econômica desenvolvidos durante a graduação em Ciência da Computação na UNESP. Cada tema combina premissas explícitas, fórmulas, tabelas e interpretação dos resultados. O objetivo é mostrar como transformar uma questão quantitativa em uma decisão justificável: comparar financiamentos, avaliar investimentos e descobrir quais mudanças tornam um projeto inviável.

> **Escopo:** exercícios e cenários didáticos. Os valores não representam recomendações de investimento ou crédito nem resultados de uma empresa real.

## Comece por uma decisão

| Pergunta | Método | Onde ver | Exemplo de conclusão |
| --- | --- | --- | --- |
| Qual sistema reduz a primeira parcela de um financiamento? | Comparação entre Price e SAC | [Aula 5: notebook](Aula_5_Sistemas_de_Amortizacao.ipynb) · [planilha](Aula_5_Sistemas_de_Amortizacao.xlsx) | No cenário do exercício 6, Price reduz o desembolso inicial; SAC amortiza o principal mais rapidamente. |
| Um investimento cobre a taxa mínima exigida? | VPL, TIR, payback e CAUE | [Aula 6: notebook](Aula_6_Analise_de_Investimentos.ipynb) · [planilha](Aula_6_Analise_de_Investimentos.xlsx) | No exercício 1, a reforma tem VPL aproximado de R$ 4.071,64 para uma TMA de 12% a.a. |
| O que acontece se as premissas mudarem? | Sensibilidade, ponto de equilíbrio e cenários | [Aula 7: notebook](Aula_7_Analise_de_Sensibilidade_e_Risco.ipynb) · [planilha](Aula_7_Analise_de_Sensibilidade_e_Risco.xlsx) | No exercício 5, a escolha entre empilhadeiras muda em cerca de 527,60 horas de uso por ano. |

## Conteúdo

### 1. Sistemas de amortização · Aula 5

Construção e leitura de cronogramas de pagamento, com separação de **juros, amortização, prestação e saldo devedor**. Inclui pagamento único, Sistema Americano, Tabela Price e SAC, além de uma comparação orientada por critério de decisão. São seis exercícios resolvidos.

**Aplicação:** projeção de desembolsos, análise de endividamento e distinção entre pagamento do principal e custo financeiro.

### 2. Análise de investimentos · Aula 6

Avaliação de alternativas com **Valor Presente Líquido (VPL), Taxa Interna de Retorno (TIR), TIR incremental, payback simples e descontado e Custo Anual Uniforme Equivalente (CAUE)**. Os nove exercícios incluem comparação de softwares, escolha entre materiais com vidas úteis diferentes, franquia com valor residual e momento de substituição de um caminhão.

**Aplicação:** comparar projetos com fluxos de caixa distintos, explicitar a TMA e relacionar o resultado numérico à decisão.

### 3. Sensibilidade e risco · Aula 7

Exploração de **ponto de equilíbrio, lucro-alvo, mudanças de receita e investimento, vida útil mínima, ponto de indiferença, taxa de Fisher, valor esperado do VPL e alavancagem financeira**. Há oito exercícios resolvidos e um cenário adicional com probabilidades.

**Aplicação:** localizar limites operacionais e testar o quanto uma conclusão depende das premissas adotadas.

## Como explorar

1. Abra o **notebook** de um tema diretamente no GitHub para ler o enunciado, acompanhar o cálculo e ver a interpretação.
2. Abra a **planilha correspondente** para examinar as tabelas e fórmulas no Excel ou em um editor compatível.
3. Altere uma premissa, como taxa, prazo, preço ou fluxo de caixa, e compare a nova decisão com o cenário original.

Para executar os notebooks localmente, instale Python e Jupyter em um ambiente virtual:

```bash
python -m venv .venv
source .venv/bin/activate  # No Windows: .venv\Scripts\activate
python -m pip install jupyter pandas matplotlib
jupyter notebook
```

Os notebooks usam `pandas` para organizar resultados e `matplotlib` para gráficos; os cálculos financeiros apresentados são implementados em Python. Os exemplos foram escritos para leitura individual, sem base de dados externa. Os resultados dependem das premissas declaradas em cada exercício; ao reaproveitar um modelo, confira as unidades das taxas e dos períodos.

## Organização

```text
├── Aula_5_Sistemas_de_Amortizacao.ipynb
├── Aula_5_Sistemas_de_Amortizacao.xlsx
├── Aula_6_Analise_de_Investimentos.ipynb
├── Aula_6_Analise_de_Investimentos.xlsx
├── Aula_7_Analise_de_Sensibilidade_e_Risco.ipynb
├── Aula_7_Analise_de_Sensibilidade_e_Risco.xlsx
├── Engenharia Econômica - Aula 5 - Sistemas de Amortização.pdf
└── Engenharia Econômica - Aula 7 - Análise de Sensibilidade e Risco.pdf
```

Os PDFs são os materiais de referência das aulas disponíveis neste repositório. Os notebooks identificam os exercícios e registram as premissas usadas nos cálculos.

## Autor

**João Victor de Melo Schimith** · Ciência da Computação, UNESP · [GitHub](https://github.com/jvschimith)
