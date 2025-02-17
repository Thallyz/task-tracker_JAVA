# task-tracker_JAVA
Aplicação CLI de tarefa
Este é um aplicativo de interface de linha de comando (CLI) simples para gerenciar tarefas. Você pode adicionar, atualizar, excluir, marcar e listar tarefas diretamente do terminal.

## Características
Adicionar uma tarefa: adicione uma nova tarefa com uma descrição.
Atualizar uma tarefa: atualiza a descrição de uma tarefa existente.
Excluir uma tarefa: remove uma tarefa pelo seu ID.
Marcar uma tarefa: marque uma tarefa como "em andamento" ou "concluída".
Listar tarefas: liste todas as tarefas ou filtre-as por status (por exemplo, todo, in progress, done).

## Instalação
Clone o repositório:
```bash 
git clone https://github.com/lephuocloc1729/task_tracker_cli
cd task_tracker_cli
```
**Compile o código fonte:**
```bash 
javac TaskCLIApp.java Task.java TaskManager.java Status.java
```
**Execute o aplicativo:**
```bash 
java TaskCLIApp <command> [arguments]
```
## Uso
```bash
# Adding a new task
java TaskCLIApp add "Buy groceries"
# Output: Task added successfully (ID: 1)

# Updating a task
java TaskCLIApp update 1 "Buy groceries and cook dinner"
# Output: Task updated successfully (ID: 1)

# Deleting a task
java TaskCLIApp delete 1
# Output: Task deleted successfully (ID: 1)

# Marking a task as in progress
java TaskCLIApp mark-in-progress 1
# Output: Task marked as in progress (ID: 1)

# Marking a task as done
java TaskCLIApp mark-done 1
# Output: Task marked as done (ID: 1)

# Listing all tasks
java TaskCLIApp list
# Output: List of all tasks

# Listing tasks by status
java TaskCLIApp list todo
java TaskCLIApp list in-progress
java TaskCLIApp list done
```
