# Documento para explicar onde estão os dados vistos no relatório semanal de KitchenAid

Objetivo: Esse arquivo tem por finalidade documentar onde estão os dados do relatório no GA e explica os dados que são contas.  
  
Conta: 01. | WHIRLPOOL | All Sites  
Propriedade: KITCHEN AID | E-Commerce + Site Institucional (UA-44518086-3)  
Vista: kitchenaid.com.br (90011251)  
  
Temos arquivo com extração.  
  
O relatório é fixo, ou seja, não possui partes pontuais.  
  
Usamos extração por Analytics Edge.  
  
O relatório é feito e entregue em Excel.  
Temos 3 abas: **Consolidado**, **Por Mês** e **Mês Origem**.  
  
Para atualizar a extração basta clicar em Refresh All do Analytics Edge.  
Após isso, olhe no link do Drive os dados de NET SALES. Precisa colocar esses dados manualmente na extração após ser atualizada.  
Link do Drive: https://docs.google.com/spreadsheets/d/16xwHbfEGfAACDdPZAkNLBWGo1O9qCBqj_svgntRkCy4/edit?ts=598e096f#gid=798406770  
  
Após atualizar esse dados, faça uma cópia do relatório da semana anterior, atualize a data e cole como valor as abas da extração.
  
### Validação:

#### Aba Consolidado:

Selecione o período de janeiro de 2017 até a data do relatório.  
  
Os dados de **Visitas**, **Usuários**, **Taxa de rejeição** e **Porcentagem de novas sessões** são encontrados em:  
Público > Visão Geral  
O dado de **Novos Sessões** não está explicito no GA. Lembre que *(Novas sessões)/(Sessões) = Porcentagem de Novas Sessões*.  
Como possuímos o valor de sessões e porcentagem de novas sessões, conseguimos saber qual o valor de Novas sessões.  
  
Os dados de **Transações**, **Valor médio do pedido**, **Receita** e **Taxa do comércio eletrônico** são encontrados em:  
Conversão > Comércio Eletrônico > Visão Geral  
  
O dado de **Porcentagem de aprovação** é uma conta de NET SALES / Receita.  
**Lembre que o dado de NET SALES precisa ser pego pelo DRIVE.**  
  
Os dados de **Investimento de Mídia** e **Porcentagem de ROI** não são preenchidos por BI.  
Quem preenche esses dados é a pessoa de mídia para quem é enviado o relatório.  

#### Aba Por Mês:

Selecione o período do começo do mês até a data do relatório.  
  
Os dados olhados são os mesmos da aba Consolidado, a diferença é que não estamos olhando o total do ano até a data e sim os meses separados.  
A validação segue quase igual, a única diferença é que não possuímos o valor de NET SALES por mês. Assim essa célula fica vazia até o final do mês.  
No final do mês podemos colocar o NET SALES pois o temos em todas as semanas, ou seja, no último relatório de cada mês possuímos o NET SALES total do mês.  

#### Aba Mês Origem:

Selecione o período do começo do mês até a data do relatório.  
  
Caso tenha alguma dúvida sobre o que for escrito a seguir ou não lembrar de todos os passos, olhe na fórmula de cada Canal para saber o que está sendo pego.  
  
Para ver Transações e Receita, basta colocar as conversões em *Comércio Eletrônico*.  
  
**Canal Google Search:**  
Note que no GA temos que Paid Search é google/cpc e google/display.  
Portanto, para saber exatamente qual o valor de google/cpc precisa ser feita uma extração.  
Observe também que o valor do relatório sempre vai ser menor do que o valor do GA.  
GA: Aquisição > Todo o tráfego > Canais  
  
**Canal Google Display:**  
É o canal Display que aparece em Canais do GA.  
GA: Aquisição > Todo o tráfego > Canais  
  
**Canal Google & Bing Organic:**  
É o canal Organic que aparece em Canais do GA.  
GA: Aquisição > Todo o tráfego > Canais  
  
**Canal Direto:**  
É o canal Direct que aparece em Canais do GA.
GA: Aquisição > Todo o tráfego > Canais  
  
**Canal Criteo:**  
Precisamos olhar em Origem/Mídia para saber o valor desse canal.  
Ga: Aquisição > Todo o tráfego > Origem / Mídia  
Coloque como filtro *criteo* e olhe os valores de Criteo/cpc.  
  
**Canal CityAds:**  
Precisamos olhar em Origem/Mídia para saber o valor desse canal.  
Ga: Aquisição > Todo o tráfego > Origem / Mídia  
Coloque como filtro *cityads* e olhe os valores de cityads/cpa.  
  
**Canal Email:**  
Precisamos olhar em Origem/Mídia para saber o valor dessa canal, pois o Canal E-mail que fica em Todo o tráfego > Canais contém dados a mais do que precisamos.  
GA: Aquisição > Todo o tráfego > Origem / Mídia  
Coloque como filtro *email* e olhe os valores de **kitchenaind_mail**.  
  
**Canal Facebook (sem referral):**  
Precisamos olhar em Origem/Mídia para saber o valor desse canal.  
GA: Aquisição > Todo o tráfego > Origem / Mídia  
Coloque filtro avançado de incluir origem/mídia que contém facebook e excluir regex correspondente (referral|ccontent).  
Aí é só olhar o valor total dos dados que aparecem.  
  
### Observe que

Após finalizar a validação do relatório, precisa colocar dados no Drive.  
Todas as células que estão em amarelo são de preenchimento de BI, ou seja, quem fez o relatório e o validou preenche o Drive.
