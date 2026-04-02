Tratamento de Erros com try-catch
Sobre

O try-catch é uma estrutura usada em C# para tratar erros que podem acontecer durante a execução do programa.

Basicamente, ele tenta executar um código e, se der algum erro, o programa não quebra — ele entra no catch e trata isso.

Como funciona
try: onde fica o código que pode dar erro
catch: onde o erro é tratado caso aconteça

Exemplo simples:

try
{
    int numero = int.Parse("abc"); // vai dar erro
}
catch
{
    Console.WriteLine("Erro ao converter valor!");
}

Nesse caso, ao invés do programa travar, ele mostra uma mensagem.

Ligação com IHC (Prevenção de Erros)

Isso se conecta com a heurística de Nielsen:

Prevenção de Erros

A ideia é evitar que o usuário tenha problemas ou, pelo menos, reduzir o impacto quando algo dá errado.

Onde isso aparece no código

Com o try-catch, o sistema:

Evita que o programa feche sozinho
Controla erros inesperados
Pode mostrar mensagens mais claras pro usuário
Por que isso é importante?

Sem tratamento de erro:

O programa pode simplesmente travar
O usuário não entende o que aconteceu
Gera frustração

Com try-catch:

O erro é controlado
O sistema continua funcionando
O usuário recebe um feedback melhor
Conclusão

O try-catch ajuda a deixar o sistema mais seguro e mais amigável.

Mesmo quando algo dá errado, o programa consegue lidar com isso sem prejudicar tanto a experiência do usuário.
