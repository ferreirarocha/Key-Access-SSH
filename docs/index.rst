.. figure:: https://camo.githubusercontent.com/69a379292944cd4e1a0c977df0374246928abc5e/68747470733a2f2f322e62702e626c6f6773706f742e636f6d2f2d7a4a6c626e57454d79326f2f57323177733649787378492f41414141414141424966592f4d44686a6d49336a666363727841414f4a5168674b787734667243674158786451434c63424741732f733332302f6b61732d7373682d6163636573732d4b6579732e706e67
   :alt: 

| Author Marcos Ferreira da Rocha
| EMail marcos.fr.rocha@gmail.com
| Este script envia automatiza a geração e inserção de chave pública em um servidor ssh.
| version=1.0


.. _header-n18:

Ajuda
=====

.. code:: 

   Todas as opções;

   -a --add 		Adiciona um nova conexão
   -c --conf		Lista os arquivos de configuração e diretórios do script
   -e --edit		edita o arquivo de  conexões
   -h --help		Exibe o menu de ajuda
   -i --import		importar registro de conexões
   -I --import-all	Importa  as chaves e as  conexões registradas
   -l --list		Lista as conexões registradas
   -n --new-key         Cria um novo par de chaves
   -r --reset		Limpar   registro de conexões
   -s --save-key	Salva o par de chaves utilizadas  pelo script  na home do usuário corrente
      --set-editor	Configure o editor padrão
      --uninstall		   Remover o script	   
   -x --export		Exportar registro de conexões
   -X --export-all	Salva as chaves e as  conexões registradas
      --install		Instala ou atualiza o Key Access ssh (kas)

.. _header-n23:

Ajuda-registro
==============

.. code:: 

   Para registrar uma nova  conexão siga o exemplo;

   kas -a servidor user@192.168.1.1

.. _header-n25:

Ajuda-export
============

.. code:: 

   Para exportar todos os registros de conexões siga o exemplo;

   kas -e nome-do-arquivo
   kas --export nome-do-arquivo

.. _header-n28:

Ajuda-import
============

.. code:: 

   Para importar todos os registros de conexões siga o exemplo;

   kas -i nome-do-arquivo
   kas --import nome-do-arquivo

.. _header-n32:

Ajuda-import-all
================

.. code:: 

   Para importar todos os registros de conexões e chave ssh siga o exemplo;

   kas -I nome-do-arquivo
   kas --import-all nome-do-arquivo

.. _header-n35:

Ajuda-export-all
================

.. code:: 

   Para exportar todos os registros de conexões e chave ssh siga o exemplo;

   kas -X nome-do-arquivo
   kas --export-all nome-do-arquivo

.. _header-n39:

Config
======

.. code:: 

   Abaixo é apresentado o conjuto de  diretórios e arquivos que compõem a aplicação

   access_functions	Armazena as conexões registradas
   ~/.local/share/acesso/	Armazena os arquivos de configuração da aplicação
   ~/.bashrc		Exportar o arquivo access_functions para o shell corrent
   ~/.zshrc		Exportar o arquivo access_functions para o shell corrente
   ~/.ssh/			Diretório utilizado para  acessar o par de chaves
   /usr/bin/		Diretório com  script executável
