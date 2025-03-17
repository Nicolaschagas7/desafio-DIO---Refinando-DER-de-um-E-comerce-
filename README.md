# desafio da DIO Refinando projeto conceitual de um E-comerce

## **Descrição do Projeto**  
Este projeto apresenta um **Modelo Entidade-Relacionamento Aprimorado (MER)** para um sistema de **e-commerce**, que foi inicialmente desenvolvido pela instrutora juliana e aprimorado como parte do **desafio "Refinando um Projeto Conceitual de Banco de Dados – E-COMMERCE" ofertado pela Digital inovation one(DIO)**. O objetivo do modelo é organizar a estrutura do banco de dados para gerenciar clientes, pedidos, produtos, fornecedores, estoque, pagamentos e entregas de forma eficiente.  

O aprimoramento realizado incluiu:  
- **Criação da entidade "Pagamentos"** para registrar os detalhes das transações realizadas pelos clientes.  
- **Criação da entidade "Entregas"**, permitindo armazenar informações logísticas dos pedidos.  
- **Implementação de uma diferenciação entre clientes "Pessoa Física" e "Pessoa Jurídica"**, garantindo que um cliente só possa ser um dos dois tipos, nunca ambos.  

---

## **Contextualização do Modelo**  

O modelo reflete a operação de um sistema de e-commerce, estruturado da seguinte forma:  

1. **Cadastro de Clientes**  
   - Um cliente pode ser **Pessoa Física** ou **Pessoa Jurídica**, mas nunca ambos.  
   - Os clientes realizam pedidos e registram pagamentos.  

2. **Gerenciamento de Pedidos e Produtos**  
   - Cada pedido está vinculado a um cliente e pode conter múltiplos produtos.  
   - Os produtos possuem categorias e informações específicas.  

3. **Gestão de Fornecedores e Estoque**  
   - A entidade **"Fornecedor"** armazena informações sobre as empresas que fornecem os produtos.  
   - A entidade **"Estoque"** gerencia a localização e disponibilidade dos produtos no armazém.  

4. **Processo de Pagamento e Entrega**  
   - A entidade **"Pagamentos"** foi criada para registrar os métodos de pagamento e seus detalhes, relacionando-se diretamente com a entidade **"Forma de Pagamento"**.  
   - A entidade **"Entregas"** foi adicionada para acompanhar o status da logística do pedido, garantindo que cada pedido tenha informações de entrega associadas.  

---

## **Estrutura do Modelo**  

### **Entidades e Relacionamentos**  
O modelo aprimorado possui as seguintes entidades:  

- **Cliente** → Pode ser **Pessoa Física** ou **Pessoa Jurídica**, mas não ambos.  
- **Pedido** → Vinculado a um cliente e pode conter vários produtos.  
- **Produto** → Associado a categorias e presente em múltiplos pedidos.  
- **Fornecedor** → Armazena informações sobre as empresas fornecedoras dos produtos.  
- **Estoque** → Gerencia a localização e disponibilidade dos produtos no armazém.  
- **Forma de Pagamento** → Define os tipos de pagamento disponíveis.  
- **Pagamentos** → Registra os métodos e detalhes da transação do pedido, relacionando-se com **Forma de Pagamento**.  
- **Entregas** → Contém informações logísticas e status da entrega do pedido.  

---

## **Entrega**  

### **Arquivos no Repositório**  
1. **Diagrama (PNG/PDF)** → Contém o modelo final aprimorado do MER.  
2. **README.md** (este arquivo) → Explicação do contexto, estrutura e melhorias aplicadas ao modelo.  

---

## **Como Utilizar**  

1. Clone este repositório.  
2. Abra o arquivo do diagrama (PNG/PDF) para visualizar o modelo entidade-relacionamento.  
3. Consulte o `README.md` para entender a estrutura e as decisões de modelagem.  

---

## **Contribuições**  

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests para sugerir melhorias ou correções.  
