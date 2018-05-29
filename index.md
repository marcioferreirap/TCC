# Procedimentos iniciais

Os procedimentos abaixo tem por objetivo instruir aos usuários como preparar o ambiente para instalação das ferramentas.

## Instalação do Java develpment kit 8

Para que haja uma instalação correta de todos os aplicativos é necessário fazer o download do JDK 8 (Java development kit) em sua última versão que está disponível [clicando aqui](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html). Como é possível verificar na figura, a seguir.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig01.png)

Após o download realizado basta abrir o arquivo e seguirá a instalação. 

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig02.png)

Os passos para instalação, são assistentes simples, que indicam apenas para avançar até concluir, como é observado na figura a seguir.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig03.png)

É necessário aguardar o assistente de instalação para que a instalação seja iniciada.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig04.png)

Após aguardar a tela de instalação ser inicializada, é necessário que se aguarde a tela instalação.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig05.png)

Quando finaliza a instalação é exibida a tela informando ao usuário que a instalação foi realizada com sucesso.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig06.png)

Com isso é necessário que o usuário vá até as propriedades de “Meu computador”, depois em “Configurações Avançadas do Sistema”, em seguida “Variáveis de Ambiente” e insira uma nova “Variável de sistema”.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig07.png)

Em seguida após adicionar é só verificar se foi inserida. Para verificar se tudo foi corretamente instalado, basta abrir o “Prompt de Comando” e digitar “java -version” e verificar se é exibido a versão do java.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-java/fig08.png)


## Instalação do Pentaho Suite

Após a instalação do JDK, deve-se acessar o site da SourceForge, no qual os arquivos de instalação estão armazenados e disponíveis para download que são obtidos a partir do link: https://sourceforge.net/projects/pentaho/files/. Na figura é possível observar várias pastas, que devem ser escolhidas uma por vez. Deve-se iniciar pela pasta principal: Data Integration (PDI – Pentaho Data Integration). 

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig01.png)

Após entrar na pasta “Data Integration”, é necessário selecionar qual versão será instalada. Esse é um momento importante, pois todas as demais ferramentas devem ser da mesma versão ou compatível com a versão do servidor instalado. Como podemos observar na figura abaixo existem diversas versões do Pentaho, com diferentes funcionalidades. Pelo fato da pesquisa ter iniciado em 2016, a escolha da versão ficou na mais atual que era ainda a versão 6.1. 

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig02.png)

Após a escolha da versão deve-se fazer o download do arquivo pdi-ce-6.1.0.1-196.zip, como se observa na figura, e este arquivo deve ficar descompactado em uma pasta, onde ficarão todos os demais pacotes da suíte do Pentaho.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig03.png)

Após o download e descompactação do arquivo, ele já fica pronto para fazer as transformações porém, por se tratar de uma suíte de aplicativos, deve-se realizar o download das demais ferramentas para realizar o processo de forma completa.
Dando seguimento às ferramentas, temos o Business Intelligence Server que é o painel de acesso aos resultados realizados no ETL e também manipulação dos relatórios.
É necessário voltar para a estrutura apresentada na primeira figura, e escolher a pasta “Business Intelligence Server”. Logo após essa escolha observará que a estrutura ficou semelhante à figura 17, então deve-se escolher a pasta “6.1”, uma vez que a versão foi selecionada.
Com isso deve ser fazer o download do arquivo “biserver-ce-6.1.0.1-196.zip” conforme observamos abaixo.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig04.png)

Prosseguindo com as instalações, deve-se instalar a ferramenta para criação dos cubos de análise, o Pentaho Workbench (Mondrian). Ele está disponível em um outro link diferente das demais ferramentas já apresentadas.
Por isso se faz necessário que navegue até o link: https://sourceforge.net/projects/mondrian/files/.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig05.png)

Em seguida é necessário escolher a versão. Nessa pesquisa foi escolhida a versão 3.12.0, pois está é a versão compatível com as versões das outras ferramentas já instaladas, que pode ser observado através da figura anterior, com a release final 196.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig06.png)

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig07.png)

Após realizar o download das ferramentas é possível verificar essa mesma estrutura de pastas. Existem outras ferramentas para a suíte que podem ser observadas na referida figura, porém estas não foram usadas para este trabalho de pesquisa foram realizados os downloads apenas para caso haja evolução a suíte fique disponível para o uso. 

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig08.png)

Após o download de todas as ferramentas, elas já podem já podem ser iniciadas e prontas para o uso. Ao abrir a pasta “biserver-ce”, é possível verificar vários arquivos; dentre eles o arquivo "start-pentaho”, que pode ser com extensão “.sh” para usuários Linux, ou “.bat” para usuários Windows. Neste caso, foi escolhido “start-pentaho.bat”, e é necessário que se aguarde um tempo para que haja o carregamento de todos os componentes do usuário.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig09.png)

Caso não haja nenhuma alteração das configurações padrão, após a inicialização do servidor é possível abrir no browser do computador o servidor local usando o seguinte endereço: “localhost:8080/pentaho/Login” e um tela igual à figura 99 aparecerá solicitando o login e senha. Por padrão o login e senha são, respectivamente, “admin” e “password”.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig10.png)

Após realizar o login na ferramenta, o usuário está apto a manusear os dados, e realizar as criações de relatórios, bem como verificar os cubos criados e a partir daí realizar as análises dos dados obtidos.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig11.png)

De forma semelhante a que o BI Server foi executado, temos o PDI que possui um arquivo com extensão “.bat” chamado Spoon. Para que a ferramenta seja inicializada é necessário abrir esse arquivo.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig12.png)

Após a abertura do arquivo deve-se aguardar o carregamento da ferramenta. Quando ela é carregada apresenta a tela semelhante à figura a seguir. Na figura observamos a versão instalada, que pode ser obtida acessando o menu “Ajuda> Sobre”.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig13.png)

Não existe sequência para abertura, mas indica-se abrir uma ferramenta por vez, ou dependendo da necessidade do momento e das configurações disponíveis. Finalmente, a seguir, executaremos o Pentaho Schema Workbench. De forma semelhante às demais ferramentas, como esta é uma versão Windows, será executado o arquivo “workbench.bat” para que seja executada a ferramenta.

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig14.png)

Após ser aberta a ferramenta, fica disponível para criação dos cubos analíticos sendo necessário fazer a publicação destes cubos para que estes fiquem disponíveis no “bi server”, conforme a tela a seguir. 

![image](https://raw.githubusercontent.com/marcioferreirap/TCC/master/figuras/instalacao-pentaho-suite/fig15.png)

Nesta pesquisa foram realizadas provas de conceito com a suíte na intenção de prototipar a aplicação final. Com os testes finalizados foi verificado que a ferramenta iria atender aos requisitos necessários e os e deu-se continuidade aos passos seguintes.



## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/marcioferreirap/TCC/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/marcioferreirap/TCC/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
