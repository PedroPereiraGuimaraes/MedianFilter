# Filtro Mediano
O filtro mediano é uma técnica de filtragem digital não linear , frequentemente usada para remover ruídos de uma imagem ou sinal.

A ideia principal do filtro de medianas é percorrer o sinal entrada por entrada, substituindo cada entrada pela mediana das entradas vizinhas. O padrão de vizinhos é chamado de "janela", que desliza, entrada por entrada, sobre todo o sinal. Para sinais unidimensionais, a janela mais óbvia é apenas as primeiras entradas anteriores e seguintes, enquanto para dados bidimensionais (ou de dimensão superior), a janela deve incluir todas as entradas dentro de um determinado raio ou região elipsoidal (ou seja, o filtro mediano não é um filtro separável ).

# Imagens 

<div align="left">
  <img height="400em" src="https://user-images.githubusercontent.com/71026262/200625721-351c3135-2adb-4980-ba83-ee331e2cd05a.png"/>
  <img height="400em" src="https://user-images.githubusercontent.com/71026262/200625732-87ae083e-087b-4a7b-96b0-b5635332be3d.png"/>
</div>

# Exemplo
O filtro mediano geralmente é usado para reduzir o ruído em uma imagem. Estaremos lidando com o ruído de sal e pimenta no exemplo abaixo. O método Median_Filter recebe 2 argumentos, matriz de imagem e tamanho do filtro. Digamos que você tenha seu array Image na variável chamada img_arr e queira remover o ruído dessa imagem usando o filtro mediano 3x3. É assim que se faz.

```
removed_noise = FiltroDeMediana(arr, 3)
```

Para o filtro mediano 5x5, você só precisa alterar o segundo argumento para 5 e assim por diante.
