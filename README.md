# Plantilla para elaborar trabajo de graduación - [ECFM](https://ecfm.usac.edu.gt/)

Este repositorio contiene los ficheros para escribir el trabajo de graduación para las carreras de matemáticas o física.

La plantilla inicial se realizó con Texlive 2015, TeXstudio, sobre el sistema Operativo GNU/Linux Debian 8.2. Las actualizaciones más recientes se hicieron con Ubuntu 20.04 (TeXstudio y TeXlive 2019) y MacOS Monterey (TeXstudio y TeXlive 2021), el autor nunca la ha corrido con Windows pero supone que no debe haber problema.

## Descripción del contenido

- `thesisECFM.cls` fichero modificado a partir de `book.cls`.
- `macros.sty` fichero que hace llamada a los paquetes: babel, ifthen, textcase, inputenc fontenc, amsfonts, amsmath, amssymb, amsthm, mathrsfs, geometry, setspace, caption, color, longtable, pdfpages, graphicx, hyperref, url, breakurl. La mayoría de estos paquetes ya están preconfigurados con las especificaciones para el trabajo de graduación, **NO SE DEBEN CAMBIAR**, si necesita otros paquetes los debe llamar desde `TesisTotal.tex` o `TesisTotalBibTex.tex` y hacer las configuraciones respectivas.
- `escudo.pdf` fichero que contiene el escudo de la USAC.
- `TesisTotal.tex` fichero principal en donde se declaran macros y la inclusión de restantes ficheros _*.tex_, lo utiliza si no usará **BibTeX** para gestinar la bibliografía y citas.
- `bbtesis.tex` fichero que contiene la bibliografía, dentro de él están las normas para el formato de cada tipo de referencia, para usar con _TesisTotal.tex_.
- `TesisTotalBibTeX.tex` fichero que un inicio se incluyó para implementar las **normas APA** y **BibTeX** para gestinar la bibliografía y citas. Ahora se cambió para utilizar **flexbib.sty** y los complementos **flexbib.bst** y **spanishbst.tex**, éstos últimos ficheros fueron descargados de [VJornadas](https://github.com/JornadasR/VJornadas), con lo cual se tiene mejor control del estilo bibliográfico en español. Para una guía de uso de _flexbib_ consultar [CervanTeX](http://www.cervantex.es/files/cervantex/texemplares6.pdf).
- `ordenImpresion.pdf` este fichero debe sustituirse por copia digital de la carta emitida por el Director de la escuela, donde autoriza la impresión del trabajo de graduación.
- `bbtesis.bib` fichero que contiene la bibliografía para gestión con _BibTeX_, en `bibtesis.txt` hay una descritpción del tipo de referencia.
- `tch1.tex` fichero con un ejemplo de un capítulo del trabajo de graduación, ejemplos ecuaciones, grupos de ecuaciones, tablas, tablas largas (longtables), imágenes, y de la identificación de éstas (recordar dar la fuente de cada una, si es propia obviarlo). Con los pies de página dentro de tablas, considerar el comando **\footnotetex**.
- `tch2.tex` fichero con una tabla con los comandos para citas válidos con **flexbib**, éste solamente está incluido en `TesisTotalBibTeX.tex`.
- `agradecimientos.tex`, `dedicatoria.tex`, `introduccion.tex`, `objetivos.tex`, `simbolos.tex`, `c_y_r.tex` ficheros para incluir contendio adicional: agradacemientos que el autor quiera incluir, dedicatoria del trabajo de graduación que el autor quiera hacer, introducción, objetivo general y objetivos específicos, lista de símbolos a utilizar, conclusiones y recomendaciones.
- `apoyops.pdf` una guía de _LaTeX_ para resolver las dudas más comunes.

## Ambientes de teoremas
Los ambientes de teoremas (teoremas, definiciones, proposiciones, corolarios, lemas, axomas, notas y ejemplos) están configurados para numerarlos de forma consecutiva respecto al capítulo sin discriminar el tipo.

```
\begin{defn} Definición \end{defn}
\begin{axm} Axioma \end{axm}
\begin{exa} Ejemplo \end{exa}
\begin{rem} Nota \end{rem}

\begin{thm} Teorema \end{thm}
\begin{cor} Corolario \end{cor}
\begin{lem} Lema \end{lem}
\begin{prp} Proposición \end{prp}
```

### Contacto

William Roberto Gutiérrez-Herrera, _wgutierrez at ecfm dot usac dot edu dot gt_.
