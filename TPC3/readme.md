Comecei por importar o random, para este ser usado na função modo2() e criar as jogadas aleatórias do computador. 
A função modo1() irá permitir que o utilizador inicie a sua jogada antes do computador. Defini que o número inicial de fósforos era 21, através da variável fosf. 
Criei um ciclo while de forma que o jogo decorresse enquanto o número de fósforos fosse maior que 0. Iniciei o ciclo com a impressão do número de fósforos disponíveis. De seguida criei a variável b, que pedia ao utilizador que inserisse o número de fósforos que pretendia retirar. Com o intuito de impedir que o número que ele inserisse fosse maior que 4 ou menor que 0, e que em adição fosse maior que o número de fósforos, criei um ciclo while. Caso ele inserisse um número dentro dessas condições, seria novamente lhe pedida uma nova impressão do número de fósforos. 
À variável fosf, retirei b (o número inserido pelo utilizador) e imprimi o resultado.
A variável c representa o valor a jogar pelo computador. O computador deverá escolher um número que somado ao número escolhido anteriormente pelo utilizador seja igual a 5. Esta soma deverá ser sempre igual a 5, de forma que na última jogada do jogo exista a sobra de um fósforo e que assim o primeiro jogador a jogar seja o que irá perder. 
À variável fosf retirei o c.
Para terminar o ciclo decidi colocar uma condição, para quando o fosf fosse igual a 1, o programa imprimisse que o jogo tinha terminado e que o último jogador a retirar o fósforo tinha perdido a partida. Adicionei ainda que fosf era igual a 0 de forma que o ciclo terminasse mesmo.
Para o modo 2, criei outra função designada por modo2(). 
Defini a variável fosfe como sendo 21 e outra variável “ver” igual a false. Esta variável irá permitir que caso o utilizador escolha um número diferente do que é suposto, seja ativo um modo onde o computador irá inverter o seu papel e irá escolher números em que somados com o do utilizador darão 5. 
Enquanto o fosfe for maior que 0 e ver for False, será impresso o número de fósforos existentes e o computador irá escolher um número random de 1 a 4. Enquanto esse número for maior que o número existentes de fósforos, será pedido que o computador crie um novo b. 
Após a criação do b, este será retirado ao fosfe e será seguidamente impresso o próprio b e o número de fósforos que restam. 
A variável c é o número introduzido pelo utilizador. Enquanto esse número for maior que 4 e menor que 1, o utilizador terá que introduzir um novo número até este ser válido. 
O jogo irá decorrer enquanto 
À variável fosf será retirado o c. Caso o c introduzido não vá de encontro ao raciocínio de ( 5 – b),  a variável ver, passará a ser True.
Ao c será somado o b.
Todo o algoritmo irá começar novamente, e neste caso, se o ver for true, o b já não será gerado aleatoriamente, mas será igual à subtração de b ao 5. O algoritmo irá decorrer de igual forma até o fosfe ser 1. Quando este for 1, o jogo irá terminar e o ciclo while também.
A função jogar(), irá permitir que o utilizador escolha qual dos modos quer jogar. 
Enquanto o utilizador não escolher 1, 2 ou 0, será lhe pedido que introduza novamente o número do modo que pretende jogar. Após ele escolher um destes três números, o ciclo while termina e teremos 3 condições. Se o número introduzido pelo utilizador for 1, a função modo1() será chamada. Se o número introduzido for 2, será chamada a função modo2(), de forma que seja jogada a modalidade 2. Caso tenha sido introduzido 0, o programa irá terminar.
