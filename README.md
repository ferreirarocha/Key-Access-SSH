# KAS ssh access keys

Gerencia os registros de conexão ssh

![kas-ssh-access-Keys](https://2.bp.blogspot.com/-zJlbnWEMy2o/W21ws6IxsxI/AAAAAAABIfY/MDhjmI3jfccrxAAOJQhgKxw4frCgAXxdQCLcBGAs/s320/kas-ssh-access-Keys.png)



# UsersList
O userlist é um utilitário para listar de forma simples usuários e grupos presentes no sistema.

# Instalando

`wget https://raw.githubusercontent.com/ferreirarocha/utilitarios/master/userslist`

Enviando o arquivo pra o diretório /usr/bin 

`sudo cp  userslist  /usr/bin/`


## Uso 
 list [-u| users]  -- Exibe os usuarios criados criados com ferramentas administrativas normalmente  possuiem ID acima de 1000 e que possuam diretório home , exceto o  user nobody  

 [-U| all-users]   -- Exibe todos os usuarios do sistema 

 [groups|-g ]      -- Exibe grupos criados via addgroup 

 [all-groups|-G] -- Exibe todos os grupos do sistema
