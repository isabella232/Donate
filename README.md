# Introdução

Esta é uma aplicação de referencia para solicitar doações que ajudem em seus projetos.
As doações são mandadas para terceiros e não para o dono da aplicação e os pagamentos são
recebidos através da API Adaptive Payments. Em particular, estamos usando o Parallel Payments
para dividir as doações entre várias instituições de caridade definidas pela aplicação.

# Pre requisitos

* Google App Engine SDK for Python instalado. Baixe através do link:
  http://code.google.com/appengine/downloads.html

* Experiência prática com o Google App Engine e projetos utilizando Django.
  Nós NÃO estamos usando uma app engine com Django Framework, mas estamos usando
  grandes projetos que modificaram a ultima versão Django para ser usado com essa
  app engine. Para mais informações sobre esses grandes projetos, seguem os links:
    http://code.google.com/appengine/docs/python/gettingstarted/
    http://www.djangoproject.com/
    http://www.allbuttonspressed.com/projects/django-nonrel

* Possuir um brower moderno (Safari, Chrome, Firefox) pois a parte client-side é
  implementada usando Protovis - um poderoso framework para visualizações web baseado
  em JavaScript e SVG: http://vis.stanford.edu/protovis/

# Estrutura do Projeto

Abaixo uma breve descrição individual dos componentes do GAE.

* app.yaml - Arquivo de configuração da app engine. A principal coisa que deve ser
  modificada neste arquivo é o parametro que define o nome do seu aplicativo na 
  app engine. Veja http://appengine.google.com para criar uma aplicação.

* urls.py - Todo o mapeamento das URLs finals que o código tem permissão de manipular.

* donate - Diretório que contém toda a lógica de visão e definições de modelo do projeto.

* templates - Diretorio que contem todos os arquivos de template do projeto.

* static - Diretorio que contém todos os arquivos estátidos do projeto.(images, .css, etc)

* settings.py - O modulo de configurações dos projetos Django. Ele também contem as
  propriedades específicas do projeto PayPal e definições de Entidades de Caridade.
  Você terá de modificar várias propriedades neste arquivo para usar sua própria conta
  PayPal. Preste bastante atenção também na lista "CHARITIES", que é onde você irá definir
  as entidades de caridade que receberão as doações da sua aplicação.

# Screenshot

![screenshot!](https://github.com/zaffra/Donate/raw/master/screenshot.png)

Provided by: Zaffra, LLC - http://zaffra.com
Traduzido por: Alê Borba
