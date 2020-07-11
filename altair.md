# Import

import altair as alt
import pandas as pd

# Gráfico de barras

alt.Chart(PD).mark_bar().encode(
    x='column X',
    y= 'Column Y'
)

# Gráfico de puntos
alt.Chart(brain).mark_point().encode(
    x='Brain Weight',
    y= 'Body Weight'
)


# Gráfico de líneas

trends_line = alt.Chart(trends).mark_line().encode(
    x='yearmonth(date):T',
    y= 'mean(value)',
    color='search_term'
).properties( 
  width=1200,
  height=400, 
  title="Busquedas Medias de terminos de Data Science" 
).interactive()
