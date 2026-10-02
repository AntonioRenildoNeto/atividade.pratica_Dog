# atividade.pratica_Dog

Problemas identificados

Durante a análise do sistema, foram encontrados os seguintes pontos que precisam de correção:

1. O sistema impede o cadastro quando o nome do cliente está vazio, porém apresenta o problema somente por meio de um `alert`.

2. A verificação do e-mail possui uma validação básica, podendo permitir endereços que não são válidos.

3. Clientes cadastrados como VIP não recebem automaticamente o desconto de 15% previsto no sistema.

4. O cadastro de pets pode ser realizado sem que o tipo do animal seja informado.

5. A validação da idade do pet apresenta falhas e permite a entrada de valores que deveriam ser considerados inválidos.

6. É possível realizar o cadastro de um produto sem preencher o campo referente ao nome.

7. O sistema permite cadastrar produtos com preço igual a zero, apesar de esse valor não ser permitido.

8. Valores inválidos no campo de preço, como textos, não são tratados de forma adequada.

9. O carrinho permite a inclusão de produtos que possuem preço igual a zero.

10. A função de remoção do carrinho não identifica corretamente o produto selecionado, removendo sempre o primeiro item.

11. Antes de adicionar um produto ao carrinho, o sistema não realiza uma verificação adequada para confirmar se o produto é válido.

12. As regras responsáveis pelo funcionamento do sistema estão muito ligadas à parte visual, o que dificulta a realização de testes.

13. As funções utilizadas pelo sistema não estão devidamente exportadas no `app.js`, dificultando o acesso individual delas durante os testes com Jest.

14. O carrossel utiliza o `setInterval()` diretamente, tornando mais difícil realizar testes automatizados para verificar a alteração das imagens.

15. A funcionalidade do botão **Finalizar** depende do `alert()` e de um carrinho armazenado globalmente, dificultando a realização de testes isolados.
