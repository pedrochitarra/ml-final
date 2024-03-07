# PUC Minas
## Pós-Graduação em Ciência de Dados e Big Data
## Machine Learning
## Professor: Gabriel Oliveira Assunção
### Trabalho Prático - relatório da base de dados

#### Alunos:
- Guilherme de Gouvêa Almada
- Pedro Henrique Batista Chitarra

---

# Stellar Classification Dataset
https://www.kaggle.com/datasets/fedesoriano/stellar-classification-dataset-sdss17/

Arquivo MD: https://github.com/pedrochitarra/ml-final

## Contexto
Na astronomia, a classificação estelar é a classificação de estrelas com base em suas características espectrais. O esquema de classificação de galáxias, quasares e estrelas é um dos mais fundamentais na astronomia. A catalogação precoce de estrelas e sua distribuição no céu levou à compreensão de que elas compõem nossa própria galáxia e, seguindo a distinção de que Andrômeda era uma galáxia separada da nossa, inúmeras galáxias começaram a ser pesquisadas à medida que telescópios mais poderosos eram construídos. Este conjunto de dados tem como objetivo classificar estrelas, galáxias e quasares com base em suas características espectrais.

O estudo estelar de identificação e classificação de corpos tem inúmeras aplicações, desde mais diretas, como mapeamento do universo, até mais complexas como varredura de busca por planetas potencialmente habitáveis, ou indiretas, como uso de software de reconhecimento de estrela em imagens de tecidos humanos para detectar possíveis células mortas e focos de câncer.

## Conteúdo
Os dados consistem em 100.000 observações do espaço obtidas pelo SDSS (Sloan Digital Sky Survey). Cada observação é descrita por 17 colunas de características e 1 coluna de classe que a identifica como sendo uma estrela, galáxia ou quasar.

## Variáveis
- obj_ID: Identificador de Objeto, o valor único que identifica o objeto no catálogo de imagens usado pelo CAS
  - Variável categórica nominal (identificadora)
- alpha:  angulo de Ascensão Reta, de acordo com o Sistema Equatorial[1] (no ponto de época J2000[2])
  - Variável numérica contínua
- delta:  angulo de Declinação, de acordo com o Sistema Equatorial[1]  (no ponto de época J2000[2])
  - Variável numérica contínua
- u: Filtro Ultravioleta no sistema fotométrico
    - Variável numérica contínua
- g: Filtro Verde no sistema fotométrico
    - Variável numérica contínua
- r: Filtro Vermelho no sistema fotométrico
    - Variável numérica contínua
- i: Filtro de Infravermelho Próximo no sistema fotométrico
    - Variável numérica contínua
- z: Filtro de Infravermelho no sistema fotométrico
    - Variável numérica contínua
- run_ID: Número de Execução usado para identificar a varredura específica
    - Variável categórica nominal (identificadora)
- rerun_ID: Número de Repetição para especificar como a imagem foi processada
    - Variável categórica nominal (identificadora)
- cam_col: Coluna da Câmera para identificar a linha de varredura dentro da execução
    - Variável numérica discreta
- field_ID: Número do Campo para identificar cada campo
    - Variável numérica discreta
- spec_obj_ID: ID Único usado para objetos espectroscópicos ópticos (isso significa que duas observações diferentes com o mesmo spec_obj_ID devem compartilhar a classe de saída)
    - Variável categórica nominal (identificadora)
- **class: classe de objeto (galáxia, estrela ou objeto quasar)**
    - Variável categórica nominal (alvo)
- redshift[3]: valor de desvio para o vermelho com base no aumento no comprimento de onda
    - Variável numérica contínua
- plate: ID da placa, identifica cada placa no SDSS
    - Variável numérica discreta (identificadora)
- MJD: Data Juliana Modificada, usada para indicar quando um determinado dado do SDSS foi obtido
    - Variável numérica discreta
- fiber_ID: ID da fibra que identifica a fibra que apontou a luz no plano focal em cada observação
    - Variável numérica discreta

1. O sistema de coordenadas equatoriais descreve as posições dos objetos celestes em relação ao equador celeste. A ascensão reta (AR) mede a distância angular de um objeto para o leste ao longo do equador celeste, começando do Primeiro Ponto de Áries. A ascensão reta é o equivalente celeste da longitude terrestre. A declinação (Dec) mede a distância angular de um objeto ao norte ou ao sul do equador celeste.
2. Época J2000 é a data 01 de Janeiro de 2000, data referência padrão para indicar as coordenadas dos corpos estelares.
3. Redshift é o desvio para vermelho do comprimento da onda capturada, utilizado para discernir se o objeto observado está se movendo, e caso esteja, se o mesmo se move na direção do observador, ou para longe.

## Observações
1. Duas observações diferentes com o mesmo spec_obj_ID devem compartilhar a classe de saída

## Referências
- https://arxiv.org/ftp/arxiv/papers/1512/1512.05272.pdf
- https://pweb.cfa.harvard.edu/research/topic/medical-applications
