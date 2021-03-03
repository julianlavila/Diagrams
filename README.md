Here is a template to make easy diagrams for academic use
---------------------------------------------------------

For the construction of the diagram we are going to use the [nomnoml
package](https://github.com/rstudio/nomnoml)

``` r
nomnoml::nomnoml("[Hello]-[World!]")
```

![](README_files/figure-markdown_github/unnamed-chunk-1-1.png)

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

![](README_files/figure-markdown_github/unnamed-chunk-2-1.png)

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

![](README_files/figure-markdown_github/unnamed-chunk-3-2.png)
