```python
#Digamos que você está analisando as vendas de produtos de uma empresa de varejo.

#Essa lista tem: (produto, vendas de 2019, vendas de 2020) para cada produto.

#Crie uma lista com as vendas de 2019 e produtos, quantidade de produtos vendidos e a quantidade e produto mais vendido de 2019.

#Criar uma  List Comprehension para executar o código.

vendas_produtos = [('iphone', 558147, 951642), ('galaxy', 712350, 244295), ('ipad', 573823, 26964), ('tv', 405252, 787604), ('máquina de café', 718654, 867660), ('kindle', 531580, 78830), ('geladeira', 973139, 710331), ('adega', 892292, 646016), ('notebook dell', 422760, 694913), ('notebook hp', 154753, 539704), ('notebook asus', 887061, 324831), ('microsoft surface', 438508, 667179), ('webcam', 237467, 295633), ('caixa de som', 489705, 725316), ('microfone', 328311, 644622), ('câmera canon', 591120, 994303)]

lista_vendasprodutos2019 = []
lista_vendasprodutos2019 = [(vendas_2019,produtos) for produtos,vendas_2019,vendas_2020 in vendas_produtos]
print(lista_vendasprodutos2019)
print(len(lista_vendasprodutos2019))
print(max(lista_vendasprodutos2019))
```

    [(558147, 'iphone'), (712350, 'galaxy'), (573823, 'ipad'), (405252, 'tv'), (718654, 'máquina de café'), (531580, 'kindle'), (973139, 'geladeira'), (892292, 'adega'), (422760, 'notebook dell'), (154753, 'notebook hp'), (887061, 'notebook asus'), (438508, 'microsoft surface'), (237467, 'webcam'), (489705, 'caixa de som'), (328311, 'microfone'), (591120, 'câmera canon')]
    16
    (973139, 'geladeira')
    
