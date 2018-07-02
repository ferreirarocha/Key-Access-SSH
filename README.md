# UsersList
O userlist é um utilitário para lista de forma simples usuários e grupos presentes no sistema, ele confere se estão no  diretório /home e no arquivo /etc/password

# Instalando

`wget https://raw.githubusercontent.com/ferreirarocha/utilitarios/master/userslist`

Enviando o arquivo pra o diretório /usr/bin 

`sudo cp  userslist  /usr/bin/`


## Uso 
 list [-u| users]  -- Exibe os usuarios criados criados com ferramentas administrativas normalmente  possuiem ID acima de 1000 e que possuam diretório home , exceto o  user nobody  

 [-U| all-users]   -- Exibe todos os usuarios do sistema 

 [groups|-g ]      -- Exibe grupos criados via addgroup 

 [all-groups|-G] -- Exibe todos os grupos do sistema
