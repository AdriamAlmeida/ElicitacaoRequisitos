## História 1 - Acompanhamento do pedido

**Como** usuário, **quero** ser notificado para acompanhar o pedido depois de fazer a compra, **para que** eu saiba em que etapa ele está.

**Critérios de aceitação:**
1. Dado que fiz o pagamento, quando o pedido for confirmado, então preciso acompanhar quando ele estiver sendo preparado, quando sair para entrega e quando for entregue.
2. Dado que o pedido já foi preparado, quando ele sair para entrega, então devo ser avisado de que logo será entregue.

### RNFs

| RNF | Característica ISO/IEC 25010 |
|---|---|---|
| 1 | A atualização do status do pedido deve ser refletida na tela do usuário em no máximo 5 segundos após a mudança no backend. | **Eficiência de desempenho** (Performance Efficiency) |
| 2 | A tela de acompanhamento do pedido deve ser compreensível sem necessidade de tutorial, seguindo um fluxo visual intuitivo. | **Usabilidade** (Usability) |
| 3 | A funcionalidade de acompanhamento de pedidos deve estar disponível 99,5% do tempo, mesmo em picos de acesso. | **Confiabilidade** (Reliability) |

---

## História 2 - Item indisponível no cardápio

**Como** dono do restaurante, **quero** avisar quando um item do cardápio fica indisponível, **para que** não haja transtornos com os clientes.

**Critérios de aceitação:**
1. Dado que o item está fora do estoque, quando eu marcar essa condição no sistema, então preciso deixar meus clientes cientes de que ele não está disponível.
2. Dado que um item foi marcado como indisponível, quando um cliente tentar pedi-lo, então o sistema deve impedir a adição ao carrinho.

### RNFs

| RNF | Característica ISO/IEC 25010 |
|---|---|---|
| 1 | Apenas usuários autenticados com perfil de restaurante devem poder alterar a disponibilidade de um item. | **Segurança** (Security) |
| 2 | A funcionalidade de marcar/desmarcar disponibilidade deve ser implementada como um módulo isolado, facilitando testes e manutenção futura. | **Manutenibilidade** (Maintainability) |
| 3 | A alteração de disponibilidade de um item deve ser sincronizada de forma consistente entre a versão web e a versão mobile do aplicativo. | **Compatibilidade** (Compatibility) |

---

## História 3 - Reportar problema na entrega

**Como** entregador, **quero** reportar um erro que tive durante a entrega, **para que** seja corrigido o quanto antes e não ocorra novamente.

**Critérios de aceitação:**
1. Dado que o erro foi apresentado, quando eu estiver fazendo a entrega do pedido do cliente, então é necessário registrar o problema para que uma equipe especializada faça a correção.
2. Dado que o problema foi registrado, quando eu enviar o relato, então o suporte deve recebê-lo com os detalhes do pedido e da ocorrência.

### RNFs

| RNF | Característica ISO/IEC 25010 |
|---|---|---|
| 1 | O envio do relato de problema deve ser reenviado automaticamente em caso de falha de conexão, garantindo que não se perca mesmo com internet instável. | **Confiabilidade** (Reliability) |
| 2 | O processo de reportar um problema não deve exigir mais do que 3 toques na tela do entregador. | **Usabilidade** (Usability) |
| 3 | A funcionalidade de report deve funcionar corretamente nas diferentes versões de Android e iOS utilizadas pelos entregadores. | **Portabilidade** (Portability) |