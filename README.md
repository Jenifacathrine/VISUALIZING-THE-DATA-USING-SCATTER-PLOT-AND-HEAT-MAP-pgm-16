# VISUALIZING-THE-DATA-USING-SCATTER-PLOT-AND-HEAT-MAP-pgm-16
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
x = np.random.rand(100) * 10 # X values (random numbers between 0 and 10)
y = np.random.rand(100) * 10 # Y values (random numbers between 0 and 10)
heatmap_data = np.random.rand(10, 10)
plt.figure(figsize=(12, 6)) 
plt.subplot(1, 2, 1) 
plt.scatter(x, y, color=&#39;blue&#39;, alpha=0.7)
plt.title(&quot;Scatter Plot&quot;)
plt.xlabel(&quot;X-axis&quot;)
plt.ylabel(&quot;Y-axis&quot;)
plt.subplot(1, 2, 2)
sns.heatmap(heatmap_data, annot=True, cmap=&#39;coolwarm&#39;, cbar=True)
plt.title(&quot;Heatmap&quot;)
plt.tight_layout()
plt.show()
