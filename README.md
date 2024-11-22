# Exemplo de Tabela Fictícia: `clientes`

## Estrutura da Tabela
```sql
CREATE TABLE clientes (
    id INT PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(100),
    email VARCHAR(100),
    telefone VARCHAR(15),
    data_cadastro DATE
);

```

## Operações CRUD
### 1. Criar (Create)
Adicionar um cliente a tabela.
``` sql
INSERT INTO clientes (nome, email, telefone, data_cadastro) VALUES 
('João Silva', 'joao.silva@email.com', '11999998888', CURDATE());

```
### 2. Selecionar (Read)
Lê as informações de um cliente com base no ID.
``` sql
SELECT * FROM clientes WHERE id = 1;

```
### 3. Editar (Update)
Atualiza as informações de um cliente com base no ID.
``` sql
UPDATE clientes 
SET telefone = '11988887777', email = 'joao.silva@novoemail.com' 
WHERE id = 1;

```
### 4. Apagar (Delete)
Remove um cliente da tabela
``` sql
DELETE FROM clientes WHERE id = 1;
```







