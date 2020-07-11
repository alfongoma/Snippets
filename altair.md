# Import

import altair as alt
import pandas as pd

# Gráfico de barras

alt.Chart(PD).mark_bar().encode(
    x='column X',
    y= 'Column Y'
)
