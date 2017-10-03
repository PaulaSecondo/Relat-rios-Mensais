# Documento para explicar onde estão os dados vistos no relatório mensal de KitchenAid

Objetivo: Esse arquivo tem por finalidade documentar onde estão os dados do relatório no GA e explica os dados que são contas.  
  
Conta: 01. | WHIRLPOOL | All Sites  
Propriedade: KITCHEN AID | E-Commerce + Site Institucional (UA-44518086-3)  
Vista: kitchenaid.com.br (90011251)  
  
Temos arquivo com extração.  
  
O relatório pode conter partes pontuais, caso achem algum dado interessante de ser mostrado.  
  
**Vendas são transações.**  
  
Dependemos da Mídia para obter alguns dos dados do relatório. São eles: Valores de Investimento, Canais que compõe Mídia e Campanhas de Adwords do mês.  
Sabemos que o canal Mídia é composto por Adowords, Facebook Ads, Criteo e City Ads. Porém não sabemos qual outro Canal foi utilizado.  

### Year-to-date e Month-over-month:

Nesse slide temos dados de **Investimento**, **Usuários**, **Sesssões**, **Vendas** e **Receita** por YTD e MoM.  
Dados por YTD são do período de Janeiro do Ano até a data do relatório, enquanto MoM são do mês do relaótio comparado com o mês anterior.  
A primeira coluna de dados são de YTD, ou seja, são dados de 2017 comparados com 2016.  
Já a segunda coluna de dados são de MoM, ou seja, são dados do mês atual comparado com o mês anterior.  
  
GA para Usuários e Sessões: Público > Visão Geral  
GA para Vendas e Receita: Conversões > Comércio Eletrônico > Visão Geral  

### Canais (comparativo com o ano anterior):

Nesse slide temos dados de **Sessões**, **Vendas** e **Receita** por YTD.  

O dado de Referência é visto de maneira diferente do que os demais.  
GA para Referência: Aquisição > Todo o tráfego > Origem/Mídia  
Coloque no filtro referral e veja o total dos dados  
Coloque a conversão em *Comércio Eletrônico*.  
  
Para os outros Canais podemos olhar como:  
GA: Aquisição > Todo o tráfego > Canais  
Coloque a conversão em *Comércio Eletrônico*.  
  
Para o dado de Mídia, nós temos uma fórmula nesse slide que é **Mídia = Total -Orgânico -Direto -Referência -E-mail**  
O **Total** da fórmula é o total que aparece em Canais.  

### Canais - Esforços de Mídia (comparativo com o ano anterior):

Nesse slide temos dados de **Investimento**, **Vendas** e **Receita**.  
O valor de Outros é o canal que foi utilizado por Mídia e não inclui Adwords, Facebook Ads, Criteo ou CityAds.  
Mas note que nesse slide não precisamos saber qual é o canal Outros. Basta pegar o valor de Mídia do slide anterior e subtrair os dados de Adwords, Facebook Ads, Criteo e CityAds.  
  
GA para Adwords: Aquisição > Adwords > Contas  
Olhe o total dos valores  
  
GA para Facebook Ads: Aquisição > Todo o tráfego > Origem/Mídia  
Some os valores de facebook/cpc e facebook/social.  
  
GA para CityAds: Aquisição > Todo o tráfego > Origem/Mídia  
Filtre para pegar os dados de cityads/cpa  
  
GA para Criteo: Aquisição > Todo o trafégo > Origem/Mídia  
Filtre para pegar os dados de criteo/cpc  
  
Para ver transações e receita coloque a conversão em *Comércio Eletrônico*.  
  
### Canais (comparativo trimestre):

Os dados de Canais são feitos da mesma maneira que Canais (comparativo com o ano anterior), a única diferença é que olhamos por cada mês e não por YTD.  

### Canais - Esforços de Mídia (comparativo trimestre):

OS dados de Canais - Esforços de Mídia são feitos da mesma maneira que Canais - Esforços de Mídia (comparativo com o ano anterior), a única diferença é que olhamos por cada mês e não por YTD.

### Dispositivos Móveis (comparativo trimestre):

Nesse slide olhamos dados de **Sessões**, **Vendas** e **Receita** por dispositivo móvel.  
GA: Público > Dispositivos Móveis > Visão Geral  
Coloque a converão em *Comércio Eletrônico*.  
  
### Jornada de Conversão - Conversões Assistidas:

Nesse slide temos dado de **Vendas** pelo mês atual e passado.  
Olhamos os dados por **Last Click** e **Assitência**.  
  
GA para Last Click: Conversões > Atribuições > Ferramenta de comparação  
**Mude a conversão (que fica acima do gráfico) para somente TRANSAÇÕES**  
Olhe *Conversões de Última interação*.  
Para olhar os dados de Direto, Orgânico e Email, mude para Agrupamento padrão de canais.  
Para olhar o dado de Referência, mude para Origem/Mídia e filtre por *referral*.  
Para olhar os dados de Mídia:  
  
Adwords: Mude a dimensão principal para *Campanhas de Google Adwords*. Precisa pegar o nome de cada campanha utilizada no mês e olhar seu valor de conversões.  
Facebook Ads: Mude para Origem/Mídia e some os valores de facebook/cpc e facebook/social.  
CityAds: Olhe o valor de cityads/cpa.  
Criteo: Olhe o valor de citreo/cpc.  
  
GA para Assistência: Conversões > Funis Multicanal > Conversões assistidas  
**Mude a conversão (que fica acima do gráfico) para somente TRANSAÇÕES**  
Os dados são pegos da mesma maneira que em Last Click.  
  
### Visão do Público - Acesso ao Site e Compra:

Nesse slide temos as **sessões** e **receita** por idade e sexo.
GA: Público > Informações demográficas > Idade  
  
Coloque como dimensão secundária *sexo* e ordene as idades da menor para a maior, assim fica mais fácil pegar os dados.  
Se quiser pode colocar filtro avançado de correspondência exata para pegar os valores de cada sexo separados.  
  
### Visão do Público - Interesses do Público:

Nesse slide temos dados de **Transação**, **Receita** e **Taxa de conversão** por afinidade de interesse.  
GA: Público > Interesses > Categorias de afinidade  
Mude a conversão para *Comércio Eletrônico*.
  
Na dimensão princial temos **interesse/afinidade/categoria**.  
Os dados que nos interessam nesse slide são **interesse/afinidade**, ou seja, não queremos dados que possuem categorias.  
O melhor para olhar cada dado é filtrar pela afinidade e ignorar os dados com categoria.  

### Visão Geográfica:

Nesse slide olhamos os 10 estados que possuem maior valor de **vendas**. Temos também a **receita** dos estados com maior valor de transações.  
GA: Público > Geográfico > Local  
Selecione o pais Brazil e ordene os estados por Transações.  
Coloque a conversão em *Comércio Eletrônico*.  
  
Agora é só escrever os textos de cada slide e as recomendações.
