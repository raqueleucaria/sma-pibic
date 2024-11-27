# BookTrading
### Classes
1. BookBuyerAgent
   - Vendedor 
   - Possui uma tela para cadastrar livros à venda
2. BookSellerAgent
   - Comprador 
   - Ao ser executado, passa como paramêtro o nome do livro que deseja
3. BookSellerGui
   - Interface gráfica do vendedor

### Passos
1. Criar o primeiro agente com o comando para abrir a interface do prório jade
   - Name: `JADE_BookTradingSeller1`
   - Project: `bookTrading`
   - Arguments: `-gui -local-host 127.0.0.1 -local-port 1099 seller1:BookSellerAgent`
   - Cadastrar o nome do livro e preço
2. Cria um ou mais agentes para ter concorrência
   - Name: `JADE_BookTradingSeller2`
   - Project: `bookTrading`
   - Arguments: `-container seller2:BookSellerAgent` 
   - Cadastrar o nome do livro e preço
3. Tentar fazer uma comprar como comprador
   - Name: `JADE_BookTradingBuyer1`
   - Project: `bookTrading`
   - Arguments: `-container buyer1:BookBuyerAgent(SenhorDosAneis)` 
   - A classe foi criada para passar o nome do livro

### Resultados


### Análise das classes