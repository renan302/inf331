## Tarefa sobre catálogo de componentes

![Foodmart](notebook/components-01-catalog.ipynb)

## Tarefa Web Components 1
> <dcc-trigger  label="Mundo" value="Trump é contaminado por covid19" action="noticia/mundo/politica" ></dcc-trigger>
> <dcc-trigger label="Brasil P" value="Presidente é contaminado por covid19" action="noticia/brasil/politica" ></dcc-trigger>
> <dcc-trigger label="Brasil E" value="PSG VS ATALANTA" action="noticia/brasil/esporte" ></dcc-trigger>
> <dcc-trigger label="Bahia" value="Esportes estão suspensos na Bahia" action="noticia/bahia/esporte"></dcc-trigger>
> <dcc-lively-talk duration="0s" character="doctor" speech="Estou lendo: "><subscribe-dcc topic="noticia/+/politica"></subscribe-dcc></dcc-lively-talk>
> <dcc-lively-talk duration="0s" character="nurse" speech="Estou lendo:  "><subscribe-dcc topic="noticia/brasil/+"></subscribe-dcc></dcc-lively-talk>
> <dcc-lively-talk duration="0s" character="patient" speech="Estou lendo: "> <subscribe-dcc topic="noticia/#"></subscribe-dcc> </dcc-lively-talk>

## Tarefa Web Components 2
> <dcc-trigger label="Buscar Noticia" action="next/rss"></dcc-trigger>
> <dcc-rss publish="noticias/science" source="https://www.wired.com/category/science/feed"><subscribe-dcc topic="next/rss" role="step"></subscribe-dcc></dcc-rss>
> <dcc-rss publish="noticias/design" source="https://www.wired.com/category/design/feed"><subscribe-dcc topic="next/rss" role="step"></subscribe-dcc></dcc-rss>
> <dcc-aggregator publish="aggregate/science" quantity="3"><subscribe-dcc topic="noticias/science"></subscribe-dcc></dcc-aggregator>
> <dcc-lively-talk id="doctor" duration="0s" character="doctor" speech="News "><subscribe-dcc topic="aggregate/science"></subscribe-dcc></dcc-lively-talk>
> <dcc-lively-talk id="nurse" duration="0s" character="nurse" speech="News "><subscribe-dcc topic="noticias/science"></subscribe-dcc></dcc-lively-talk>
> <dcc-lively-talk id="patient" duration="0s" character="patient" speech="News "><subscribe-dcc topic="noticias/design"></subscribe-dcc></dcc-lively-talk>