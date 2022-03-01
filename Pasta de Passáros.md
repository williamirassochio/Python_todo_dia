```python
#Criar pastas com nome de passáros
from pathlib import Path
import shutil
passaros = ['Trinca Ferro','Azulão','Coleiro']
for passaro in passaros:
    Path('mpasta nova/{}'.format(passaro)).mkdir()
```
