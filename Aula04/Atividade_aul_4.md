## Processo 1 - Vendedores registrarem pedidos

**Requisito 1.** O sistema deve permitir registrar pedidos feitos por telefone ou em encontros presenciais, indicando o canal utilizado na venda.
Fonte A: Entrevista com o vendedor. Fonte humana, nível operacional, classe de usuário vendedor.
Fonte B: Política comercial da empresa sobre os canais de venda aceitos. Fonte não humana, categoria documentação.

**Requisito 2.** O sistema deve registrar, para cada pedido, os produtos escolhidos, as quantidades e o preço praticado no momento da venda.
Fonte A: Entrevista com o vendedor. Fonte humana, nível operacional, classe de usuário vendedor.
Fonte 2: Planilha atualmente usada para controle manual de vendas. Fonte não humana, categoria sistema legado.

**Requisito 3.** O sistema deve validar se há quantidade suficiente em estoque antes de confirmar um pedido.
Fonte A: Entrevista com o time de estoque. Fonte humana, nível operacional, classe de usuário estoquista.
Fonte B: Análise de sistemas concorrentes de vendas com controle de estoque integrado. Fonte não humana, categoria concorrência.

---

## Processo 2 - Administrador cadastrar e remover produtos

**Requisito 1.** O sistema deve permitir ao administrador cadastrar um novo produto informando nome, descrição, preço e categoria.
Fonte A: Entrevista com o administrador. Fonte humana, nível tático.
Fonte B: Catálogo de produtos atualmente utilizado pela empresa. Fonte não humana, categoria documentação.

**Requisito 2.** O sistema deve permitir a remoção ou inativação de produtos que deixaram de ser vendidos.
Fonte A: Entrevista com o administrador. Fonte humana, nível tático.
Fonte B: Planilha antiga de cadastro de produtos. Fonte não humana, categoria sistema legado.

**Requisito 3.** O sistema deve impedir a remoção de um produto que possua pedidos pendentes vinculados a ele
Fonte A: Reunião com a diretoria da empresa. Fonte humana, nível estratégico.
Fonte B: Boas práticas de integridade de dados em sistemas de gestão. Fonte não humana, categoria norma.

---

## Processo 3 - Time de estoque controlar a quantidade disponível

**Requisito 1.** O sistema deve dar baixa automática no estoque assim que um pedido for confirmado por um vendedor
Fonte A: Entrevista com o time de estoque. Fonte humana, nível operacional, classe de usuário estoquista.
Fonte B: Fluxo atual de controle de estoque feito em planilha manual. Fonte não humana, categoria sistema legado.

**Requisito 2.** O sistema deve permitir registrar entradas de novos lotes de produtos, atualizando automaticamente a quantidade disponível.
Fonte A: Entrevista com o time de estoque. Fonte humana, nível operacional, classe de usuário estoquista.
Fonte B: Notas fiscais de fornecedores. Fonte não humana, categoria documentação.

**Requisito 3.** O sistema deve emitir um alerta quando a quantidade de um produto atingir o nível mínimo de estoque definido.
Fonte A: Reunião com o gerente de estoque. Fonte humana, nível tático.
Fonte B: Estudo de sistemas de gestão de estoque concorrentes que utilizam alertas de reposição automática. Fonte não humana, categoria concorrência.