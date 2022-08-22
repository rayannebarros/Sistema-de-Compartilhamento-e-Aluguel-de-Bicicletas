# Sistema-de-Compartilhamento-e-Aluguel-de-Bicicletas
Projeto realizado na disciplina de Mineração de Dados, no período 2021.1

Os sistemas de compartilhamento de bicicletas são um meio de alugar bicicletas em que o processo de obtenção de inscrição, aluguel e devolução de bicicletas é automatizado por meio de uma rede de quiosques em toda a cidade.
 
Usando esses sistemas, as pessoas podem alugar uma bicicleta em um local e devolvê-la a outro local conforme a necessidade. 
Atualmente, existem mais de 500 programas de compartilhamento de bicicletas em todo o mundo.

Os dados gerados por esses sistemas os tornam atraentes para os pesquisadores porque a duração da viagem, o local de partida, o local de chegada e o tempo decorrido são registrados explicitamente. 
Os sistemas de compartilhamento de bicicletas, portanto, funcionam como uma rede de sensores, que pode ser usada para estudar a mobilidade em uma cidade.

Neste projeto, são combinados padrões históricos de uso com dados meteorológicos para prever a demanda de aluguel de bicicletas no programa na cidade de Washington.

O dataset tem dados de aluguel (por dia ou hora) durante dois anos. 

O objetivo é prever a contagem total de bicicletas alugadas durante cada dia coberta pelo conjunto de teste, usando apenas as informações disponíveis antes do período de locação.

Dados:
datetime - data por hora + timestamp
season - 1 = primavera, 2 = verão, 3 = outono, 4 = inverno
holiday - se o dia é considerado feriado
workingday - se o dia não é fim de semana nem feriado
wheater:
1: céu limpo, poucas nuvens ou parcialmente nublado
2: Névoa + Nublado, Névoa + Nuvens quebradas, Névoa + Algumas nuvens, Névoa
3: neve fraca, chuva fraca + trovoada + nuvens dispersas, chuva fraca + nuvens dispersas
4: Chuva forte + Paletes de gelo + Trovoada + Névoa, Neve + Nevoeiro
temp - temperatura em Celsius
atemp - sensação térmica em Celsius
humidity - umidade relativa do ar
windspeed - velocidade do vento
---------------
casual - número de aluguéis de usuários não registrados no sistema
registered - número de aluguéis de usuários registrados 

no sistema
> cnt - número total de locações (nossa previsão)

São realizadas:

- Uma análise exploratória dos dados
- Um etapa de pré-processamento (limpeza, extração de novas features, seleção de features, etc)
- O treinamento, usando pelo menos 2 técnicas: um classificador padrão de ML e uma rede neural.
- Avaliação dos modelos usando a métrica MSE (Mean Squared Error)
