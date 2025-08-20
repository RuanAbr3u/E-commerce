# 📦 Projeto de Modelagem Conceitual – E-commerce

## 📝 Descrição
Este projeto apresenta a modelagem conceitual de um **sistema de e-commerce**, contemplando as principais entidades e relacionamentos que suportam o processo de compra, pagamento e entrega de produtos.

O modelo foi elaborado para atender às regras de negócio propostas no desafio, garantindo consistência e flexibilidade na gestão dos dados.

---

## 🎯 Regras de Negócio Implementadas

1. **Clientes (PF e PJ)**  
   - O sistema diferencia clientes do tipo **Pessoa Física (PF)** e **Pessoa Jurídica (PJ)**.  
   - Cada cliente só pode ser **um tipo** (PF ou PJ), garantindo exclusividade das informações.  

2. **Formas de Pagamento**  
   - Um pedido pode ter **mais de uma forma de pagamento cadastrada** (PIX, Boleto, Cartão de Crédito).  
   - A entidade **Aprovação** foi criada para controlar o **status do pagamento** associado a cada forma de pagamento.  

3. **Entrega**  
   - Todo pedido gera uma entrega vinculada.  
   - A entidade **Entrega** contém:  
     - **Status** (ex.: aguardando envio, em transporte, entregue).  
     - **Código de rastreio** para acompanhamento logístico.  

---

## 📊 Estrutura Conceitual

- **Cliente PF**: Nome, CPF, Endereço, Email.  
- **Cliente PJ**: Razão Social, CNPJ, Endereço, Email.  
- **Pedido**: status, descrição, frete, valor total, vínculo com cliente.  
- **Forma de Pagamento**: PIX, Boleto, Cartão de Crédito.  
- **Aprovação**: controla status do pagamento e vínculo com entrega.  
- **Entrega**: status e código de rastreio.  
- **Produto**: categoria, descrição, valor.  
- **Relação Pedido–Produto**: quantidade de cada item no pedido.  
- **Estoque e Fornecedores**: controle de disponibilidade de produtos.  
- **Devolução**: registro de prazos e motivos de devoluções.  

---

## ✅ Conclusão
O modelo conceitual atende aos requisitos do desafio:  
- Diferenciação de clientes PF e PJ;  
- Pedido com múltiplas formas de pagamento;  
- Entrega com status e código de rastreamento.  

Este esquema fornece uma base sólida para a implementação futura do banco de dados de um sistema de e-commerce.
