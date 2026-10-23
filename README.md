# Banco de Projetos — Portfólio e Captação de Recursos

Repositório de dados abertos de projetos e oportunidades de financiamento, preparado a partir de planilha institucional e quatro editais fornecidos.

## Conteúdo

- `dados/projetos.csv`: 325 registros extraídos da aba **Banco de Projetos**, com campos públicos selecionados.
- `dados/editais.csv`: 4 oportunidades identificadas nos documentos anexados.
- `documentacao/dicionario.md`: significado e ressalvas sobre as colunas.

## Como utilizar

Abra os CSVs no GitHub, Excel, LibreOffice ou Python. Os arquivos estão em UTF-8 com BOM para facilitar a leitura de acentos no Excel.

## Cuidados com os dados

Os valores e status refletem a planilha de origem, **não** representam verificação atual nem confirmação de financiamento. Registros podem conter duplicidades de nomes de projetos em diferentes unidades. Campos vazios indicam informação ausente ou não disponibilizada.

**Privacidade:** foram excluídos nomes de gerentes, telefones, observações livres, identificadores de processos e URLs internas. Recomenda-se revisão institucional antes de tornar o repositório público, inclusive dos nomes de projetos e valores.

**Editais:** prazos e condições precisam ser confirmados nos documentos oficiais e em eventuais retificações. O edital CONAVEG trata de homologação territorial, não de repasse automático de recursos.

## Publicação no GitHub

1. Crie um repositório novo no GitHub (por exemplo `banco-de-projetos`).
2. Envie o conteúdo deste pacote usando **Add file → Upload files**.
3. Revise as informações e publique apenas após autorização institucional.
4. Para atualização, edite os CSVs e registre as alterações em um commit.

## Fontes

- Banco de projetos 2.0 (planilha fornecida).
- Edital MMA 2/2026 Prospera Amazônia.
- Edital CONAVEG 02/2026.
- MAPFRE Projetos Incentivados 2026.
- Projeto Floresta+ Amazônia — Modalidade Comunidades 01/2026.

*Versão inicial para revisão e publicação; não é portal de submissão de projetos.*

## Site visual (GitHub Pages)

Este repositório inclui `index.html`, `site.css` e `site.js`, um painel estático responsivo que lê diretamente os CSVs em `dados/`.

### Publicar

1. Crie um repositório **público** no GitHub e envie os arquivos **na raiz** do repositório (não apenas o ZIP).
2. Em **Settings → Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/(root)` e salve.
3. Aguarde a disponibilização do endereço indicado pelo GitHub Pages, geralmente `https://USUARIO.github.io/REPOSITORIO/`.
4. Para atualizar o painel, substitua os arquivos CSV mantendo os mesmos cabeçalhos e publique a alteração.

O site não utiliza serviços externos nem exige instalação. Para testar localmente, execute `python -m http.server 8000` na pasta do repositório e abra `http://localhost:8000/` (abrir diretamente como `file://` pode bloquear a leitura dos CSVs).

**Atenção:** o total de valores é uma soma descritiva dos registros, não uma estimativa de captação. Valores repetidos em projetos por unidade podem inflar o total. Os editais cadastrados não são apresentados como comprovadamente abertos.
