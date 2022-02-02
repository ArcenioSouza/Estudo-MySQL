# Estudo sobre a linguagem SQL aplicada ao MySQL

Esse repositório é para registrar comandos SQL para manipulação de dados em banco de dados relacionais. 
O intuito desse registro também é oferecer uma fonte de consulta para a comunidade.

## Database de exemplo

**database:** dezzer

**tabela:** musica

**exemplo da tabela**

| id | nome_musica |
|---:|-------------|
| 1  | Pais e filhos |

## Comandos de criação

*Criar um banco de dados*
```
CREATE DATABASE dezzer;
```

*Criar uma tabela*
```
CREATE TABLE 'musica' (
   'id' INT PRIMARY KEY,
   'nome_musica' TEXT
);
```

## Comandos de controle de transação

*Alternar o auto commit para ligado e desligado*
```
SET AUTOCOMMIT = 0; -- desligado
SET AUTOCOMMIT = 1; -- ligado
```

*Inicia o controle de transação, as mudanças só serão salvas se for feito um commit*
```
START TRANSACTION;
```

*Salva as mudanças no banco de dados*
```
COMMIT;
```

*Desfaz as mudanças voltando até o último commit*
```
ROLLBACK;
```

## Comandos de alteração

*Alterar tabela adicionando um atributo*
```
ALTER TABLE 'musica' ADD 'tempo' TIME;
```

*Alterar tabela removendo um atributo*
```
ALTER TABLE 'musica' DROP 'tempo';
```



