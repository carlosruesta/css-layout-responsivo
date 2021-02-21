# css-layout-responsivo

# projeto-apeperia
Arquivos do projeto para a Apeperia

### Tamanhos Responsivos

* **REM** é uma unidade relativa à propriedade font-size da tag <html>, portanto se a tag <html> tem 16px de font-size 1 REM é equivalente à 16px. 
* **EM** é relativa à propriedade font-size da tag mãe, portanto se a tag mãe tiver um font-size de 16px 1 EM é equivalente à 16px.

* **REM** vem de “Root ephemeral” que em uma tradução técnica fica “variável à raiz”, ou seja, é variável em relação à propriedade font-size da tag raiz (HTML). 
* **EM** vem de “ephemeral” que significa “variável”, e ela é variável à propriedade font-size da tag mãe.

### Uso de SVG

* Quando vamos trabalhar com imagens, o formato SVG apresenta uma grande vantagem por ser leve e não perder qualidade quando ampliado por ser
 gerado por uma instrução de computador.
* É recomendado usar imagens do tipo SVG em imagens simplificadas, ícones e logotipos. SVG não consegue manter detalhes de uma imagem complexa.

### Mobile First - Desktop First

* Na hora de seguir um conceito de desenvolvimento, seja mobile-first ou desktop-first, não existe certo ou errado. 
* Cada um deles tem suas vantagens e desvantagens, e elas devem ser avaliadas de acordo com as necessidades do projeto.

* Algumas motivações para usar mobile-first:
   + Grande parte dos acessos e vendas vem de dispositivos mobile
   + O design é minimalista e simplificado
   + Foco em conteúdo
* Algumas motivações para usar desktop-first:
   + A interface pode ter diversas features mais ricas
   + Maior capacidade de banda e processamento
   + O produto é otimizado para desktop (ex: Google Docs)

* Então na hora de desenvolver é importante analisar todos os pontos que vão influenciar no projeto:
   + clientes, 
   + features, 
   + custo
   + linguagem visual
* São alguns dos pontos que vão favorecer uma abordagem sobre a outra.

### Meta Viewport
+ O meta “viewport” é o que habilita o navegador a visualizar a página como se fosse um dispositivo móvel.
+ “meta name=“viewport” content=”largura da tela vai ser igual a largura do dispositivo”
+ Como o browser não tem como saber o tamanho da tela do dispositivo em polegadas, ele usa a resolução do dispositivo como um parâmetro. 
+ O “viewport” faz uma conversão desse tamanho em pixels para um tamanho que seja plausível, um tamanho que seja mais amigável para um celular daquele tamanho. 
+ “initial-scale” no “1.0” para garantir que a escala da página sempre vai ficar proporcional ao tamanho da tela do dispositivo
+ “initial-scale” menor que “1.0” geram um zoom maior na renderização do site

### Uso variaveis e Tag root
* Para declaração de variáveis de ambiente. No caso, de cores, foi adicionada a tag root no CSS base.
* A tag "root" ela representa a tag HTML só que com especifidade e peso maior.
* Ao usar a tag root não corremos o risco de ser sobreescrita. As variáveis declaradas terão escopo "global". 
* Declaramos dentro de algum seletor (que costuma ser o :root {}) escrevendo --nome-da-variavel: valor
   + Chamamos as variáveis seguindo uma sintaxe, usamos uma função var e passando o nome da variável dentro dessa função.
   
### Uso do emmet

section.destaque.container>h2.destaques__titulo+(a*2>figure.destaque__painel>img.destaque_painel-imagem+figcaption.destaque__painel-texto)+a.destaques__botao.botao

### Uso de unidades viewport e max-width com medidas fixas

Unidades de viewport são unidades relativas, como por exemplo, porcentagem.
100vh -> 100% da altura da tela do dispositivo
100vw -> 100 % da largura da tela do dispositivo

