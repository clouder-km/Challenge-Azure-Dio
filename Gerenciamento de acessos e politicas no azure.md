# Gerenciamento de acessos e politicas no azure


## Tipos de Lock *** Descrever

- Lock Delete - A nivel do Resource Group este lock não deixa deletar o resource group mas pode fazer alterações nos recursos. A nivel do Resorce o lock não deixa deletar o recurso porém se tivermos lock em um recurso e for deletar o Resource Group não irá deletar nenhum recurso mesmo que os outros recursos não tenham lock.
- Lock Read - A nivel do Resource Group este lock somente deixará ler as informações não irá deixar deletar e nem alterar (atualizar) qualquer recurso. A nivel do Resource somente aquele recurso não irá deixar deletar e alterar porém se deletar o resource group não irá deixar deletar da mesma forma que a de cima.

## Lock Delete no Resource Group 

- Acesse o [Portal Azure]()
- Vá para Resource Group 
- Em *"Settings"* : *"Locks"*
- *"+ add"*
  - Lock name: Nome do Lock
  - Lock Type: Tipo do Lock (Delete)
  - Notes: Mensagem importante para o Lock 

- Por exemplo caso o usuário administrador do ambiente não saiba do que se trata esse grupo de recurso ou recurso e o usuário for deletar isso,  o azure vai 
apresentar mensagem de erro e o motivo do erro , usuário vai para "locks" e aparecerá o lock com a mensagem que configuramos em notes.

- Em *"Overview"* clique em *"Delete Resource Group"*
- Forneça o nome do *"resource group"*
- Marque a caixa * "Apply force delete ..."*
- Clique em *"Delete"* e confirme o *"Delete"*
- Aparecerá mensagem de erro
- Vá para "Locks" e verifica o porque não conseguiu apagar o resource.

## Lock Read no Resources 

-Vá para o recurso Ex: Virtual Machine
-Clique na Vm que deseja colocar o lock
-Clique em *"Settings" : "Locks"*
- *"+ add"* e preencha as informações (Read)
- Em *"Availability + Scale"* clique em *"Size"*
- Selecione a Vm que atenda a sua necessidade
- Click em *"resize"* e confirme *"resize"*
- Aparecerá mensagem de erro
- Vá para "Locks" e verifica o porque não conseguiu apagar o resource.

Mover recursos

- Vá para *"Resource Group*" que irá remover os resources
- Selecione os resources que quer mover
- Clique em Move
- Clique em Move to another resource group
- Selecione o outro resource group e click em next
- Aguarde checar e clique em Next
- Marque *"I underrstand ... "*
- Aguarde mover e aparecerá a mensagem de confirmação que foi movido
