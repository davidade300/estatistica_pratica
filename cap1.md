## Estimativas da variabilidade

- também chamada de dispersão, mede se os valores dos dados estão muito agrupados ou distribuidos

### Termos chave para estimativas de variabilidade

- Desvios (erros,resíduos)
    - Diferança entre os valores observados e a estimativa de localização.
- Variância (erro médio quadratico):
    - Soma dos quadrados dos devios da média, divididos por _n-1_, em que n é o número dos valores de dados.
- Desvio-padrão:
    - raiz quadrada da variância.
- Desvio absoluto médio (norma l1, norma Manhattan):
    - Média do valor absoluto dos desvios da média.
- Desvio absoluto mediano da mediana
    - Mediana dos valores absolutos dos desvios da mediana.
- Amplitude:
    - Diferença entre o maior e o menor valor no conjunto de dados.
- Estatísticas ordinais (classificação):
    - Estimativass baseadas nos valores de dados classificados do menor ao maior.
- Percentil (quantil):
    - Valor tal que a porcentagem _P_ dos valores assume esse valor ou menos e a porcentagem _100-P_ dos valores assume
      esse valor ou mais.
- Amplitude interquartílica:
    - Diferença entre o 75º percentil (terceiro quartil) e o 25º percentil (primeiro quartil).

### Desvio padrão e Estimativas relacionadas

- As estimativas de variação mais utilizadas são baseadas nas diferenças, ou nos _devios_, entre a estimativa de
  localização e o dado observado.
- considere o conjunto {1,4,4}
    - media: 3
    - desvio da média: 1 (1-3 = -2), (4-3 = 1), (4-3 = 1)
    - valor absoluto dos desvios da média: 2,1,1
    - média dos desvios: 1,33 ((2+1+1)/3)
- a média dos desvios é conhecida como _desvio absoluto médio_ e é calculada a partir da formula:
  $$ \frac{\Sigma_{i=1}^n|x_i - \bar{x}|}{n} $$
    - em que $\bar{x}$ é a média da amostra.

- As estimativas de variabilidade mais conhecidas são a variância e o desvio-padrão, que são baseados nos desvios
  quadráticos. A variância é uma média dos desvio quadráticos e o desvio-padrão é a raiz quadrada da variância.
    - variância:
      $$ \frac{\Sigma_{i=1}^n (x_i - \bar{x})^2}{n} $$
    - Desvio padrão
      $$ \sqrt{variância}$$
      $$ alternativamente $$
      $$ \sqrt{\frac{\Sigma_{i=1}^n (x_i - \bar{x})^2}{n}} $$
- Nem a variância nem o desvio-padrão, nem o desvio absoluto médio são totalmente robustos frente aos valores atípicos e
  aos valores extremos. A variância e o desvio-padrão são especialmente sensíveis aos valores atípicos, pois são
  baseados nos desvios quadráticos. Uma estimativa de variabilidade robusta é o _desvio absoluto mediano da mediana ou
  MAD_.
  - O desvio absoluto mediano é dado por:
  $$ Mediana(|x_1 - m|,|x_2 - m|,...,|x_n - m|)$$
  - em que:
    - $m$ é a mediana da amostra.
- Como a mediana, o MAD não é influenciado pelos valores atípicos. 
