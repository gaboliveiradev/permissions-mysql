# Como criar Usuários
```
CREATE USER 'nome_do_user'@'localhost' IDENTIFIED BY 'senha_do_user';
```

# Como Adicionar Previlégios a um Usuário
```
GRANT ALL PRIVILEGES ON nome_do_banco.* TO 'nome_do_user'@'localhost';
```

# Adicionando Insert, Update e Select ao Usuário
```
GRANT UPDATE, INSERT, SELECT ON nome_do_banco.* TO 'nome_do_user'@'localhost' IDENTIFIED BY 'senha_do_user';
```

# Como Remover Previlégios a um Usuário
```
REVOKE ALL, GRANT OPTION FROM 'nome_do_user'@'localhost';
```

# **ATENÇÃO - ATENÇÃO - ATENÇÃO - ATENÇÃO**
*Caso você tenha feito alguma alteração nos previlégios, utilize este comando:*
```
FLUSH PRIVILEGES;
```

# Lista de Previlégios
**ALL PRIVILEGES** <br> dá a um usuário do MySQL todo o acesso a uma determinada base de dados (ou se nenhuma base de dados for selecionada, todo o sistema)<br> <hr>
**DELETE** <br> permite deletar linhas das tabelas<br> <hr>
**INSERT** <br> permite inserir linhas nas tabelas<br> <hr>
**SELECT** <br> permite utilizar o comando select para ler bases de dados<br> <hr>
**UPDATE** <br> permite atualizar linhas das tabelas<br> <hr>
**CREATE** <br> permite criar novas tabelas ou bases de dados<br> <hr>
**DROP** <br> permite deletar tabelas ou bases de dados<br> <hr>
**GRANT OPTION** <br> permite conceder ou revogar privilégios de outros usuários<br>
