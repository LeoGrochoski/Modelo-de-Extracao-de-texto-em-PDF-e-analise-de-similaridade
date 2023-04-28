# Modelo de Extracao de texto de PDF e analise de similaridade entre textos

### Resumo: 

Modelo criado visando extrair texto de dois ou mais arquivos PDF a fim de realizar uma analise de similaridade entre seus conteudos.

### Ferramentas: 

Foi utilizado o jupyter notebook dentro do ambiente Anaconda para ser escrito o codigo em python 

### Bibliotecas: 

[**io**](https://docs.python.org/3/library/io.html): Biblioteca padrão do Python que fornece ferramentas para trabalhar com arquivos em memória, em vez de armazená-los em disco. Ela é útil para lidar com dados que não precisam ser armazenados permanentemente em um arquivo.

[**re**](https://docs.python.org/3/library/re.html): Biblioteca padrão do Python para expressões regulares. Ela fornece uma sintaxe para trabalhar com padrões de texto e permite pesquisar, substituir e manipular strings com base nesses padrões.

[**string**](https://docs.python.org/3/library/string.html): Biblioteca padrão do Python para manipulação de strings. Ela fornece uma série de constantes úteis, como caracteres ASCII, dígitos e pontuação.

[**sklearn**](https://scikit-learn.org/0.21/documentation.html): Biblioteca popular para aprendizado de máquina em Python. Ela fornece ferramentas para pré-processamento de dados, seleção de recursos, modelagem e avaliação, entre outras tarefas relacionadas ao aprendizado de máquina.

[**TfidfVectorizer**](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html): Classe da biblioteca sklearn que implementa a vetorização de termos com TF-IDF (term frequency-inverse document frequency). É uma técnica comum para representar documentos como vetores de recursos numéricos, que podem ser usados como entrada para modelos de aprendizado de máquina.

[**cosine_similarity**](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html): Função da biblioteca sklearn que calcula a similaridade do cosseno entre dois vetores. É comumente usada para comparar vetores de recursos numéricos em tarefas de aprendizado de máquina.

[**pdfminer**](https://pdfminersix.readthedocs.io/en/latest/): Biblioteca Python para processamento de PDF. Ela fornece ferramentas para extrair texto, imagens e outros dados de arquivos PDF, além de outras tarefas relacionadas ao processamento de PDF. A classe extract_text fornece uma interface para extrair o texto de um arquivo PDF.

## Funcionamento:

Foram utilizados dois pdfs retirados de vagas anunciadas pelo linkedin, com estes pdf's foi feito um pré-processamento para limpar os textos, após os pdf's são incluidos em dois diretorios no codigo, são lidos, extraidos e processados. Depois é checado a qualidade dessa extração e emfim é feito o calculo de similaridade, gera a nota baseada em regras pré estabelecidas de negocio e por fim apresentado o resultado. 
