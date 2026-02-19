# 👑 Rei da Chapa | Cardápio Digital

## 📚 Descrição do Projeto

O **Rei da Chapa | Cardápio Digital** é uma aplicação web desenvolvida como trabalho acadêmico com o objetivo de simular um sistema real de pedidos para lanchonetes.

O sistema permite que o cliente:

- Visualize o cardápio digital dividido por categorias  
- Adicione produtos ao carrinho  
- Personalize lanches com adicionais  
- Escolha forma de pagamento  
- Selecione entre entrega ou retirada  
- Envie o pedido diretamente para o WhatsApp do estabelecimento  

O projeto foi desenvolvido utilizando **HTML**, **CSS (TailwindCSS)** e **JavaScript puro**, sem utilização de frameworks ou back-end.

---

## 🎯 Objetivos Acadêmicos

Este trabalho teve como principais objetivos:

- Aplicar conceitos de desenvolvimento web front-end  
- Trabalhar manipulação de DOM com JavaScript  
- Implementar lógica de carrinho de compras  
- Desenvolver interface responsiva  
- Criar uma experiência de usuário intuitiva  
- Integrar a aplicação com a API do WhatsApp para envio de pedidos  

---

## 🛠 Tecnologias Utilizadas

- HTML5  
- CSS3  
- TailwindCSS (via CDN)  
- Font Awesome (ícones)  
- JavaScript (ES6)  
- API do WhatsApp (`https://api.whatsapp.com/send`)  

---

## 📱 Funcionalidades

### 🔎 1. Filtro por Categoria
O usuário pode filtrar os produtos pelas categorias:
- Todos  
- Sanduíches  
- Artesanais  
- Bebidas  

A filtragem é feita dinamicamente via JavaScript.

---

### 🛒 2. Carrinho de Compras

O carrinho permite:

- Adicionar produtos  
- Adicionar adicionais aos lanches  
- Selecionar opções em bebidas  
- Aumentar ou diminuir quantidade  
- Remover itens automaticamente ao zerar quantidade  
- Visualizar total atualizado em tempo real  

Cada item possui um `cartId` único gerado com `Date.now()`.

---

### 🍔 3. Sistema de Adicionais

Alguns produtos permitem personalização com adicionais como:

- Cheddar  
- Catupiry  
- Bacon  
- Hambúrguer  
- Ovo  

O valor final do produto é recalculado automaticamente com base nos adicionais selecionados.

---

### 🚚 4. Entrega ou Retirada

O cliente pode escolher entre:

- Entrega (exige endereço)
- Retirada (não exige endereço)

A interface altera dinamicamente os campos obrigatórios conforme a escolha.

---

### 💳 5. Forma de Pagamento

Opções disponíveis:

- Pix  
- Cartão  
- Dinheiro  

Caso a opção seja dinheiro, o cliente pode informar o valor para troco.

---

### 📲 6. Envio do Pedido via WhatsApp

Ao finalizar o pedido, o sistema:

1. Valida os campos obrigatórios  
2. Gera uma mensagem formatada automaticamente  
3. Redireciona para a API do WhatsApp  
4. Abre a conversa com o pedido preenchido  

Exemplo de estrutura enviada:

\`\`\`
👑 REI DA CHAPA - NOVO PEDIDO
TIPO: ENTREGA
CLIENTE: Nome
ENDEREÇO: Rua X

PEDIDO:
• 2x Rei Clássico (+ Bacon) - R$ 36,00

PAGAMENTO: Dinheiro
TROCO PARA: 50

TOTAL: R$ 36,00
\`\`\`

---

## 🎨 Design e Experiência do Usuário

O layout foi desenvolvido com foco em:

- Visual moderno e atrativo  
- Identidade visual forte (cores amarelo e laranja)  
- Responsividade para dispositivos móveis  
- Navegação simples e intuitiva  
- Animações suaves e efeitos visuais  

---

## 📂 Estrutura do Projeto

O projeto está contido em um único arquivo HTML, contendo:

- Estrutura da página (HTML)
- Estilização (Tailwind + CSS interno)
- Lógica da aplicação (JavaScript interno)

Principais funções JavaScript:

- \`renderProducts()\`
- \`openProductLogic()\`
- \`addToCart()\`
- \`updateCart()\`
- \`changeQty()\`
- \`sendOrder()\`

---

## 🔐 Validações Implementadas

O sistema impede o envio do pedido caso:

- O nome não seja preenchido  
- O endereço não seja informado (quando entrega)  
- O carrinho esteja vazio  

---

## 📈 Possíveis Melhorias Futuras

- Implementação de back-end com banco de dados  
- Painel administrativo para gestão de produtos  
- Sistema de login para clientes  
- Integração com pagamento online  
- Persistência do carrinho com LocalStorage  

---

## ✅ Conclusão

O projeto demonstra a aplicação prática de conceitos fundamentais de desenvolvimento web, como manipulação de DOM, lógica condicional, estruturação de layout responsivo e integração com serviços externos.

Além de cumprir os requisitos acadêmicos, o sistema simula uma aplicação real que poderia ser utilizada por pequenos estabelecimentos para digitalizar seus pedidos.

---

**Desenvolvido para fins acadêmicos.**
