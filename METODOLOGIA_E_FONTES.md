# Metodologia e fontes — Radar Macroeconômico Brasil e Goiás

## 1. Escopo

Período de referência: janeiro de 2021 a dezembro de 2025. O projeto é descritivo e organiza séries macroeconômicas nacionais e regionais. Não tem, nesta versão, identificação econométrica para estimar causalidade.

## 2. Indicadores e fontes

| Indicador | Fonte | Série/tabela | Frequência pretendida | Observações |
|---|---|---|---|---|
| IPCA mensal — Brasil | IBGE, divulgado também pelo SGS/BCB | SGS 433 / SIDRA 7060 | Mensal | Conferir a série escolhida e sua unidade no arquivo de fontes. |
| IPCA acumulado em 12 meses — Brasil | IBGE, divulgado também pelo SGS/BCB | SGS 13522 | Mensal | Validar a série diretamente; comparar com qualquer cálculo por composição. |
| IPCA mensal — Goiânia | IBGE / SGS-BCB | SGS 13255; referência SIDRA 7060 | Mensal | A série permanece pendente na versão atual. Goiânia não é sinônimo de todo o estado. |
| Meta Selic | Banco Central/Copom | SGS 432 | Diária | É a meta definida pelo Copom, não a taxa efetiva. |
| IBC-Br com ajuste sazonal | Banco Central | SGS 24364 | Mensal | Indicador de atividade econômica nacional. |
| IBC-Br sem ajuste sazonal | Banco Central | SGS 24363 | Mensal | Usar para comparações compatíveis com a série sem ajuste. |
| IBCR-GO com ajuste sazonal | Banco Central | SGS 25384 | Mensal | Indicador regional de atividade econômica. |
| IBCR-GO sem ajuste sazonal | Banco Central | SGS 25383 | Mensal | Série regional sem ajuste sazonal. |
| Taxa de desocupação | IBGE/PNAD Contínua | SIDRA 6468 | Trimestral | A série histórica precisa ser reconciliada por meio de uma extração metodologicamente consistente. |
| Meta de inflação | Conselho Monetário Nacional / BCB | Resoluções anuais | Anual | Registrar a vigência da meta aplicável a cada ano. |

Links oficiais e detalhes de códigos também estão registrados na aba `05 Fontes` do Excel.

## 3. Transformações

- As datas mensais devem corresponder ao mês de referência do indicador.
- A meta Selic mensal pode ser resumida pelo valor vigente no último dia do mês ou pela média diária do mês; esses critérios são diferentes e devem estar indicados pelo nome da coluna.
- A variação mensal de um índice deve ser calculada a partir de observações comparáveis e, para séries de atividade com ajuste sazonal, deve utilizar a série dessazonalizada.
- Para obter variações acumuladas, deve-se aplicar a composição adequada das taxas, e não simplesmente somar percentuais mensais.
- Observações trimestrais de desemprego devem permanecer trimestrais. Não criar valores mensais interpolados.

## 4. Limitações explícitas

- IPCA de Goiânia: sem série mensal completa na versão atual; não deve ser usado para afirmar que a inflação representa todo Goiás.
- Desocupação: valores compilados na planilha precisam de conferência com uma única extração da SIDRA 6468, mantendo conceito e período homogêneos.
- IPCA Brasil: a série existente e o acumulado de 12 meses precisam de validação integral contra as séries oficiais.
- Meta Selic: a série diária deve ser conferida integralmente com o SGS 432.
- Os indicadores podem apresentar associações no tempo, mas isso não comprova causalidade.

## 5. Checklist antes de publicar resultados como definitivos

- [ ] Conferir os 60 meses de IPCA Brasil diretamente com a fonte oficial.
- [ ] Comparar o IPCA acumulado em 12 meses com a série oficial correspondente.
- [ ] Extrair e validar a série de IPCA de Goiânia.
- [ ] Reextrair a taxa de desocupação de Brasil e Goiás na mesma configuração da SIDRA 6468.
- [ ] Confirmar a série diária de meta Selic no SGS 432.
- [ ] Atualizar fórmulas e gráficos após as validações.
- [ ] Registrar a data da extração de cada fonte.
- [ ] Revisar os rótulos, unidades e notas metodológicas do dashboard.

## 6. Referências

- IBGE/SIDRA, tabela 7060: https://sidra.ibge.gov.br/tabela/7060
- IBGE/SIDRA, tabela 6468: https://sidra.ibge.gov.br/tabela/6468
- BCB, SGS 432: https://dadosabertos.bcb.gov.br/dataset/432-taxa-de-juros---meta-selic-definida-pelo-copom
- BCB, SGS 24364: https://dadosabertos.bcb.gov.br/dataset/24364-indice-de-atividade-economica-do-banco-central-ibc-br---com-ajuste-sazonal
- BCB, SGS 24363: https://dadosabertos.bcb.gov.br/dataset/24363-sgs
- BCB, SGS 25384: https://dadosabertos.bcb.gov.br/dataset/25384-sgs
- BCB, SGS 25383: https://dadosabertos.bcb.gov.br/dataset/25383-sgs
