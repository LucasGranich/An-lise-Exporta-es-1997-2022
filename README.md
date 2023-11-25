# An-lise-Exporta-es-1997-2022
Trabalho final de Data Science II
Introdução 

Uma análise minuciosa da balança comercial brasileira revela detalhes macro e microeconômicos dos atores político-econômicos envolvidos, e sendo o próprio resultado da balança comercial algo de extrema importância histórica, o Brasil sempre dependeu de um bom resultado da balança comercial para não ter problemas internos, de políticas monetárias, fiscais e cambiais, todos os grandes ciclos econômicos brasileiros não abrangeram necessidades nacionais, e sim internacionais, por isso as grandes recessões internas foram, direta ou indiretamente, resultantes de problemas econômicos proporcionados por falta de demanda, como o café, concorrentes internacionais, açúcar ou crises de produção, como a do ciclo do ouro, assim como o Brasil continuamente se beneficia e se beneficiou de altas nas demandas dos mesmos recursos, sendo a mais recente o do Super-Boom das commodities chinesas no começo do milênio e que de certa forma se estende até os dias atuais. 

Além disso a produção brasileira para exportação impacta diretamente as economias regionais dos países fronteiriços, em especial Argentina e Paraguai, sendo a capacidade produtiva brasileira tão superior a estes que o Mercosul tem se tornado imponente frente a evidência que uma abertura comercial destes países ocasionaria em quebra de empresas, gerando constantes entraves a diplomacia. 

Então se algo é tão importante para a economia e influência centenas de milhões de habitantes brasileiros e não-brasileiros, se torna imperativo uma análise cuidadosa, holística e também particularizada dos fatores que impactam os fatores produtivos. 

A base de dados escolhida foi a do COMEX STAT, o portal de acesso gratuito às estatísticas do comércio exterior, que integra o Ministério do Desenvolvimento, indústria e comércio, sendo utilizada a base de dados detalhada por NCM, pois nela é registrado a categoria do produto, o valor da exportação, quantidade, de qual estado da federação, a forma de transporte e a quantidade, assim como peso. 

Metodologia 

A forma utilizada para limpeza e tratamento de dados foi a biblioteca pandas e para a geração dos gráficos a Seaborn e a Matplotlib.	 

A base de dados estava separada por ponto e vírgula, portanto tivemos que mudar para virgula para permitir melhor leitura dos dados e todas as colunas continham apenas valores nominais como as colunas de valore, peso, quantidade e também os códigos dos produtos, países e forma de exportação, e essas tabelas com os códigos e seus valores correspondentes estavam também no mesmo site do COMEX STAT na área de tabelas auxiliares, portanto foi necessário correlacionar usando a função “merge” para sabermos quais eram os produtos, países e formas de exportações com as tabelas auxiliares. 

 

 	Após isso fizemos as verificações de valores nulos e anomalias, e foi verificado que em nenhum dos anos possuíam valores nulos e não possuíam valores em lugares errados e nem algum erro ao longo da base de dados, e foi realizada essa limpeza e verificação em todos os data frames de 1997 até 2022 sendo cada data frame possuindo na média 1 milhão e 300 mil linhas cada. 

Dessa tabela final dos dados brutos, geramos 2 outras tabelas, a da somatória de exportações para cada país que o Brasil exportou e outra com os produtos mais exportados, portanto decidimos analisar os países que mais importavam e também as pautas de exportações. 
