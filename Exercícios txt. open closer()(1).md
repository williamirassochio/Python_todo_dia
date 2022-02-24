```python
arquivo = open('Alunos.txt','r')
linhas = arquivo.readlines()

#indicadores
qtd_anuncio = 0
qtd_org = 0
qtd_yt_org = 0
qtd_igfb_org = 0
qtd_site_org = 0

#percorrer
del linhas[:4]
for linha in linhas:
    email,origem = linha.split(',')
    if '_org' in origem:
        qtd_org += 1
        if 'hashtag_yt_org' in origem:
            qtd_yt_org += 1
        if 'hashtag_site_org' in origem:
            qtd_site_org += 1
        if 'hashtag_ig_org' in origem or 'hashtag_igfb_org' in origem:
            qtd_igfb_org +=1 
    else:
        qtd_anuncio += 1
        
#Fechar arquivo
arquivo.close()

with open('indicadores.txt','w') as arquivo_indicadores:
    arquivo_indicadores.write('Quantidade Anuncio: {}\n'.format(qtd_anuncio))
    arquivo_indicadores.write('Quantidade Orgânico: {}\n'.format(qtd_org))
    arquivo_indicadores.write('Quantidade YouTube: {}\n'.format(qtd_yt_org))
    arquivo_indicadores.write('Quantidade Instagram: {}\n'.format(qtd_igfb_org))
    arquivo_indicadores.write('Quantidade Site: {}\n'.format(qtd_site_org))
print('Fim do código')
```

    Fim do código
    
