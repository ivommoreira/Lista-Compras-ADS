## Sobre

Antes de iniciar, precisamos executar algumas configurações do CodeIgniter para funcionar localmente.

### Trocar os arquivos no caminho `application/config/`

#### config.php
```[26] $config['base_url'] = 'http://localhost/lista_de_compras/';```
Troque pela URL do seu projeto

#### database.php
```
$db['default'] = array(
		'dsn'	=> '',
		'hostname' => 'localhost',
		'username' => 'root',
		'password' => '',
		'database' => 'mercado',
		'dbdriver' => 'mysqli',
		'dbprefix' => '',
		'pconnect' => FALSE,
		'db_debug' => (ENVIRONMENT !== 'production'),
		'cache_on' => FALSE,
		'cachedir' => '',
		'char_set' => 'utf8',
		'dbcollat' => 'utf8_general_ci',
		'swap_pre' => '',
		'encrypt' => FALSE,
		'compress' => FALSE,
		'stricton' => FALSE,
		'failover' => array(),
		'save_queries' => TRUE
);
```
Mude o hostname username e database com os seus dados para conexão com seu banco local<br>
O arquivo sql está no caminho `database/banco.sql`

<h3 align="center">ENDPOINTS</h3>

#### Substitua a {{URL}} pela url definida acima
``` 
http://localhost/mercado/api
```

#### Header das requisições
	Content-Type: application/json

----

#### Programador 

Aluno: Ivo Manoel Moreira

