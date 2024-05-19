# Desafio de Backend: Sistema de Gerenciamento de Caixas de Leite

**Objetivo**: Desenvolver uma API RESTful para gerenciar caixas de leite. A API deve permitir a criação, leitura, atualização e exclusão (CRUD) de caixas de leite.

#### Requisitos

1. **Modelo de Dados**:
    - **Caixa de Leite**:
        - `id` (inteiro, gerado automaticamente)
        - `marca` (string)
        - `volume` (inteiro, em mililitros)
        - `data_validade` (data)
        - `preco` (decimal)

2. **Endpoints da API**:

    - **Criar Caixa de Leite**:
        - **Método**: `POST`
        - **Rota**: `/caixas`
        - **Corpo da Requisição**:
            ```json
            {
                "marca": "string",
                "volume": "inteiro",
                "data_validade": "data",
                "preco": "decimal"
            }
            ```
        - **Resposta**:
            - **Código**: `201 Created`
            - **Corpo**:
                ```json
                {
                    "id": "inteiro",
                    "marca": "string",
                    "volume": "inteiro",
                    "data_validade": "data",
                    "preco": "decimal"
                }
                ```

    - **Listar Caixas de Leite**:
        - **Método**: `GET`
        - **Rota**: `/caixas`
        - **Resposta**:
            - **Código**: `200 OK`
            - **Corpo**:
                ```json
                [
                    {
                        "id": "inteiro",
                        "marca": "string",
                        "volume": "inteiro",
                        "data_validade": "data",
                        "preco": "decimal"
                    },
                    ...
                ]
                ```

    - **Obter Caixa de Leite por ID**:
        - **Método**: `GET`
        - **Rota**: `/caixas/{id}`
        - **Resposta**:
            - **Código**: `200 OK`
            - **Corpo**:
                ```json
                {
                    "id": "inteiro",
                    "marca": "string",
                    "volume": "inteiro",
                    "data_validade": "data",
                    "preco": "decimal"
                }
                ```

    - **Atualizar Caixa de Leite**:
        - **Método**: `PUT`
        - **Rota**: `/caixas/{id}`
        - **Corpo da Requisição**:
            ```json
            {
                "marca": "string",
                "volume": "inteiro",
                "data_validade": "data",
                "preco": "decimal"
            }
            ```
        - **Resposta**:
            - **Código**: `200 OK`
            - **Corpo**:
                ```json
                {
                    "id": "inteiro",
                    "marca": "string",
                    "volume": "inteiro",
                    "data_validade": "data",
                    "preco": "decimal"
                }
                ```

    - **Excluir Caixa de Leite**:
        - **Método**: `DELETE`
        - **Rota**: `/caixas/{id}`
        - **Resposta**:
            - **Código**: `204 No Content`

#### Tecnologias Sugeridas

- Linguagem: Python, JavaScript (Node.js), Java, ou qualquer outra linguagem com a qual você queira praticar.
- Frameworks: Flask ou Django para Python, Express para Node.js, Spring Boot para Java.
- Banco de Dados: SQLite, PostgreSQL, ou outro de sua preferência.
- Ferramentas adicionais: Docker (opcional), Postman para testar a API.

#### Tarefas Extras

- Implementar autenticação e autorização na API.
- Adicionar paginação na listagem de caixas de leite.
- Criar testes automatizados para os endpoints da API.
- Implementar validações nos campos do modelo de dados.

#### Entrega

- Código fonte hospedado em um repositório Git (GitHub, GitLab, etc.).
- Arquivo `README.md` com instruções sobre como configurar e executar o projeto.

Boa sorte e divirta-se com o desafio!
