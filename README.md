# quarto-shiny-test
A demo of using shiny ui and server modules in a shiny dashboard          
         
- This repo contains an example of how shiny server and ui modules can be included in an interactive quarto document (running a shiny runtime)
- The shiny is adapted from <a href="https://github.com/Russell-Shean/mapasaurus/tree/main/inst/route-explorer-app">here</a>
- The quarto document containing the shiny is <a href="https://github.com/Russell-Shean/quarto-shiny-test/blob/main/demo_shiny.qmd">here</a>
- The shiny processes a gpx file downloaded from strava. I included an <a href="https://github.com/Russell-Shean/quarto-shiny-test/blob/main/753089014.gpx">example file</a> for testing. Just download it and then upload it to the shiny.
- The modules are stored in the R folder.
- It appears that the R folder isn't automatically recognized so I added source calls in a setup context. (see lines 9, 32-35 in demo_shiny.qmd)
- I put a server context into the quarto document instead of using a shiny.R or global.R file.
- Here's a link to some < a href="https://quarto.org/docs/interactive/shiny/execution.html">documentation</a> with more possibile options: 
- I have not tried this with shinylive/webR because one of the packages I use in the shiny has a curl dependency and isn't yet available for webR/WebAssembly


