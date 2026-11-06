# Trabalho CMU - Mod2

Tema Agricultura

## Datasources

### 1. Valor da produção agrícola: total e por tipo

#### Sobre os dados

- **Âmbito geográfico:** Portugal, NUTS I, NUTS II, Ilhas
- **Operação estatística:** Contas Económicas da Agricultura
- **Tipo de operação estatística:** Estudo estatístico
- **Período ou momento de referência:** Ano civil
- **Periodicidade:** Anual
- **Entidade responsável:** INE
- **Âmbito geográfico de referência:** Localização física da exploração

##### Conceitos

| Nome | Definição |
|------|-----------|
| Produção | A produção é constituída pelos produtos criados durante o período contabilístico. São abrangidos os seguintes casos especiais: a) os bens e serviços fornecidos por uma unidade de atividade económica (UAE) local a diversas UAE locais pertencentes à mesma unidade institucional; b) os bens produzidos por uma UAE local que continuem integrados nas existências após o final do período em que são produzidos, independentemente da sua utilização ulterior. (metainformação - INE) |

##### Séries

| Série | U. Medida | Tipo Valor | Escala | Notas |
|-------|-----------|------------|--------|-------|
| Produção agrícola | Euro | Valor absoluto | 10^6 | As atividades secundárias não agrícolas incluem atividades que representam uma continuação da atividade agrícola e que utilizam produtos agrícolas (ex.: transformação de produtos agrícolas) e atividades que utilizam a exploração agrícola e os seus meios de produção (ex.: o agroturismo). |

##### Arquivos
[valor_da_producao_agricola_total_e_por_tipo](data/valor_da_producao_agricola_total_e_por_tipo.xlsx)
##### Link
https://www.pordata.pt/db/portugal/ambiente+de+consulta/tabela/5844454

### 2. Ajudas do Pagamento Único (PU) 2015--2022

## Modelo integrado de dados

### Mapeamento de variáveis
A variável "região" tem designações diferentes nos datasets, embora deva corresponder a uma região NUTS. Serão consolidados numa única designação através de um código NUTS.

O que aconteceu foi que em 2024 foram criadas 3 novas regioes NUTSII, desdobrando a região "Lisboa e vale do Tejo". No dataset 1, serão somados as regioes xx, xx e xx para obter o valor correspondente.

Criação das NUTS II correspondentes a "Lisboa e vale do Tejo" ([link para a fonte](https://ra2019.ine.pt/xportal/xmain?xpid=INE&xpgid=ine_faqs&FAQSfaq_boui=655407417&FAQSmodo=1&xlang=pt)):
- Grande Lisboa - municípios a norte do Tejo da extinta Área Metropolitana de Lisboa.
- Península de Setúbal - municípios a sul do Tejo da extinta Área Metropolitana de Lisboa.
- Oeste e Vale do Tejo - municípios das NUTS III Oeste, Lezíria do Tejo e Médio Tejo.