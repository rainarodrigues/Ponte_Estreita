### SISTEMAS OPERACIONAIS 2024.1
##### Prof. Fernando Parente Garcia
##### Projeto I - Problema da Ponte Estreita

Carros vindos do leste e carros vindos do oeste chegam a uma ponte com só uma pista. Os que viajam no mesmo sentido podem atravessar a ponte ao mesmo tempo, mas os que viajam em sentido oposto não podem. Portanto, um carro não pode atravessar a ponte quando houver carros atravessando a ponte no sentido contrário. Modele os carros como threads e use semáforos para sincronização entre threads. Os carros devem sair da ponte na mesma ordem
em que entraram (não é possível ultrapassagem, pois a ponte só tem uma pista).
Entradas:
A aplicação deverá possuir um botão para que o usuário possa criar um carro a qualquer momento. Durante a criação do thread carro deverão ser definidos os seguintes parâmetros:
>  Identificador do carro: pode ser um nome ou número.

>  Tempo de travessia: tempo (em segundos) que o carro leva para atravessar a ponte na ausência de carros mais lentos à frente dele. Um carro não pode ultrapassar outro sobre a ponte. O carro não deve dormir durante este tempo (deve ser CPU bound).

> Tempo de permanência: tempo (em segundos) que o carro permanece no mesmo lado da ponte. Depois de decorrido este tempo, o carro deverá tentar atravessar a ponte para o outro lado. O carro não deve dormir durante este tempo (deve ser CPU bound).

Saídas:
A interface deverá atender aos seguintes requisitos:
>  Mostrar os dados de cada carro: identificador, tempo de travessia e tempo de
permanência.

> Mostrar, a cada instante, o status de cada thread carro (atravessando a ponte no sentido leste-oeste, atravessando a ponte no sentido oeste-leste, aguardando a liberação da ponte ou parado no mesmo lado da ponte).

> Mostrar um log com os principais eventos de cada carro.
