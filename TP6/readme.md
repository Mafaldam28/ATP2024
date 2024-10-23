readme.md
Comecei por criar a função criaTurma, que cria uma lista vazia.
Na função seguinte, inserealuno(aluno, turma), verifiquei se o aluno não estava na lista criada anteriormente através da função consulta, e caso este não estivesse, seria adicionado à lista turma.
Na função listar(turma), percorri a lista através do ciclo for, para que cada elemento da lista fosse impresso.
Na função consulta(turma, id), percorri a lista através do ciclo for, de forma a comparar o id inserido com o id do elemento da lista turma. Caso o id do elemento da lista fosse igual ao inserido, seria impresso esse elemento, ou seja, o aluno.
Na função guarda(turma), criei uma variável que guarda o ficheiro inserido pelo utilizador. Abri o ficheiro, de forma a escrever nele. Através do ciclo for, a lista foi percorrida, e cada elemento na lista foi colocado no ficheiro. O ficheiro foi fechado.
Na função carrega(), foi criada a lista turma, de forma a serem lá adicionados os alunos do ficheiro. Através da variável a, foi guardado o ficheiro escolhido pelo utilizador. Foi criada a variável i com valor 1, que terá a função de contador. O ficheiro foi aberto e foram percorridas cada uma das suas linhas, de forma a serem lidas. O ficheiro foi escolhido.
Foi impresso ao utilizador o menu de forma a este escolher qual quer aceder. 
Criou-se uma variável a = 1, de forma a iniciar-se o ciclo while, que irá terminar quando o a for 0. Dentro do ciclo é pedido ao utilizador o número que pretende aceder e este é atalizado em a. Para cada a escolhido, será chamada a função correspondente.