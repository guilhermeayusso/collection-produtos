# Postman Collection - Microsserviço de Produtos

Esta é uma coleção de requests do Postman para o microsserviço de produtos. A coleção inclui requisições para criar, buscar, atualizar e deletar produtos.

## Requisitos

- [Postman](https://www.postman.com/downloads/)

## Importando a Coleção

1. Baixe a coleção do [repositório do GitHub](https://github.com/guilhermeayusso/produtos/tree/feature/criando-api-produtos).
2. Abra o Postman.
3. Vá para `File -> Import`.
4. Selecione o arquivo `Microsserviço de Produtos.postman_collection.json`.

## Endpoints

### Cadastrar Produto

- **Método:** POST
- **URL:** `http://localhost:8080/api/v1/produtos`
- **Body:**
  ```json
  {
    "nome": "Câmera Digital ProShot",
    "preco": 1200.00,
    "descricao": "Câmera digital com lentes intercambiáveis e vídeo em resolução 4K.",
    "quantidadeEmEstoque": 8
  }
  ```

### Buscar Todos os Produtos
- **Método:** GET
- **URL:** http://localhost:8080/api/v1/produtos

### Buscar Produto por ID
- **Método:** GET
- **URL:** http://localhost:8080/api/v1/produtos/{id}

### Buscar Produto por Nome
- **Método:** GET
- **URL:** http://localhost:8080/api/v1/produtos/buscar-por-nome/{nome}

## Deletar Produto
- **Método:** DELETE
- **URL:** http://localhost:8080/api/v1/produtos/{id}

## Estrutura da Coleção

## A coleção contém os seguintes endpoints:

- Cadastrar Produto: Cria um novo produto no sistema.
- Buscar Todos os Produtos: Retorna todos os produtos cadastrados.
- Buscar Por ID: Retorna um produto específico pelo seu ID.
- Buscar Por Nome: Retorna produtos que correspondem ao nome fornecido.
- Deletar Produto: Remove um produto específico pelo seu ID.
