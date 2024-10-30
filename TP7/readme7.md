
Comecei por definir as funções e contruí-las de forma a depois poder incorporá-las no algoritmo do menu. 
Na função medias(tabMeteo), comecei por criar uma lista vazia de forma que depois pudesse adicionar a data e a média das temperaturas. Percorri a lista, e para cada elemento, criei uma variável soma, onde era guardada a soma da temperatura mínima (elem[1]) com a temperatura máxima (elem[2]). Defini a variável média, ainda dentro do ciclo for, como sendo igual à soma a dividir por 2. Seguidamente adicionei à lista um tuplo com a data (elem[0]) e com a média. Retornei a lista.
Na função guardaTabMeteo(t, fnome), comecei por abrir o ficheiro com o intuito de escrever, logo usei o “w”. Percorri os dias da tabela meteorológica e escrevi no ficheiro cada componente de cada dia. Seguidamente transformei tudo em strings e decidi dividir a data, tempmin, tempmax, e prec com o divisor “;” e dentro da data o dia, mês e ano com o divisor “,” , sem esquecer no fim do \n para passar a linha.
Na função carregaTabMeteo(fnome), criei uma lista vazia e abri o ficheiro para ler. Percorri as linhas do ficheiro e retirei o \n de cada linha ao fazer linha = linha[:-1]. Seguidamente, como o split da linha pelo ";" dá uma lista com (data,tempmin,tempmax,prec) atribui a cada elemento desta lista uma variável para depois colocar na minha lista que vou retornar. Fiz split novamente na data para conseguir retirar o ano, mês e dia. Fiz append de todas as variáveis que criei, tendo em conta o formato pretendido e convertendo-os todos a inteiros e floats (no caso da precipitação). Retornei a lista.
Na função minMin( tabMeteo), defini a variável min como sendo 1000, de forma a que esta fosse maior que qualquer temperatura mínima da tabela meteorológica. Seguidamente percorri a lista e comparei a temperatura mínima com a variável min, e caso a temperatura mínima fosse menor que a variável, a variável seria redefinida e igual á temperatura mínima. Retornei a variável min.
Na função amplTerm(tabMeteo), criei a lista res, como sendo vazia. Percorri a lista através do ciclo for, e para cada elemento, retirei a temperatura mínima à máxima. Guardei o resultado na variável amp. Adicionei à lista res, o tuplo (elem[0], amp), que é especificamente (data, amplitude). Retornei a lista res.
Na função maxChuva(tabMeteo), defini a variável max como 0, de forma a que esta fosse mínima o suficiente para ser comparada com o resto das precipitações da tabela. Percorri a lista através do for, e comparei se a precipitação do elemento era maior que a variável max, caso isso se sucedesse, max passaria a ser o valor da precipitação desse elemento. Retornei a variável max.
Na função diasChuvosos(tabMeteo, p), Criei uma lista vazia designada de res. Percorri a lista inserida na função através do for, e comparei a precipitação de cada emento com o p. Caso fosse maior, adicionei o tuplo com a data desse elemento e a precipitação dentro da lista, através do append. Retornei a lista res.

Defini o ”a” como sendo 1 de forma a poder iniciar o ciclo while a seguir. Enquanto a variável a for maior que 0, será impresso o menu e será pedido ao utilizador que insira o número do menu ao qual pretende aceder. De acordo com o número introduzido pelo utilizador será chamada a função correspondente. O ciclo acaba quando o utilizador insere 0.