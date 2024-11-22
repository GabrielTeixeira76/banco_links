# banco_links

# Interfaces

A interface `IBancoLink.java` define 4 métodos principais:

- `adicionarLink`: Adiciona um novo link ao sistema, recebendo o assunto e a URL;
- `listarLinks`: Exibe todos os links cadastrados no sistema;
- `editarLink`: Permite editar um link existente, fornecendo o ID, assunto e URL;
- `deletarLink`: Remove um link do sistema com base no ID fornecido.

# `links.txt`

O arquivo links.txt armazena os links cadastrados, onde cada linha é separada por | representando respectivamente o ID, o assunto e a URL de cada link.

# `BancoLink`

A classe `BancoLink` implementa as operações de CRUD (Criar, Ler, Atualizar e Deletar) para os links. Ela também inclui um método chamado `obterUltimoId`, que é responsável por gerar o próximo ID para um link, com base no último ID registrado. Isso assegura que a sequência de IDs seja mantida, mesmo após o encerramento e reinício do programa.

# `TesteBancoLink`

A classe `TesteBancoLink` é onde ocorre a interação com o usuário. Ela apresenta um menu com as seguintes opções:

- Adicionar link
- Listar links
- Editar link
- Deletar link
- Sair
