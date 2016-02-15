Repositório de dados sobre ocorrências de trânsito de 2014 com vítimas fatais na cidade de São Paulo. Os dados foram pedidos via Lei de Acesso à Informação.

## Dados abertos

Download dos dados em formato abertos

## Dados originais em formato proprietário

A prefeitura disponibilizou um arquivo .zip com os seguintes arquivos de dados em formato proprietário.

1) `GeocodificaЗ╞o_2014_crg_Tadeu-11_12_15_ACDIS.TAB`

Georeferenciamento dos acidentes, em formato Mapinfo. Use o ogr2ogr para conversão, por exemplo:

    ogr2ogr -f "ESRI Shapefile" ocorrencias-fatais-2014.shp dados/GeocodificaЗ╞o_2014_crg_Tadeu-11_12_15_ACDIS.TAB


2) `Protocolo PR 12024.accdb`

Detalhes das ocorrências em formato MS Access 2007. Use o `mbtools` para conversão, por exemplo:

    mdb-export Protocolo\ PR\ 12024.accdb Acidentes2014 > acidentes-2014.csv

3) `Prot 120224 Dicionario de Dados.pdf`

Dicionário de dados em PDF.
