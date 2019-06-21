<img src="../../src/images/benner_rgb.png" align="right"/>

# Customização do Portal De Serviços

1.  **[Introdução](#introdução)**
2.  **[Customização - Geral](#customização-geral)**
3.  **[Customização - Login](#customização-login)**
4.  **[Customização - Princiapl](#customização-principal)**
5.  **[Customização - Rede de Atendimento](#customização-rede-de-atendimento)**
6.  **[Customização - Favicon](#customização-favicon)**
7.  **[Lembretes](#lembretes)**

## Introdução

Neste manual será abordado de forma simples como alterar os temas pré-definidos do Portal(WES), plano de fundo da página de login e seu logo, logo da página principal, o ícone que está localizado na aba do navegador e um exemplo de como aplicar scripts na página de login.

> Nota: É importante que para a realização da customização o conceito de camadas do WES esteja claro (Camadas 20 e 50), pois será necessário alterar artefatos da camada Benner (20) para a camada Cliente (50). Caso contrário as alterações realizadas não serão utilizadas uma vez que a camada ativa será a maior.

## Customização Geral

Inicialmente é necessário acessar o Portal de Serviços com usuário que possua papel “Desenvolvedor”, ativa o modo desenvolver, alterar o papel e então ativar a customização dos itens que serão alterados:

> Ativar Desenvolvimento
![001](src/images/001.png)

> Desenvolvedor > Configuações 
![002](src/images/002.png)

> Desenvolvedor > Configuações > Customização
![003](src/images/003.png)

>Desenvolvedor > Configuações > Customização > Ativar a customização dos itens que serão alterados
![004](src/images/004.png)

Ao selecionar para customizar a página de login exibirá janela para selecionar qual é a forma de login desejada: da camada anterior (no formato padrão do Portal), ao lado direito, no centro com outro padrão, e no centro sem imagem de fundo.
Escolha a opção que desejar e então clique no botão “Salvar e Reiniciar” para aplicar as alterações.

>Selecionar a forma de login
![005](src/images/005.png)

>Salvar e reiniciar
![006](src/images/006.png)

Feito isso será criado os arquivos necessários na camada do Cliente (50) dentro da pasta de instalação da aplicação do Portal, é Através destes arquivos que serão realizadas as alterações de tema, imagem, logo, etc.

## Customização Login
O arquivo Login50.aspx deve ter sido criado e é através dele que é aplicado o tema na página de login. É necessário alterar a tag “Theme”.

>Alterar tag theme
![007](src/images/007.png)

É possível utilizar os temas padrões do WES existentes na pasta “App_Themes” ou criar um tema próprio (copiando e colando um tema base existente):

>Temas padrões
![008](src/images/008.png)

>Tema customizado
![009](src/images/009.png)

Após o tema criado, é necessário alterar no Login50.aspx o tema.

>Tema alterado
![010](src/images/010.png)

Dentro da pasta do tema recém-criado existirá um CSS onde é possível realizar as alterações para o estilo da página de login, inclusive o logo e a imagem de fundo.

>CSS Custom
![011](src/images/011.png)

>Alterar logo da tela login
![012](src/images/012.png)

>Logo alterado da tela de login
![013](src/images/013.png)

>Alterar imagem de fundo da tela de login
![014](src/images/014.png)

>Imagem de fundo alterada da tela de login
![015](src/images/015.png)

>Alterar Bordas e cor do botão da tela de login
![016](src/images/016.png)

>Bordas e cor do botão alterados da tela de login
![017](src/images/017.png)

Na página Login50.aspx é possível alterar a cor do botão da rede de atendimento e também aplicar scripts para ajustar o login como desejar.

>Alterar botão rede de atendimento da tela de login
![018](src/images/018.png)

>Botão rede de atendimento alterado da tela de login
![019](src/images/019.png)

>Aplicar script para ajustar tela de login
![020](src/images/020.png)

>Script aplicado na tela de login
![021](src/images/021.png)

Também é necessário ajustar a customização da página de novo usuário, para isso é necessário copiar o arquivo “default.css” do caminho ~Content/css/Portal/Public/NovoUsuario para ~Content/css/public e renomea-lo para “custom.css”.

>Tela de cadastro de novo usuário.
![022](src/images/022.png)

>Arquivo default.css
![023](src/images/023.png)

>Arquivo default.css renomeado para custom.css
![024](src/images/024.png)

Neste novo arquivo custom.css é possível alterar o logo, imagem de fundo e as cores.

>Alterar Logo tela cadastro de usuário
![025](src/images/025.png)

>Logo alterado da tela de cadastro de usuário
![025](src/images/026.png)

>Alterar imagem de fundo da tela de cadastro de usuário
![027](src/images/027.png)

>Imagem de fundo alterada da tela de cadastro de usuário
![028](src/images/028.png)

>Alterar cores da tela de cadastro de usuário
![029](src/images/029.png)

>Cores alteradas na tela de cadastro de usuário
![030](src/images/030.png)

## Customização Principal

É necessário alterar a tag “Theme” do web.config para alterar o tema da página principal do Portal, pode-se escolher entre os temas padrões do Portal.

>Arquivo Wheb.config
![031](src/images/031.png)

>Temas disponiveis no portal
![032](src/images/032.png)

>Benner - padrão portal
![033](src/images/033.png)

>Blue
![034](src/images/034.png)

>Dark blue
![035](src/images/035.png)

>Default
![036](src/images/036.png)

>Grey
![037](src/images/037.png)

>Light
![038](src/images/038.png)

>Light2
![039](src/images/039.png)

Para alterar a logo da página principal é necessário ir na pasta do tema escolhido e criar um arquivo cópia do custom.css na camada 50 e nele alterar a imagem da logo.

>Cópia do arquivo custom.css
![040](src/images/040.png)

>Alterar logo da página principal
![041](src/images/041.png)

>Logo da página principal alterado
![042](src/images/042.png)

É importante também alterar a logo do tema de alto-contraste, para isto repita os passos feito no tema escolhido e no arquivo “Default50.master” na raiz do Portal altere o css que é utilizado para o alto-contraste.

>Tela principal em alto-contraste
![043](src/images/043.png)

>Cópia custom.css no tema de alto-contraste
![044](src/images/044.png)

>Alterar logo da página principal no tema de alto-contraste
![045](src/images/045.png)

>Arquivo Default50.master
![046](src/images/046.png)

>Alterar o arquivo Default50.master
![047](src/images/047.png)

>Logo da página principal no tema de alto-contraste alterado
![048](src/images/048.png)

## Customização Rede de Atendimento

A página da Rede de Atendimento utiliza um layout diferente, por isso também é necessário ajustá-la.
Para customizar a rede de atendimento é necessário criar um css cópia do “index.css” e renomear o arquivo para “custom.css” e a partir deste ajustar o css como desejado.

>Cópia custom.css na tela da rede de atendimento
![049](src/images/049.png)

>Alterar logo na tela da rede de atendimento
![050](src/images/050.png)

>Logo da tela rede de atendimento alterado
![051](src/images/051.png)

>Alterar cor de fundo do topo da tela da rede de atendimento
![052](src/images/052.png)

>Cor de fundo alterada da tela de rede de atendimento 
![053](src/images/053.png)

## Customização Favicon

Para alterar o ícone que é exibido no navegador é necessário substituir o arquivo “favicon50.ico” na pasta raíz da aplicação do Portal, é de extrema importância que o arquivo seja no formato ICO.

>Arquivo favicon50.ico antes de alterar o ícone
![054](src/images/054.png)

>Icone no navegador antes de alterar o ícone
![055](src/images/055.png)

>Arquivo favicon50.ico depois de alterar o ícone
![056](src/images/056.png)

>Icone no navegador depois de alterar o ícone
![057](src/images/057.png)

## Lembretes

>Lembrando que é possível alterar os artefatos de camada Cliente (50) como desejar, ou seja, é possível customizar a página de login e os estilos dos temas da forma que mais agrada ao cliente.

>Após finalizar as customizações desejadas é necessário desativar o modo desenvolvedor do Portal de Serviços.
