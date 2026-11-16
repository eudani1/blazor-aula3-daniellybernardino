O FormProduto não adiciona o produto diretamente à lista porque sua responsabilidade é apenas exibir o formulário, validar os dados e comunicar o resultado.
Quem mantém a lista é a página Produtos.razor, que concentra o estado da tela.
Quando o cadastro é válido, o FormProduto dispara o EventCallback<Produto>, enviando o produto para a página.
A página recebe esse aviso no método AdicionarProduto e então inclui o produto na lista.
