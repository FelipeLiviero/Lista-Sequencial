# Lista-Sequencial

Na função de inicializar a lista, fiz uma modificação para que ela seja criada dinamicamente. Caso não consiga ser criada por falta de espaço na memoria, retorna uma mensagem de aviso e usei a função 'exit(1)' para que o programa seja encerrado (encontrei esse método na internet, aonde pessoas usaram em seus projetos). 

Mantive as funções de exibição da lista, a funcao de retorno de tamanho e de tamanho em bytes, de primeiro, ultimo e enesimo elemento, a funcao de reinicializar a lista (numero de elementos), a de busca sequencial, sentinela e binaria.

Na funcao de excluir elementos e a de excluir elementos da lista ordenada, fiz algumas alteracoes. Mantive o comeco da funcao, mas quando a funcao entra no loop coloquei uma condicional para que verifique se o numero de elementos da lista e menor ou igual do que a capacidade dividida por 4, que seria os 25% que estao na instrucao da atividade, se essa condição se satisfazer, o programa diminui a capacidade da lista pela metade. 

Na funcao de insercao de elementos na lista ordenada e na lista ordenada sem duplicata, tambem fiz algumas alteracoes. Primeiro coloquei uma condicional para verificar se o elemnto que esta sendo inserido, tem a posicao maior ou igual a capacidade da lista, se essa condicao satisfazer, ela dobra o tamanho da lista. 

Criei a funcao de redimensionamento da lista, que recebe como parametro um ponteiro para a LISTA e a nova capacidade. Com isso, o ponteiro para o bloco de memoria recebe como valor a funcao realloc, que recebe o ponteiro da memoria, a nova capacidade e multiplica pelo tamanho em bytes de REGISTRO. Coloquei uma condicional para que se haja o retorno NULL na posicao de memoria, exiba para o usuario "Memoria insulficiente" e encerre o programa. Ao final, recebemos o ponteiro para a variavel capacidade, que recebera o valor de nova capacidade.
