Atividade prática estagiário TI – Banco do Brasil

Esta atividade tem por objetivo avaliar o conhecimento do candidato em estrutura de dados por meio do desenvolvimento de um programa para cadastro de clientes.
A linguagem de programação para criação do programa, fica a critério do candidato. Na resposta deve ser informada a linguagem utilizada para elaboração do programa.

Programa

O programa precisa armazenar em memória os dados de um cliente com as seguintes características:
	Nome do tipo texto;
	Data de nascimento do tipo date;
	Dois endereços um do tipo comercial e outro tipo residencial.

Cada endereço deve ter:
	Logradouro do tipo texto;
	Bairro do tipo texto;
	Cep do tipo texto;
	Cidade do tipo texto;
	Tipo endereço (comercial ou residencial) do tipo enum ou outro tipo de dado ou objeto estático que a linguagem permita.

Atribuição / instanciação dos dados

Os dados podem ser atribuídos ou instanciados diretamente no código ou via entrada manual no terminal (console).
Após atribuídos os respectivos valores, o programa deve mostrar no terminal:
	O nome do cliente;
	Os dois endereços do cliente identificando claramente o endereço residencial e o endereço comercial, juntamente com os demais dados do endereço;
	E a idade do cliente (o programa deve armazenar a data de nascimento em memória, porém deve mostrar na tela a idade do cliente na data de hoje, baseado na data de nascimento).

Banco de dados

Baseado nas informações anteriores do programa, formular três queries SQL, de acordo com as informações abaixo:
Tabela1 Cliente:
	Coluna id_cliente do tipo Integer (primary key);
	Coluna nome do tipo varchar;
	Coluna data_nascimento do tipo date.

Tabela2 Endereco:
	Coluna id_endereco do tipo Integer (primary key);
	Coluna logradouro do tipo varchar;
	Coluna cep do tipo varchar;
	Coluna cidade do tipo varchar;
	Coluna tipo_endereco do tipo enum (comercial, residencial);
	Coluna cliente_id (FK id_cliente).

Query 1:
	Retornar 1 resultado com o nome, data de nascimento e endereço residencial com logradouro, cep, bairro e cidade do cliente id número 1.

Query 2: 
	Retornar 1 resultado com o nome, data de nascimento e endereço comercial com logradouro, cep, bairro e cidade do cliente id número 1.

Query 3:
	Retornar todos resultados com o nome, data de nascimento e todos os endereços com logradouro, cep, bairro e cidade do cliente id número 1.

O arquivo com o programa, deve ser colocado no GitHub do candidato (se não tiver cadastro deve cadastrar-se) como projeto público e o link deve ser enviado para avaliação.
