Here is a template to make easy diagrams for academic use
---------------------------------------------------------

For the construction of the diagram we are going to use the [nomnoml
package](https://github.com/rstudio/nomnoml)

``` r
nomnoml::nomnoml("[Hello]-[World!]")
```

    ## PhantomJS not found. You can install it with webshot::install_phantomjs(). If it is installed, please make sure the phantomjs executable can be found via the PATH variable.

<!--html_preserve-->

<script type="application/json" data-for="htmlwidget-3060432fc5cd0e3320e9">{"x":{"code":"\n#fill: #FEFEFF\n#lineWidth: 1\n#zoom: 4\n#direction: right\n\n[Hello]-[World!]","svg":false},"evals":[],"jsHooks":[]}</script>
<!--/html_preserve-->

Now a more structures diagram

``` nomnoml
#stroke: #a86128
#direction: down
[<frame>Decorator pattern|
  [<abstract>Component||+ operation()]
  [Client] depends --> [Component]
  [Decorator|- next: Component]
  [Decorator] decorates -- [ConcreteComponent]
  [Component] <:- [Decorator]
  [Component] <:- [ConcreteComponent]
]
```

<!--html_preserve-->

<script type="application/json" data-for="htmlwidget-2129ab33113cdbda782b">{"x":{"code":"\n#fill: #FEFEFF\n#lineWidth: 1\n#zoom: 4\n#direction: right\n\n#stroke: #a86128\n#direction: down\n[<frame>Decorator pattern|\n  [<abstract>Component||+ operation()]\n  [Client] depends --> [Component]\n  [Decorator|- next: Component]\n  [Decorator] decorates -- [ConcreteComponent]\n  [Component] <:- [Decorator]\n  [Component] <:- [ConcreteComponent]\n]","svg":false},"evals":[],"jsHooks":[]}</script>
<!--/html_preserve-->

### Modeling procces

``` nomnoml
#stroke: steelblue
#arrowSize: 1
#bendSize: 0.3
#direction: right
#gutter: 9
#edgeMargin: 0
#edges: hard | rounded
#fillArrows: false
#font: Calibri
#fontSize: 12
#leading: 1.25
#lineWidth: 3
#padding: 8
#spacing: 40
#title: filename
#zoom: 1
[<frame>Ocurrences|
  [Data Sources|GBif|SciELO|PubMed|Google Scholar]-> [Records search|"Cutaneous"|"Leishmaniasis"|"Vectors"|"Lutzomyia"]
 [Records search]->[Data cleaning |Duplicates|long/lat inconcistencys|Polygons centroids|Sea records|Record uncertainty >400Km]
 [Data cleaning]->[Final data base |Species,Longitude,Latitude]
 
]
```

<!--html_preserve-->

<script type="application/json" data-for="htmlwidget-a1be836e7f5a49197922">{"x":{"code":"\n#fill: #FEFEFF\n#lineWidth: 1\n#zoom: 4\n#direction: right\n\n#stroke: steelblue\n#arrowSize: 1\n#bendSize: 0.3\n#direction: right\n#gutter: 9\n#edgeMargin: 0\n#edges: hard | rounded\n#fillArrows: false\n#font: Calibri\n#fontSize: 12\n#leading: 1.25\n#lineWidth: 3\n#padding: 8\n#spacing: 40\n#title: filename\n#zoom: 1\n[<frame>Ocurrences|\n  [Data Sources|GBif|SciELO|PubMed|Google Scholar]-> [Records search|\"Cutaneous\"|\"Leishmaniasis\"|\"Vectors\"|\"Lutzomyia\"]\n [Records search]->[Data cleaning |Duplicates|long/lat inconcistencys|Polygons centroids|Sea records|Record uncertainty >400Km]\n [Data cleaning]->[Final data base |Species,Longitude,Latitude]\n \n]","svg":false},"evals":[],"jsHooks":[]}</script>
<!--/html_preserve-->
