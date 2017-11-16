Deadlock é um bloqueio entre threads ou processos que pretendem acessar os mesmos recursos ou que dependem um do outro, fazendo com que à espera da liberação de um, impacte um segundo e o mesmo esteja a espera de um terceiro, e assim por diante.

Existem diversas ações para resolver esses potenciais problemas e a implementação pode variar de sistema para sistema.

#### Sincronização:
Sincronizar regiões críticas dos código faz com que o recurso não seja compartilhados entre as threads, fazendo com que haja a espera da liberação do mesmo antes que outra thread fique dependente.

#### Semaforo:
- Inicialização de threads indicando a quantidade de processos que podem acontecer simultaneamente
- Valor de espera da thread, para que ela aguarde quando poderá ser executada novamente de acordo com as notificações de outra thread, usado quando um thread fique aguardando a liberação, mas ao invés de ela ficar retendo o acesso ao "recurso" ela fica "dormindo" esperando que outra thread que esteja usando o recurso anteriromente à avise que ela pode começar sua operação.
- Sinalização quando a thread avisa outra thread que ela pode começar suas operações, caso que essa thread faça parte dos grupo de threads do semáforo