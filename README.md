# Seaborn

**Seaborn, Matplotlib kütüphanesine yüksek seviye arayüz sağlayan bir kütüphanedir.**

Anacondaya Seaborn'u Kurma
```
conda install seaborn
```

Kütüphane kurulumu
```
import seaborn as sns
```


```
# Import the necessary libraries
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np
from matplotlib.colors import ListedColormap

# Define a variable N
N = 500

# Construct the colormap
current_palette = sns.color_palette("muted", n_colors=5)
cmap = ListedColormap(sns.color_palette(current_palette).as_hex())

# Initialize the data
data1 = np.random.randn(N)
data2 = np.random.randn(N)
# Assume that there are 5 possible labels
colors = np.random.randint(0,5,N)

# Create a scatter plot
plt.scatter(data1, data2, c=colors, cmap=cmap)

# Add a color bar
plt.colorbar()

# Show the plot
plt.show()
```

<a href="http://fvcproductions.com"><img src="https://miro.medium.com/max/1440/0*GVUIGoDbtjf4znjN.png" title="FVCproductions" alt="FVCproductions"></a>




