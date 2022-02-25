```python
#APIs# 
#Importar cotação do dólar no neste momento usando APIs,#
import requests
import json
cotacoes = requests.get('https://economia.awesomeapi.com.br/last/USD')
cotacoes_dic = cotacoes.json()
print('A cotação do dólar neste momento é de R${:.2f}'.format(float(cotacoes_dic['USDBRL']['bid'])))
    #print('Não compre {} neste momento'.format(cotacoes_dic['USDBRL']))
```

    A cotação do dólar neste momento é de R$5.12
    
