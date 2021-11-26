

# Curso de Visualización de Datos Urbanos Etopia 2021

Un repositorio con los contenidos del curso

1.  Introducción y organización del curso
2.  Herramientas
3.  Limpieza de datos
4.  Análisis de datos
5.  Visualización de datos
6.  Puesta en común de los proyectos y cierre del curso


# Sesiones


## Sesión 1. 22/10

1.  Presentación del curso, quiénes somos, etc.
2.  Presentación de las personas participantes
3.  Qué pretendemos con el taller
4.  Un par de ejemplos: Ciudad Desigual y Territorio de Datos
    1.  Ciudad Desigual: <https://jllopc.github.io/ciudad.desigual/>
    2.  Territorio de datos: <https://territoriodedatos.org>
5.  Debate entre historiadores y sociólogos, Ignacio Azcona
6.  La línea de comandos
    -   Cygwin y apt-cyg
    -   Brew
    -   WSL


## Sesión 2. 23/10

1.  Charla de experiencias artísticas con la ciudad, Julián Pérez (ver [PDF](file://src/pdf/slides-Julian.pdf))
2.  Configuración de la línea de comandos
3.  Creación de grupo de Telegram
4.  Creación de organización de Github
5.  Herramientas de línea de comandos


## Sesión 3. 29/10 Viernes


### Repaso


### Mario Pérez-Montoro

Presentación en [PDF](file://src/pdf/mpm-sesion-i.pdf)


### Github

-   Datos

    -   Organización: <https://github.com/org/mpvdes>
    -   Equipo: <https://github.com/org/mpvdes/etopia>
    -   Repositorio: <https://github.com/mpvdes/etopia-2021>

-   Ayuda

    -   Manual de Adolfo Antón Bravo: repositorio en github <https://github.com/flowsta/github> y web <http://flowsta.github.io/github/>
    -   Web oficial, <https://git-scm.com/>

-   Clonado y actualización del repositorio


## Sesión 4. 30/10, Sábado


### Mario Pérez-Montoro

-   enchroma
-   Tinta-dato y tinta-no-dato


### DONE Repasar Github


### DONE Repositorio Github propio


### Configuración nano


### Vídeo: aparcamientos en EE.UU.


### Vídeo: casas en EE.UU


## Sesión 5. 5/11


### Comunicación visual con tablas


### Google Spreadsheet

-   ImportURL

        IMPORTHTML("url"; "consulta"; índice)

-   ImportXML

        =IMPORTXML("url";"xpath")
    
    Otras opciones:
    
    -   `count(//div[@class`'']//a/@href)=
    -   `//img/@alt`
    -   `//a[contains('Escuela')]/@href`

-   ImportFeed

        =importfeed("url";"items url";VERDADERO;250)
    
    url: <http://www.ft.com/rss/home/europe>
    
        =importfeed(B2;"items url";VERDADERO;250)


### Open Refine

-   <https://openrefine.org/>

-   "A free, open source, powerful tool for working with messy data"
-   La navaja suiza de la limpieza de datos.
-   En la versión 3.4.1, en la versión para Windows, está la opción de descargarlo con [OpenJDK](https://adoptopenjdk.net/about.html) incluido.


### Python

-   csvkit

    Instalación:
    
        pip install csvkit

-   Scikit learn

    <https://scikit-learn.org/stable/>

-   Jupyter

    Instalamos:
    
        pip install jupyter
    
    Lanzamos:
    
        jupyter notebook


# Ejemplos

-   Ciudad Desigual: <https://jllopc.github.io/ciudad.desigual/>
-   Territorio de datos: <https://territoriodedatos.org>
-   Why American public transit is so bad, <https://www.vox.com/videos/21529609/usa-public-transit-trains-buses-cars>
-   NPR, Housing Segregation,  Let's Talk: Video housing segregation in everything, <https://www.npr.org/sections/codeswitch/2018/04/11/601494521/video-housing-segregation-in-everything>
-   Serie NPR: <https://www.npr.org/series/718730324/video>
-   Implant Files: <https://medicaldevices.icij.org/>
-   Offshore Leaks, <https://offshoreleaks.icij.org/>
-   Wikileaks, <https://wikileaks.org/>
-   NICAR, <https://www.ire.org/nicar/>
-   TRESCA, <https://trescaproject.eu>, Trustworthy, Reliable and Engaging Scientific Communication Approaches


## R

R es un lenguaje de programación libre de análisis estadístico. Es decir, es similar a trabajar con:

-   Excel, si lo utilizas con esa finalidad.
-   SPSS, de IBM.
-   Stata
-   otros...


### Trabajar con R

Hay varias opciones para trabajar con R:

-   La propia consola de R que lanzamos desde la terminal.
-   El programa GUI que abre la consola de R.
-   El programa RStudio.


### Instalación de la consola

De momento vamos a instalar la consola para las próximas sesiones:

-   En Cygwin, `apt-cyg install R`
-   En OSX, `brew install r` si no quieres la versión gráfica o `brew cask install r` si quieres la GUI de R.
-   En Debian/Ubuntu GNU/Linux, `sudo apt install r-base`


### Enlaces

-   [Why data journalists should start using R in 2016](https://timogrossenbacher.ch/2015/12/why-data-journalists-should-start-using-r-in-2016/).
-   [How Do I?...(do that in R)](https://smach.github.io/R4JournalismBook/HowDoI.html)
-   <http://rstudio-pubs-static.s3.amazonaws.com/6975_c4943349b6174f448104a5513fed59a9.html>
-   <https://www.r-bloggers.com/cross-tabulation-with-xtabs-exercises/>


### BBPlot

R package that helps create and export ggplot2 charts in the style used by the BBC News data team


### Katie Jolly

Es el caso de [Katie Jolly](https://www.katiejolly.io/) tal como explica en su artículo [Data Driven Design](https://www.katiejolly.io/blog/2019-04-25/data-driven-design): Data-driven design in 'Curious City: In, Out, Above, Beyond Saint Paul', donde expone su interés por el llamado "information design" o diseño de información y cómo utiliza R y software de diseño gráfico para crear una visualización llamada "Turning the Page" para el libro "Curious City: In, Out, Above, Beyond Saint Paul".

![img](https://www.katiejolly.io/blog//assets/curious-city/kjolly_final.png "Trabajo final K. Jolly")

El interés le vino siguiendo el trabajo de [James Chesire](https://spatial.ly/) que suponía que, dado que era un usuario de [R](https://cran.r-project.org/) y de [ggplot2](https://ggplot2.tidyverse.org/), igual usaba software libre.

![img](https://www.katiejolly.io/blog//assets/curious-city/treasures_before_after.jpg)

De hecho el ejemplo anterior está sacado del artículo [The coder and the designer](http://theinformationcapital.com/coder-designer/) donde cuenta su experiencia con R y cómo se apoya en sus visualizaciones para el arte final.


### BBC R and Data Journalism Cookbook for R Graphics

At the BBC data team, we have developed an R package and an R cookbook to make the process of creating publication-ready graphics in our in-house style using R’s ggplot2 library a more reproducible process, as well as making it easier for people new to R to create graphics.


# Datos


## Recursos libres

-   Freesound: <https://freesound.org/search/?q=zaragoza>
-   Wikimedia:  <https://commons.wikimedia.org/w/index.php?search=zaragoza&title=Special:MediaSearch&go=Go&type=image>
-   Archive: <https://archive.org/search.php?query=zaragoza>
-   Gutenberg Project: <https://www.gutenberg.org/ebooks/search/?query=zaragoza&submit_search=Go%21>


## Zaragoza

-   Datos abiertos Zaragoza: <https://www.zaragoza.es/sede/portal/datos-abiertos/>
-   El bosque de los zaragozanos: <https://www.zaragoza.es/sede/portal/medioambiente/elbosquedeloszaragozanos/area-descargas>
-   Contratación pública: <https://www.zaragoza.es/sede/servicio/contratacion-publica/>
-   Información polínica, <https://www.zaragoza.es/sede/portal/medioambiente/calidad-aire/polen/servicio/informacion-polen/>
-   Calidad del aire: <https://www.zaragoza.es/sede/portal/medioambiente/calidad-aire/>
-   


## Datos de prueba

-   [Dataset for visualisation construction](https://visdatasets.github.io/)
-   [The Guardian Polls](https://docs.google.com/spreadsheets/d/1oHcxlAbkTJmqfOxYQM22cvjjjRf5pETIF30x7L-qybc/edit#gid=0)


## España

-   [Base de datos de comercio exterior](http://aduanas.camaras.org/)
-   [CNMV](http://www.cnmv.es/portal/home.aspx)
-   Ejército, <http://www.ejercito.mde.es/unidades/Madrid/index.html>
-   INE, <http://www.ine.es/prensa/epa_tabla.htm>
-   datos.gob.es, <https://datos.gob.es>
-   IGN, <https://datos.ign.es/>


## Contaminación

-   Red Nacional de estaciones de medición: <https://sig.mapama.gob.es/calidad-aire/>
-   Datos oficiales Calidad del Aire 2018: <https://www.miteco.gob.es/es/calidad-y-evaluacion-ambiental/temas/atmosfera-y-calidad-del-aire/calidad-del-aire/evaluacion-datos/datos/Datos_oficiales_2018.aspx>
-   La mortalidad por cáncer en ciudades situadas en las proximidades de incineradoras e instalaciones para la recuperación o eliminación de residuos peligrosos: <https://www.sciencedirect.com/science/article/abs/pii/S0013935116311197?via%3Dihub>
-   Asociación entre Incineradoras de Residuos Municipales y Cáncer de mama invasivo: <http://www.casmadrid.org/index.php/documentos/1163-asociacion-entre-incineradoras-de-residuos-municipales-y-cancer-de-mama-invasivo>
-   Datos diarios Madrid 2001 - 2020: <https://datos.madrid.es/sites/v/index.jsp?vgnextoid=aecb88a7e2b73410VgnVCM2000000c205a0aRCRD&vgnextchannel=374512b9ace9f310VgnVCM100000171f5a0aRCRD>


## COVID19

-   <https://github.com/CSSEGISandData/COVID-19/>


# Software


## Cygwin


### apt-cyg

El gestor de paquetes de Cygwin, sigue las [instrucciones](https://github.com/transcode-open/apt-cyg) oficiales o consulta mi [manual](https://flowsta.github.io/bases-periodismo-datos/#org47541ce).


## brew

[Brew](https://flowsta.github.io/bases-periodismo-datos/#orgf689bc4) es el gestor de paquetes para el emulador de Terminal de Mac.


## WSL


## nano


### nanorc


## Editor de textos

Se recomienda nano pero si queréis otra opción [aquí tenéis](https://blog.infotics.es/2015/11/11/editor-de-textos/) una lista con algunos de los más usados


## Navegador gráfico

-   [Firefox](https://www.mozilla.org/en-US/firefox/new/)
-   [Chromium](https://www.chromium.org/Home) o [Chrome](https://www.google.com/chrome)
-   [Opera](https://www.opera.com/es)


## Git

-   [Página oficial](https://git-scm.com)
-   [Github](https://github.com)
-   [Gitlab](https://gitlab.com)
-   [Manual de Adolfo Antón Bravo](https://flowsta.github.io/github)


## Python


### Instalación

Podemos instalarlo de [python.org](https://www.python.org/downloads/) o bien desde la terminal. Instalamos la versión 3 porque la rama 2 ya está con fecha de caducidad.

-   Windows Cygwin

        apt-cyg install python3

-   OSX Brew

        brew install python3

-   GNU/Linux (incluido WSL)

        sudo apt install python3


### Arrancamos python

Una vez que lo tenemos instalado, si es desde la terminal, se lanza con `python` y veremos que el /prompt/ cambia y se pone con tres caracteres de "mayor que" `>>>`.

Para poder utilizar librerías lo mejor es instalar \*pip\* que es un gestor de librerías/paquetes en python.

¡Buenas noticias! Desde la versión de python 3.4 viene con pip preinstalado! (también en la rama 2.7 desde la versión 2.7.9)


### Comprobar versión

Lo podemos hacer con:

    python --version

Si tuvieras python2 y python3 instalado, aquí te podría salir la versión 2.7 y entonces tendrías que repetir el comando con `python3 --version` y acordarte de siempre llamar a python3.
Este mensaje también te vale para `pip`


### pip

Se puede comprobar que está instalado preguntando qué versión tiene:

    pip --version

Para cualquier duda se puede ir a la ayuda <https://pip.pypa.io/en/stable/installation/>


### Jupyter


### [Matplotlib](https://matplotlib.org/)


### [Bokeh](https://demo.bokeh.org/)


### csvkit

Instalación:

    pip install csvkit


## R

Descargarse [R](https://www.r-project.org/) es fácil pero si os parece complicado podéis bajaros también [R-Studio](https://rstudio.com/).


### RStudio


### Tidyverse


### BBPlot

R package that helps create and export ggplot2 charts in the style used by the BBC News data team


### BBC R and Data Journalism Cookbook for R Graphics

At the BBC data team, we have developed an R package and an R cookbook to make the process of creating publication-ready graphics in our in-house style using R’s ggplot2 library a more reproducible process, as well as making it easier for people new to R to create graphics.


## Tabula


## OpenRefine

-   URL, <https://openrefine.org>
-   Manual de Adolfo Antón Bravo, <https://github.com/flowsta/refine>


## Tesseract


## Sistemas operativos

-   Debian GNU/Linux: <https://debian.org>
-   Ubuntu GNU/Linux: <https://ubuntu.org>
-   Tails: <https://tails.boum.org/>


## VPN

<https://riseup.net/en/vpn>


## convert

    convert *.jpeg archivo.pdf


## Web


### Plantillas HTML

-   Plantillas HTML5 en <https://html5up.net/>
-   Bootstrap: <https://getbootstrap.com/>


### SSG

/Static Site Generator/ o sistemas de generación de contenido
estático:

-   Jekyll, <https://jekyllrb.com/>
-   Hugo, <https://gohugo.io/>
-   

