---
layout: default
title: Mesa Aberta
permalink: /sobre.html
Cardápios para todos. Aplicativo que permite a qualquer restaurante montar um cardápio acessível.
Abrir o aplicativo
Sobre o projeto
Cardápios impressos costumam ter letra pequena, cores de baixo contraste e nenhuma versão em braille, em Libras ou em linguagem simples. Para pessoas cegas, com baixa visão, daltonismo, surdez ou dificuldade de leitura, isso significa depender de outra pessoa para escolher o que comer. Do lado dos restaurantes, falta ferramenta e conhecimento: poucos sabem como converter um cardápio para braille ou que contraste usar.
O Mesa Aberta resolve os dois lados. O restaurante preenche as informações dos pratos uma única vez e o aplicativo guia o dono por sete etapas, gerando as versões acessíveis do cardápio, sem exigir conhecimento técnico em acessibilidade.
Acesse o protótipo: https://mayaralmeidassis.github.io/mesa-aberta/
Funciona no navegador do computador ou do celular, sem instalar nada. Também dá para abrir pelo QR Code:
<img src="img/qrcode.png" alt="QR Code que abre o aplicativo Mesa Aberta" width="180">
Como funciona: 7 etapas
Etapa	O que o restaurante faz	Quem se beneficia
1. Informações básicas	Cadastra nome, ingredientes e preço dos pratos	Todos os clientes
2. Alérgenos	Marca os alérgenos de cada prato e o que pode conter por contato na cozinha	Pessoas com alergia alimentar ou doença celíaca
3. Contraste e cores	Escolhe o esquema de cores e o tamanho da letra	Pessoas com baixa visão e daltonismo
4. Audiodescrição	Revisa o texto falado gerado para cada prato	Pessoas cegas ou com baixa visão
5. Libras e tradução	Adiciona vídeo em Libras, traduções e versão em linguagem simples	Pessoas surdas, estrangeiras e com dificuldade de leitura
6. Braille	Gera o cardápio em braille e o arquivo para impressão	Pessoas cegas que leem braille
7. Publicação e QR Code	Informa o endereço do cardápio e gera o QR Code	Todos os clientes
Ao lado da área de trabalho, uma prévia mostra em tempo real como o cliente verá o cardápio.
Recursos
Cadastro dos pratos
<img src="img/cadastro.png" alt="Tela de cadastro dos pratos" width="700">
Alérgenos com pictogramas
São 13 pictogramas: os oito grupos da RDC nº 26/2015 da Anvisa (glúten, crustáceos, ovos, peixes, amendoim, soja, leite e castanhas) e mais cinco (moluscos, gergelim, mostarda, aipo e sulfitos). "Contém" usa borda sólida e "pode conter" usa borda tracejada, então a informação não depende só de cor. Todo ícone vem acompanhado do nome escrito.
<img src="img/pictogramas.png" alt="Os 13 pictogramas de alérgenos" width="700">
<img src="img/alergenos.png" alt="Tela de seleção de alérgenos" width="700">
> A RDC nº 26/2015 vale para alimentos embalados e exclui os alimentos preparados e vendidos em serviço de alimentação. Em restaurantes, informar os alérgenos é uma boa prática, e não uma obrigação dessa norma. Não existe um conjunto oficial único de ícones universais para alérgenos; estes pictogramas foram desenhados pelo projeto.
Alto contraste e tamanho de letra
<img src="img/contraste.png" alt="Tela de alto contraste" width="700">
Cardápio em braille
O aplicativo converte o texto do cardápio para braille de grau 1, seguindo a Grafia Braille para a Língua Portuguesa: sinal de maiúscula, sinal de número, pontuação e letras acentuadas. O cardápio sai em linhas de 32 ou 40 células, em folhas de 25 linhas, e pode ser baixado em braille Unicode ou em ASCII, para uso em impressoras braille. A conversão é automática, por isso o resultado deve ser revisado por uma pessoa que lê braille antes de imprimir.
<img src="img/braille.png" alt="Tela do cardápio em braille" width="700">
Identidade visual
<img src="img/logo.png" alt="Logo do Mesa Aberta" width="420">
O nome expressa a ideia de que todas as pessoas têm lugar à mesa. O símbolo é um prato visto de cima com o contorno aberto à direita. Dentro dele há uma cela braille com os pontos da letra M, e um ponto âmbar na abertura representa o lugar livre. As cores são azul-marinho e âmbar, de alto contraste entre si, e a fonte é a Atkinson Hyperlegible, desenhada para facilitar a leitura por pessoas com baixa visão. Slogan: Cardápios para todos.
Tecnologia
Aplicativo em um único arquivo (`index.html`), com HTML, CSS e JavaScript puros, sem servidor.
Os dados ficam no navegador de quem usa (`localStorage`); nada é enviado para a internet.
Hospedado no GitHub Pages.
Limitações e próximos passos
O protótipo ainda não publica cada cardápio como uma página própria na internet.
Testar o aplicativo com pessoas cegas, com baixa visão e surdas.
Submeter a conversão em braille à revisão de uma instituição especializada.
Validar a lista de alérgenos e os pictogramas com nutricionistas e com pessoas que têm alergia alimentar.
Permitir o envio de vídeos em Libras (hoje feito por link).
Contexto
Projeto acadêmico desenvolvido na UNESP, Campus de São José dos Campos, curso de Engenharia Ambiental. A acessibilidade é um direito assegurado pela Lei Brasileira de Inclusão da Pessoa com Deficiência (Lei nº 13.146/2015).
