# CREATE e INSERT

## Tabela Cliente

#### CREATE TABLE cliente (id INTEGER, nome VARCHAR(100), sobrenome VARCHAR(100));
#### INSERT INTO cliente (id, nome, sobrenome) VALUES (1, 'João', 'Melo');
#### INSERT INTO cliente (id, nome, sobrenome) VALUES (2, 'Pedro', 'Silva');
#### INSERT INTO cliente (id, nome, sobrenome) VALUES (3, 'Maria', 'Bezerra');

## Tabela Produto

#### CREATE TABLE produto (id INTEGER, descricao VARCHAR(100));
#### INSERT INTO produto (id, descricao) VALUES (1, 'Arroz');
#### INSERT INTO produto (id, descricao) VALUES (2, 'Feijão');

## Tabela Fornecedor
                                                
#### CREATE TABLE fornecedor (id INTEGER, nome VARCHAR(100));                                             
#### INSERT INTO fornecedor (id, nome) VALUES (1, 'Turquesa');
#### INSERT INTO fornecedor (id, nome) VALUES (2, 'Emoções');   

## Tabela Produto_Fornecedor
    
#### CREATE TABLE produto_fornecedor (id INTEGER, produto_id INTEGER, fornecedor_id INTEGER);
#### INSERT INTO produto_fornecedor (id, produto_id, fornecedor_id) VALUES (1, 1, 2);
#### INSERT INTO produto_fornecedor (id, produto_id, fornecedor_id) VALUES (2, 2, 1);

## Tabela Estoque
    
#### CREATE TABLE estoque (id INTEGER, produto_id INTEGER, quantidade INTEGER);
#### INSERT INTO estoque (id, produto_id, quantidade) VALUES (1, 1, 100);
#### INSERT INTO estoque (id, produto_id, quantidade) VALUES (2, 2, 200);

## Tabela Vendedor
    
#### CREATE TABLE vendedor (id INTEGER, nome VARCHAR(100), sobrenome VARCHAR(100));
#### INSERT INTO vendedor (id, nome, sobrenome) VALUES (1, 'Alberto', 'Vieira');
#### INSERT INTO vendedor (id, nome, sobrenome) VALUES (2, 'Carlos', 'Chagas');

## Tabela Pedido
    
#### CREATE TABLE pedido (id INTEGER, cliente_id INTEGER, vendedor_id INTEGER);
#### INSERT INTO pedido (id, cliente_id, vendedor_id) VALUES (1, 2, 1);
#### INSERT INTO pedido (id, cliente_id, vendedor_id) VALUES (2, 3, 1);

## Tabela Item_Pedido
    
#### CREATE TABLE item_pedido (id INTEGER, pedido_id INTEGER, produto_id INTEGER, quantidade INTEGER, valor_unitario DECIMAL);
#### INSERT INTO item_pedido (id, pedido_id, produto_id, quantidade, valor_unitario) VALUES (1, 1, 1, 10, 5.00);
#### INSERT INTO item_pedido (id, pedido_id, produto_id, quantidade, valor_unitario) VALUES (2, 1, 2, 5, 6.00);
#### INSERT INTO item_pedido (id, pedido_id, produto_id, quantidade, valor_unitario) VALUES (3, 2, 1, 2, 5.50);
#### INSERT INTO item_pedido (id, pedido_id, produto_id, quantidade, valor_unitario) VALUES (4, 2, 2, 3, 6.00);

# SELECT SIMPLES

#### SELECT * FROM cliente;

<table><thead><tr><td>id</td><td>nome</td><td>sobrenome</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>João</span></td><td><span>Melo</span></td></tr><tr><td><span>2</span></td><td><span>Pedro</span></td><td><span>Silva</span></td></tr><tr><td><span>3</span></td><td><span>Maria</span></td><td><span>Bezerra</span></td></tr></tbody></table>

#### SELECT * FROM produto;

<table><thead><tr><td>id</td><td>descricao</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>Arroz</span></td></tr><tr><td><span>2</span></td><td><span>Feijão</span></td></tr></tbody></table>

#### SELECT * FROM fornecedor;

<table><thead><tr><td>id</td><td>nome</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>Turquesa</span></td></tr><tr><td><span>2</span></td><td><span>Emoções</span></td></tr></tbody></table>

#### SELECT * FROM produto_fornecedor;

<table><thead><tr><td>id</td><td>produto_id</td><td>fornecedor_id</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>1</span></td><td><span>2</span></td></tr><tr><td><span>2</span></td><td><span>2</span></td><td><span>1</span></td></tr></tbody></table>

#### SELECT * FROM estoque;

<table><thead><tr><td>id</td><td>produto_id</td><td>quantidade</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>1</span></td><td><span>100</span></td></tr><tr><td><span>2</span></td><td><span>2</span></td><td><span>200</span></td></tr></tbody></table>

#### SELECT * FROM vendedor;

<table><thead><tr><td>id</td><td>nome</td><td>sobrenome</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>Alberto</span></td><td><span>Vieira</span></td></tr><tr><td><span>2</span></td><td><span>Carlos</span></td><td><span>Chagas</span></td></tr></tbody></table>

#### SELECT * FROM pedido;

<table><thead><tr><td>id</td><td>cliente_id</td><td>vendedor_id</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>2</span></td><td><span>1</span></td></tr><tr><td><span>2</span></td><td><span>3</span></td><td><span>1</span></td></tr></tbody></table>

#### SELECT * FROM item_pedido;

<table><thead><tr><td>id</td><td>pedido_id</td><td>produto_id</td><td>quantidade</td><td>valor_unitario</td></tr></thead><tbody><tr><td><span>1</span></td><td><span>1</span></td><td><span>1</span></td><td><span>10</span></td><td><span>5.00</span></td></tr><tr><td><span>2</span></td><td><span>1</span></td><td><span>2</span></td><td><span>5</span></td><td><span>6.00</span></td></tr><tr><td><span>3</span></td><td><span>2</span></td><td><span>1</span></td><td><span>2</span></td><td><span>5.50</span></td></tr><tr><td><span>4</span></td><td><span>2</span></td><td><span>2</span></td><td><span>3</span></td><td><span>6.00</span></td></tr></tbody></table>
