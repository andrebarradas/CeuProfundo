# CeuProfundo

![](SMd.png)

[PT-BR]
**CeuProfundo** é um *script* em Python 3 para plotagem de cartas celestes retangulares e polares utilizando
dados de catálogos estelares e de objetos de céu profundo.
O tamanho e a resolução são ajustáveis para visualização e impressão.
A exibição de estrelas e objetos celestes pode ser desabilitada, criando
cartas em branco que podem ser utilizadas em atividades educacionais.
 
[EN]
**CeuProfundo** is a Python 3 script to plot sky charts in rectangular and polar modes with data 
from star and deep sky objects catalogs.
Size and resolution can be adjusted for viewing or printing.
Star and DSO exhibition can be toggled off to generate blank templates for
educational purposes.

### Instruções:

* Baixe e salve locamente os arquivos deste repositório.
* Você precisará ter o ![Python 3](https://www.python.org/downloads/) instalado com os pacotes [NumPy](https://numpy.org/), [Pandas](https://pandas.pydata.org/) e [Matplotlib](https://matplotlib.org/). A distribuição [Anaconda](https://www.anaconda.com/products/individual) inclui todos os pacotes necessários.
* Execute o *script* a partir da linha de comando, no diretório onde os arquivos foram salvos.
    Para ver os argumentos opcionais use:
    ```
    python CeuProfundo.py --h
    ```
* Argumentos opcionais:
    ```
  -h, --help        show this help message and exit
  -v, --version     show program's version number and exit
  -S, --Stars       Plota cartas com estrelas.
  -M, --Messier     Plota cartas com objetos dos catálogos Messier e Caldwell.
  -D, --Dark        Usa fundo escuro.
  -r, --retangular  Plota carta retangular.
  -s, --sul         Plota carta polar sul.
  -n, --norte       Plota carta polar norte.
  -d, --dupla       Plota carta polar norte e sul.
  -g, --png         Muda extensão do arquivo de saída para .png.
    ```
* Exemplos.
    * Para gerar a carta dupla em pdf, com os hemisférios norte e sul em fundo claro, incluindo as estrelas do Bright Star Catalogue e os objetos de céu profundo dos catálogos Messier e Caldwell:
    ```
    python CeuProfundo.py -S -M -d
    ```
    * Para gerar a carta dupla em png, com os hemisférios norte e sul em fundo escuro, incluindo as estrelas do Bright Star Catalogue e os objetos de céu profundo dos catálogos Messier e Caldwell:
    ```
    python CeuProfundo.py -S -M -D -d -g
    ```
