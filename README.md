# Macroeconomia— Brasil e Goiás (2021–2025)

Projeto de análise econômica aplicada que organiza indicadores de inflação, política monetária, atividade econômica e mercado de trabalho para o Brasil e Goiás, com dados de janeiro de 2021 a dezembro de 2025.

> **Status da versão:** dashboard e estrutura de dados organizados; algumas séries ainda estão explicitamente sinalizadas para validação final. Consulte a aba `06 Controle de Qualidade` antes de reutilizar ou divulgar os resultados como definitivos.

## Objetivo

Construir uma base rastreável e uma visão executiva para observar a evolução recente de indicadores macroeconômicos, destacando diferenças entre séries nacionais e regionais, periodicidades e limites de interpretação.

## Indicadores contemplados

- **Inflação:** IPCA mensal e acumulado em 12 meses para o Brasil; série mensal de Goiânia prevista para comparação regional.
- **Política monetária:** meta Selic definida pelo Copom, em frequência diária e agregações mensais/trimestrais documentadas.
- **Atividade econômica:** IBC-Br nacional, com e sem ajuste sazonal, e IBCR-GO, com e sem ajuste sazonal.
- **Mercado de trabalho:** taxa de desocupação da PNAD Contínua para Brasil e Goiás, em frequência trimestral.

## Arquivo principal

📥 [BAIXAR PLANILHA EXCEL](https://github.com/LucasAm0rim/Macroeconomia-Brasil/raw/refs/heads/main/Macroeconomia%20Brasil%20e%20Goias%2020212025.xlsx?download=1)
O arquivo contém as seguintes abas:

| Aba | Conteúdo |
|---|---|
| `00 Leia-me` | Objetivo, instruções e limitações gerais |
| `01 Dashboard` | Indicadores de destaque, gráficos e leitura executiva |
| `02 Mensal` | Base mensal tratada |
| `03 Trimestral` | Base trimestral e comparações de mercado de trabalho |
| `04 Selic Diária` | Série diária da meta Selic |
| `05 Fontes` | Instituições, códigos, unidades, frequências e links |
| `06 Controle de Qualidade` | Situação das séries, validações e pendências |

## Fontes oficiais

- **IBGE/SIDRA — IPCA, tabela 7060:** https://sidra.ibge.gov.br/tabela/7060
- **Banco Central — meta Selic, SGS 432:** https://dadosabertos.bcb.gov.br/dataset/432-taxa-de-juros---meta-selic-definida-pelo-copom
- **Banco Central — IBC-Br com ajuste sazonal, SGS 24364:** https://dadosabertos.bcb.gov.br/dataset/24364-indice-de-atividade-economica-do-banco-central-ibc-br---com-ajuste-sazonal
- **Banco Central — IBC-Br sem ajuste sazonal, SGS 24363:** https://dadosabertos.bcb.gov.br/dataset/24363-sgs
- **Banco Central — IBCR-GO com ajuste sazonal, SGS 25384:** https://dadosabertos.bcb.gov.br/dataset/25384-sgs
- **Banco Central — IBCR-GO sem ajuste sazonal, SGS 25383:** https://dadosabertos.bcb.gov.br/dataset/25383-sgs
- **IBGE/SIDRA — taxa de desocupação, tabela 6468:** https://sidra.ibge.gov.br/tabela/6468

A planilha também registra códigos e links específicos para cada série na aba `05 Fontes`.

## Metodologia e cuidados de interpretação

1. As séries mantêm sua periodicidade de origem: os dados de desocupação são trimestrais e não devem ser interpolados para criar observações mensais.
2. O IPCA de Goiânia representa a área geográfica coberta pelo índice para Goiânia; não deve ser descrito como medida de inflação de todo o estado de Goiás.
3. O IBC-Br é nacional. Para atividade econômica regional, o arquivo inclui o IBCR-GO, uma série distinta.
4. A meta Selic definida pelo Copom não é sinônimo da taxa Selic efetiva.
5. Variações de índices e comparações temporais devem respeitar ajuste sazonal, unidade e período de referência.
6. Coincidência temporal ou correlação entre inflação, juros, atividade e desemprego não demonstra, isoladamente, causalidade.
7. Dados ausentes ou ainda não reconciliados devem permanecer identificados como pendências, em vez de serem preenchidos por estimativas não documentadas.

Para detalhes adicionais, consulte [`docs/METODOLOGIA_E_FONTES.md`](./METODOLOGIA_E_FONTES.md) e a aba `06 Controle de Qualidade` da planilha.

## Pendências registradas nesta versão

- A série mensal de IPCA de Goiânia ainda precisa ser extraída e validada integralmente.
- A série histórica de desocupação para Brasil e Goiás precisa ser reconciliada com uma extração consistente da tabela SIDRA 6468.
- As séries de IPCA Brasil e meta Selic precisam de conferência integral contra as respectivas séries oficiais antes de serem consideradas auditadas.

Essas limitações são mantidas de forma explícita para preservar a transparência e a reprodutibilidade do projeto.

## Competências demonstradas

- Organização e documentação de dados econômicos;
- tratamento de séries temporais com periodicidades distintas;
- leitura de indicadores macroeconômicos;
- visualização executiva e construção de dashboard em Excel;
- documentação de fontes, critérios e limitações metodológicas;
- controle de qualidade de dados.

## Próximas melhorias

- concluir a extração e a validação das séries pendentes;
- automatizar a coleta de dados oficiais;
- criar um dashboard interativo no Power BI;
- acrescentar uma análise escrita dos principais movimentos observados, evitando inferências causais não sustentadas.

---

**Autor:** Lucas Souza · Estudante de Ciências Econômicas — Universidade Federal de Goiás (UFG)
