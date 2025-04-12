# pandas-notes
occasional thing to look up again
# Sampling
```python
import pandas as pd

df = pd.DataFrame({'id': range(100), 'value': range(100, 200)})

# Ensure consistent ordering
df = df.sort_values('id').reset_index(drop=True)

# Sample 20% of rows consistently
sampled = df.sample(frac=0.2, random_state=42)
```
