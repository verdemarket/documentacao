# Documentacao     
1. [Verde market](https://github.com/verdemarket/documentacao/blob/main/verdemarket.xml)
2. [Cadastro](https://github.com/verdemarket/documentacao/blob/main/Cadastro.drawio)

API para envio de pedidos. Terá tratamento de prioritários e ordinarias

Pedidos de licitação terão um throughtput de milhões de registros por hora.

Terá serviço de entrega para 4 regiıes (ZN, ZL, ZO E ZS).

Será enviado uma notificação do pedido em questão.

Envio de relatórios para receita federal. Fiscal, Trabalhista.

Controle de Estoque

Seções do mercado:  
- Biscoitos  
- Limpeza  
- Frutas  
- Geladeiras  
- Bebidas  
- Carnes  


Todos os pedidos são gravados na base de dados Pedidos.  
O estoque é controlado pela base de dados Estoque. Ao efetuar a venda, é feito a propagação do evento para o controle do estoque.  
A consulta de estoque também é feita pelo controle de estoque.  

O envio de relatórios para a receita federal é feita lendo arquivos ao final do dia do repositório de arquivos.  
O arquivo é gerado ao término do dia e gravado em um arquivo txt.

