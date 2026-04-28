*Tema:* Plataforma de Aluguel - locadora de filmes, séries e games BLACK-BOX

O projeto visa organizar o acervo de filmes, séries e games para uma locadora, e gerenciar a logística de locação dos produtos para os clientes da locadora.

### Usuários
- Funcionário


---

## 2. Requisitos Funcionais (RF)

- *RF01* - O sistema deve permitir o cadastro de novos produtos (create)
- *RF02* - O sistema deve permitir o cadastro de novos clientes (create)
- *RF03* - O sistema deve exibir cliente cadastrado (list)
- *RF04* - O sistema deve alterar informações do cliente (update)
- *RF05* - O sistema deve exibir produtos cadastrados (list)
- *RF06* - O sistema deve exibir o histórico de alugueis do cliente (list)
- *RF07* - O sistema deve permitir deletar produtos (delete)
- *RF08* - O sistema deve exibir o status do produto (alugado, devolvido) (list)


---

## 3. Requisitos Não Funcionais (RNF)

- *RNF01* - A API deve ser desenvolvida em Node.js com TypeScript
- *RNF02* - A API deve ser integrada com banco de dados
- *RNF03* - A API deve usar a biblioteca typeORM
- *RNF04* - A API deve seguir o padrão MVC


---

## 4. Regras de Negócio (RN)

- *RN01* - Não é permitido excluir um produto que tenha aluguel vinculados.
- *RN02* - O CPF do cliente deve ter no mínimo 11 caracteres.
- *RN03* - Os produtos só podem ser alugados para clientes cadastrados.
- *RN04* - Deve haver um histórico dos produtos alugados.
- *RN05* - Caso o prazo de devolução seja excedido será renovado a locação.
