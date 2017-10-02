# Documento para explicar onde estão os dados vistos no relatório mensal de Recovery

Objetivo: Esse arquivo tem por finalidade documentar onde estão os dados do relatório no GA e explica os dados que são contas.  
  
Conta: Recovery  
Propriedade: Grupo Recovery (UA-45367306-1)  
Vista: Grupo recovery - Perfil Principal (78584806)  
  
Temos arquivo com extração.  
  
O relatório é fixo, ou seja, não possuímos partes pontuais.  
  
Promessas são transações.  
  
### Slide 1:

Capa do relatório.  

### Slide 2:

Temos um gráfico de Visitas por mês.  
Precisa ser acrescentado o valor de visitas do mês do relatório.
  
**Visitas:** Público > Visão Geral

### Slide 3:

Temos dois gráficos de Visitas por dispositivos móveis e Promessas por dispositivos móveis.  
Precisa ser acrescentado o valor de desktop e mobile em cada tabela e atualizar os valores que ficam ao lado das tabelas.  
  
**Visitas:** Público > Dispositivos Móveis > Visão Geral  
**Promessas:** Públicos > Dispositivos Móveis > Visão Geral  
Mude a conversão para *Comércio Eeletrônico*.  

### Slide 4:

Temos um gráfico de Visitas por Canais.  
Precisa modificar os dados, deixando o valor do mês anterior e acrescentar o do mês atual.  
  
**Visitas:** Aquisição > Todo o tráfego > Canais  

### Slide 5:

Temos um gráfico de Taxa de Conversão e Promessas por mês.  
Precisa acrescentar o valor do mês atual.  
  
**Taxa de Conversão:** Conversão > Comércio Eletrônico > Visão Geral  
**Promessas:** Conversão > Comércio Eletrônico > Visão Geral  

### Slide 6:

Temos um gráfico de Promessas por Canais.  
Precisa modificar os dados, deixando o valor do mês anterior e acrescentando o do mês atual.  
  
**Promessas:** Aquisição > Todo o tráfego > Canais.  
Mude a conversão para *Comércio Eletrônico*.  

### Slide 7:

Temos dois gráficos. Ambos utilizam a meta 5 - Chat.  
No primeiro gráfico temos chat por dispositivos móveis.  
No segundo gráfico temos chat por canais.  
  
**Dispositivos móveis:** Público > Dispositivos Móveis > Visão Geral  
Mude a conversão para *Meta 5 - Chat*.  
**Canais:** Aquisição > Todo os tráfego > Canais  
Mude a conversão para *Meta 5 - Chat*.  

### Slide 8: 

Esse slide tem seus dados baseados em e-mail marketing.  
Temos variação de Visitas, Cadastros, Promessas e Meta 5 - Chat.  
Essa variação é feita dividindo o valor atual pelo correspondente do mês anterior e retirando 1 (ou seja, (((mês atual)/(mês anterior))-1)%).  
Os gráficos em pizza abaixo fornecem os valores de sessões e promessas de cada e-mail marketing, sendo esses valores separados em prescritos e não prescritos.  

**Sessões Prescritos:** Aquisição > Todo o tráfego > Origem/Mídia.  
Coloque dimensão secundária *conteúdo do anúnico*.  
Faça um filtro avançado de origem/ mídia que contém email e conteúdo do anúncio que contém **p-**.  
  
**Sessões Não Prescritas:** Aquisição > Todo o tráfego > Origem/Mídia.  
Coloque dimensão secundária *conteúdo do anúnico*.  
Faça um filtro avançado de origem/ mídia que contém email e conteúdo do anúncio que contém **np-**.

### Slide 9:

Esse slide contém uma tabela com o TOP 15 dos e-mails marketing prescritos e não prescritos.  
Nessa tabela pegamos os valores de prescritos e não prescritos juntos, só precisando do filtro de email.  
Para facilitar faça um filtro avançado com origem/mídia que contém *e-mail* e conteúdo do anúncio com regex correspondente *(np|p)-*.
