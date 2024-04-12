# Plantilla para elaborar trabajo de graduación - [ECFM](https://ecfm.usac.edu.gt/)

Este repositorio contiene los ficheros para escribir el trabajo de graduación para las carreras de matemáticas o física.

La plantilla inicial se realizó con Texlive 2015, TeXstudio, sobre el sistema Operativo GNU/Linux Debian 8.2. Las actualizaciones más recientes se hicieron con MacOS Sonoma 14.4.1 (TeXstudio 4.7.3 y TeX Live 2024), el autor nunca la ha corrido con Windows pero supone que no debe haber problema.

## Importante

- Al terminar el trabajo de graduación y ser aprobado por el asesor, debe presentar una copia impresa del mismo junto a la carta de aprobación del asesor al Jefe de Departamento correspondiente. Notar que tiene la línea `%\OrdenImpresion{ordenImpresion} % del archivo _TesisTotal.tex_ o _TesisTotalBibTeX.tex_ incluye orden de impresión, guardada en pdf` está comentada, **se descomentará más adelante**.
- Al tener la aprobación del Jefe de Departamento, debe ingresar el expediente con el Director de la ECFM (trabajo de graduación, carta de asesor y carta del jefe de departamento).
- El Director le dará la **Orden de Impresión**, ésta la debe escanear y guardar en un archivo pdf con el nombre `ordenImpresion.pdf`.
- Debe compilar otra vez su archivo `.tex` descomentando la línea `\OrdenImpresion{ordenImpresion} % incluye orden de impresión, guardada en pdf`, con esto tendrá completo su trabajo de graduación para ser entregado en la [Biblioteca Central](http://www.biblioteca.usac.edu.gt/biblioteca2023/tesis.html).

## Descripción del contenido

- `thesisECFM.cls` fichero modificado a partir de `book.cls`.
- `macros.sty` fichero que hace llamada a los paquetes: _babel, ifthen, textcase, inputenc fontenc, amsfonts, amsmath, amssymb, amsthm, mathrsfs, geometry, setspace, caption, color, longtable, pdfpages, graphicx, hyperref, url, breakurl_. La mayoría de estos paquetes ya están preconfigurados con las especificaciones para el trabajo de graduación, **NO SE DEBEN CAMBIAR**, si necesita otros paquetes los debe llamar desde `TesisTotal.tex` o `TesisTotalBibTex.tex` y hacer las configuraciones respectivas.
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
Los ambientes de teoremas (teoremas, definiciones, proposiciones, corolarios, lemas, axiomas, notas y ejemplos) están configurados para numerarlos de forma consecutiva respecto al capítulo sin discriminar el tipo.

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
