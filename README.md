# GRAYLOG 6
Scripts para ajudar na gerencia/administração do graylog por linha de comando.

Caminhos:
* /usr/local/sbin/graylogctl
* /etc/bash_completion.d/graylogctl_completion

OBS: Foram usados comandos basicos e somente 1 index_set

# graylogctl
Script com diversos comandos/opções para a gerencia/administração do graylog por linha de comando.

 Comandos:
           
      iniciar       - Inicia o serviço do graylog-server ou mongodb.
      parar         - Para o serviço do graylog-server ou mongodb.
      reiniciar	- Para/Inicia o serviço do graylog-server ou mongodb.
      criar         - Cria uma stream ou role padrão.
      excluir       - Excluir uma stream.
      listar        - Lista as streams, roles, index_sets ou tipos de permissões.


 Opções dos comandos:
            
      criar [tipo] [nomeapl] <usuarios>
      
      onde:
        tipo:	Deve informar [streams] ou [rolepadrao].
        nomeapl:	Nome da stream que será criada.
        usuarios:	Login do(s) usuario(s) do AD separado por virgula.
        
      excluir [nome]
      Informar o nome da stream para a exclusão. Roles não serão excluidas.
      
      onde:
        nome: Nome da stream que será excluida.
        
      listar [tipo]
      Informar o tipo para a ação solicitada.

      onde:
        tipo: Deve informar [streams|roles|index_sets|permissions].

# graylogctl_completion
Script para o autocompletar do graylogctl

