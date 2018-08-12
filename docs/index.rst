.. figure:: https://camo.githubusercontent.com/69a379292944cd4e1a0c977df0374246928abc5e/68747470733a2f2f322e62702e626c6f6773706f742e636f6d2f2d7a4a6c626e57454d79326f2f57323177733649787378492f41414141414141424966592f4d44686a6d49336a666363727841414f4a5168674b787734667243674158786451434c63424741732f733332302f6b61732d7373682d6163636573732d4b6579732e706e67
   :alt: 

Author Marcos Ferreira da Rocha

EMail marcos.fr.rocha@gmail.com

Este script envia automatiza a geração e inserção de chave pública em um
servidor ssh.

version=1.0

.. _header-n17:

Sobre
=====

O KAS Key Access SSH, automatiza a geração e inserção de chave pública
em servidores ssh, ele também cria funções para cada conexão no shell
corrente afim de facilitar o acesso futuro. Ele também pode exportar,
importar, e criar novos pares de chave de conexão, saiba mais na
documentação.

.. _header-n24:

Menu de ajuda
=============

.. code:: 

   Todas as opções;

   -a --add             Adiciona um nova conexão
   -c --conf            Lista os arquivos de configuração e diretórios do script
   -e --edit            Edita o arquivo de  conexões
   -h --help            Exibe o menu de ajuda
   -i --import          Importa registro de conexões
   -I --import-all      Importa  as chaves e as  conexões registradas
   -l --list            Lista as conexões registradas
   -n --new-key         Cria um novo par de chaves
   -r --reset           Limpa registro de conexões
   -s --save-key        Salva o par de chaves utilizadas  pelo script  na home do usuário corrente
      --set-editor      Configura o editor padrão
      --uninstall       Remove o script
   -U --update          Atualiza o Key Access ssh (kas)
   -x --export          Exporta o registro de conexões
   -X --export-all      Salva as chaves e as  conexões registradas

.. _header-n30:

Adicionando registro de conexão
===============================

Para registrar uma nova conexão siga o exemplo;

.. code:: 

   kas -a servidor user@192.168.1.1

.. _header-n36:

Exportando registros de conexão
===============================

Para exportar todos os registros de conexões siga o exemplo;

.. code:: 

   kas -e nome-do-arquivo

ou

.. code:: 

   kas --export nome-do-arquivo

.. _header-n42:

Importando registro de conexão
==============================

Para importar todos os registros de conexões siga o exemplo;

.. code:: 

   kas -i nome-do-arquivo

ou

.. code:: 

   kas --import nome-do-arquivo

.. _header-n302:

Importando todos os registros e chaves de conexão
=================================================

Para importar todos os registros de conexões e chave ssh siga o exemplo;

.. code:: 

   kas -I nome-do-arquivo

ou

.. code:: 

   kas --import-all nome-do-arquivo

.. _header-n322:

Exportando todos os registros e chaves de conexão
=================================================

Para exportar todos os registros de conexões e chave ssh siga o exemplo;

.. code:: 

   kas -X nome-do-arquivo

ou

.. code:: 

   kas --export-all nome-do-arquivo

.. _header-n60:

Exibir diretório e arquivos de Configuração
===========================================

Abaixo é apresentado o conjuto de diretórios e arquivos que compõem a
aplicação;

.. code:: 

   access_functions     Armazena as conexões registradas
   ~/.local/share/acesso/       Armazena os arquivos de configuração da aplicação
   ~/.bashrc            Exportar o arquivo access_functions para o shell corrent
   ~/.zshrc             Exportar o arquivo access_functions para o shell corrente
   ~/.ssh/                      Diretório utilizado para  acessar o par de chaves
   /usr/bin/            Diretório com  script executável

.. _header-n87:

Atualizando o script
====================

Para atualizar o script ou

.. code:: 

   kas --update 

.. _header-n114:

Instalando o script
===================

.. _header-n452:

Instalação automática
---------------------

.. code:: 

   curl -s https://raw.githubusercontent.com/ferreirarocha/Key-Access-SSH/master/kas | bash -s -- --install

.. _header-n454:

Ou

.. code::

   wget bit.ly/install-kas ; bash install-kas --install
   
.. _header-n454:

Instalação manual
-----------------

.. code:: 

   wget https://raw.githubusercontent.com/ferreirarocha/Key-Access-SSH/master/kas

.. code:: 

   chmod +x kas

.. code:: 

   cp /usr/bin/ 

.. _header-n475:

Desinstalando o script
======================

.. code:: 

   kas --uninstall 

.. _header-n121:

Editando registros
==================

.. code:: 

   kas -e

ou

.. code:: 

   kas --edit

.. _header-n140:

Alterando o editor padrão
=========================

.. code:: 

   kas  --set-editor 

Exemplo

.. code:: 

   kas --set-editor  vim

.. _header-n170:

Salvando o par de chaves usada pelo script
==========================================

.. code:: 

   kas -s 

ou

.. code:: 

   kas --save-key 

.. _header-n200:

Limpando registro de conexões
=============================

Para limpar o registro de conexões execute o comando

.. code:: 

   kas -r

ou

.. code:: 

   kas  --reset

.. _header-n224:

Listando as conexões
====================

.. code:: 

   kas -l

ou

.. code:: 

   kas --list

.. _header-n242:

Criando um novo par de chaves
=============================

.. code:: 

   kas --new-key

ou

.. code:: 

   kas -n
