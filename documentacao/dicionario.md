# Dicionário de dados

## projetos.csv

- `id`: identificador técnico, baseado na linha original; não é ID oficial.
- `projeto`: nome/descrição conforme planilha.
- `unidade_beneficiada`: unidade indicada na fonte.
- `inovacao`: indicador textual da fonte.
- `contemplado`: informação de contemplação conforme fonte.
- `portfolio_atual`: indicador de inclusão no portfólio da fonte.
- `valor_previsto_brl`: valor informado na planilha, em reais; não equivale necessariamente a recurso captado.
- `aba_origem`, `linha_origem`: rastreabilidade interna da extração.

## editais.csv

- `id`: identificador técnico.
- `edital`, `instituicao`, `tema`, `abrangencia`: classificação resumida.
- `observacoes_elegibilidade`: resumo, não substitui a leitura integral.
- `data_abertura`, `data_limite`: vazios quando não validados.
- `documento_fonte`: arquivo usado para o registro.
- `observacao_prazo`: ressalvas sobre datas e verificação.

## Limitações

Este conjunto não publica as abas de captação e recursos captados, que contêm observações e informações administrativas que requerem tratamento adicional. Não foram publicados os PDFs originais; o responsável pode incluir links públicos oficiais após verificação.
