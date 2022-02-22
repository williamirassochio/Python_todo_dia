```python
#APIs# 
#Importar cotação do dólar no neste momento usando APIs,#
import requests
import json
cotacoes = requests.get('https://economia.awesomeapi.com.br/last/USD')
cotacoes_dic = cotacoes.json()
print(cotacoes_dic)
print('A cotação do dolar neste momento é de R${:.2f}'.format(float(cotacoes_dic['USDBRL']['bid'])))
```

    {'USDBRL': {'code': 'USD', 'codein': 'BRL', 'name': 'Dólar Americano/Real Brasileiro', 'high': '5.1038', 'low': '5.1038', 'varBid': '0.0003', 'pctChange': '0', 'bid': '5.1036', 'ask': '5.1041', 'timestamp': '1645478997', 'create_date': '2022-02-21 18:29:57'}}
    A cotação do dolar neste momento é de R$5.10
    
