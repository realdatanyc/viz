# viz
data visualization

[Squirrel Census Website](https://www.thesquirrelcensus.com/)

[Squirrel Census Presentation](https://youtu.be/6JGPXuxayw4?t=1879)

[NYC Maps](https://www.nyc.gov/nyc-resources/nyc-maps.page)

' select files on computer
from google.colab import files
uploaded = files.upload()


loading from local drive

import pandas as pd
import io
 
df = pd.read_csv(io.BytesIO(uploaded['file.csv']))
print(df)

Loading Data from Github to Googe Colab

url = 'copied_raw_github_link'
df = pd.read_csv(url)
