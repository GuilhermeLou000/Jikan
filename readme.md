# Introdução

Neste trabalho de aprendizagem que foi passado para mim pelo meu atual orientador em JavaScrpit([Fernando Leonid](https://github.com/fernandoleonid)) eu utilizei de uma API chamada Jikan que também é usada no site nomeado MyAnimeList, consumindo está API eu utilizei de algumas funções para montar um card para cada anime que tivesse uma parte do nome que foi pesquisado, por exemplo: Pesquisando "Akame ga Kill" o sistema vai te retornar 50 possiveis resultados que contem uma das palavras que foram colocadas em seu nome, isto tem um certo incomodo por aparecer sempre um alto numero de respostas mas isto acaba auxiliando você a encontrar algo que não sabe o exato nome.

# Possíveis Problemas

Esta API consiste de varios tipos e generos de animes por isto acaba tendo uma grande variedade d pesquisas, mas por algumas limitações esta API não consegue fazer uma pesquisa que possua filtros, este é um dos problemas que podem ser apresentados que atualmente não encontrei solução mas achei interessante o listar para que alguém possa o resolver. Em alguns momentos o site acaba tendo um erro pela velocidade da pesquisa, por isto as pesquisas tem que ter ao menos um pequeno intervalo de 20 segundos. Também a um problema que se relaciona a pesquisas, não há como buscar um anime colocando menos que três caracteres. 

# API, passo a passo.

Para consumir está API eu precisei fazer os seguintes passos:

- **1.** Eu requisitei do HTML o que foi escrito no input text utilizando o botão como o ativador da função.

- **2.** Depois de ter pego o nome do que foi escrito eu utilizei da URL que foi disponibilizada na [documentação da API](https://jikan.docs.apiary.io/#).

- **3.** Eu transformei está url em Json utilizando de um método que vai receber o nome do Anime o adicionando da URL.

- **4.** Utilizando da função que faz a pesquisa da URL e retorna as informações de uma lista de animes eu chamo uma função que cria os cards e adiciona todos no HTML com nome, imagem e os linkando ao site que vai abrir caso clique.

# Conclusão

É necessária uma atenção quando se trata da pesquisa deste site, há alguns erros a serem corrigidos e tratados mas são coisas pouco relevantes que atualmente não vão interfirir em nada quando se trata da devida execução deste site. Não há nenhuma primeira exibição no site quando ele é aberto mas isto é algo que acreditei não ser totalmente relevante já que o prórpio usuário vai pesquisar o que ele necessita. (Obs: Na pesquisa é possível apenas fazer pesquisas usando o nome em japonês)