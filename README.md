A aplicação compara duas fotos e determina se ambas pertencem à mesma pessoa, além de fornecer métricas que ajudam a entender o nível de similaridade entre os rostos analisados. 
Como estudo de caso, foram utilizadas imagens dos sambistas brasileiros Zeca Pagodinho e Arlindo Cruz.

<img width="706" height="560" alt="Image" src="https://github.com/user-attachments/assets/3d5ba2ca-0ad8-4d3e-bea0-0ea8353b2a1b" />

<img width="599" height="558" alt="Image" src="https://github.com/user-attachments/assets/93028d9f-009a-402f-bb15-98c790cfd915" />



O reconhecimento facial é realizado através da função:

DeepFace.verify()


Essa função processa as imagens e retorna um dicionário, contendo informações sobre a comparação facial.

Estrutura do retorno
{
  'verified': True,
  'distance': 0.23,
  'threshold': 0.4,
  'model': 'VGG-Face'
}

Significado dos campos

verified
Resultado final da verificação. Indica se as duas imagens são reconhecidas como sendo da mesma pessoa.

distance
Valor numérico que representa a distância entre as características faciais extraídas das imagens. Valores menores indicam maior similaridade.

threshold
Limite utilizado pelo modelo para decidir se a distância encontrada é suficiente para confirmar a identidade.

model
Modelo de Deep Learning empregado no processo de reconhecimento facial.
