# GRAYLOG 6
Scripts para ajudar na gerencia/administração do graylog por linha de comando.

# graylogctl
Script com diversos comandos/opções para a gerencia/administração do graylog por linha de comando.

 Comandos:<br>
 * <strong>iniciar</strong>   - Inicia o serviço do graylog-server ou mongodb.<br>
 * <strong>parar</strong>     - Para o serviço do graylog-server ou mongodb.<br>
 * <strong>reiniciar</strong>	- Para/Inicia o serviço do graylog-server ou mongodb.<br>
 * <strong>criar</strong>     - Cria uma stream ou role padrão.<br>
 * <strong>excluir</strong>   - Excluir uma stream.<br>
 * <strong>listar</strong>    - Lista as streams, roles, index_sets ou tipos de permissões.<br><br>

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

# graylogctl_competion
Script para o autocompletar do graylogctl

