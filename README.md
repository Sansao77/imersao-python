# Imersão Python - Do Excel à Análise de Dados (Alura)

Esse repositório contem todo o conhecimento adquirido e praticado durante a semana de imersão python da [Alura](https://www.alura.com.br/?utm_term=alura&utm_campaign=%5BSearch%5D+%5BPerformance%5D+-+Institucional&utm_source=adwords&utm_medium=ppc&hsa_acc=7964138385&hsa_cam=386166608&hsa_grp=21666755648&hsa_ad=609948692827&hsa_src=g&hsa_tgt=aud-546438175126:kwd-300088401&hsa_kw=alura&hsa_mt=e&hsa_net=adwords&hsa_ver=3&gad_source=1&gclid=Cj0KCQjw8J6wBhDXARIsAPo7QA_4QoWoSVWiXODbOyOFikcljl_pVHze-HbwkOTAL00phiVa_9r5kX0aAlLtEALw_wcB)

## 1º Aula: Análise Exploratória com Google Sheets

- Analise Exploratória ([AED](https://ebaconline.com.br/blog/analise-exploratoria-de-dados-o-que-e#:~:text=O%20que%20é%20Análise%20Exploratória,e%20extrai%20conhecimento%20desses%20dados.)): É um processo importante do trabalho do cientista de dados porque é a partir dela que o cientista de dados vai obtendo insights e coletando informações que vão alimentar os modelos de machine learning.
- [Planilha utilizada](https://docs.google.com/spreadsheets/d/1JSPdWWxoG28Mn5PSRDucq6Nol_TlkceexIbvWOkkClc/edit?usp=sharing)
- Explicações de como usar os comandos da planilha Excel
    - função [VLOOKUP/PROCV()](https://canaltech.com.br/software/como-fazer-a-formula-procv-no-excel/)
        - Chave de pesquisa: valor que é desejado na busca;
        - A matriz_tabela avalia a quantidade de colunas sendo avaliadas na pesquisa (Se for 'A:B' avalia as colunas A e B, se for 'A:D' avalia as colunas A, B, C e D)
            - O nome do lado da matriz representa de qual tabela as colunas sendo avaliadas são.
        - O valor indice representa de qual coluna nos vamos pegar o valor, sendo '1' a primeira coluna da matriz, '2' para a segunda e assim por diante
        - O valor de intervalo, sendo esse o ultimo parametro do PROCV, pode ter dois valores:
            - '0' se não for aceitavel aproximar os valores da coluna
            - '1' se for aceitavel aproximar os valores da coluna
    - Tem como formatar os valores da planilha para valores contabilizaveis, como o real (R$)
    - Como usar a condicional [IF/SE()](https://support.microsoft.com/pt-br/office/usar-as-funções-se-com-e-ou-e-não-d895f58c-b36c-419e-b1f2-5c193a236d97)

## 2º Aula: Gráficos e Análises com Google Colab e Python Pandas

### Continuando com Excel

- Continuando o estudo das funções Excel
    - [MAX/MÁXIMO()](https://support.microsoft.com/pt-br/office/função-máximo-e0012414-9ac8-4b34-9a47-73e662c08098) - retorna o maior valor de relacionada linha ou coluna
    - [MIN/MÍNIMO()](https://support.microsoft.com/pt-br/office/função-mínimo-61635d12-920f-4ce2-a70f-96f202dcc152) - retorna o menor valor de relacionada linha ou coluna
    - [MÉDIA()](https://canaltech.com.br/apps/como-calcular-media-mediana-e-moda-no-excel/) - retorna a media dos valores de uma linha ou coluna
    - [MÉDIASE()](https://www.hashtagtreinamentos.com/formula-mediase-como-fazer) - retorna a media dos valores de uma linha ou coluna, dentro de um certo critério
    - [UNIQUE/ÚNICO()](https://support.microsoft.com/pt-br/office/função-único-c5ab87fd-30a3-4ce9-9d1a-40204fb85e1e) - Retorna todos os valores unicos, não repetidos, de uma lista especificada
    - [SUMIF/SOMASE()](https://support.microsoft.com/pt-br/office/função-somase-169b8c99-c05c-4483-a712-1697a653039b) - Serve para fazer as somas de valores especificos, dentro de um critério
    - [SUMIFS/SOMASES()](https://support.microsoft.com/pt-br/office/função-somase-169b8c99-c05c-4483-a712-1697a653039b) - Serve para fazer a soma de valores especificos, dentro de multiplos critérios
    - [COUNT/CONT.NÚM()](https://support.microsoft.com/pt-br/office/função-cont-núm-a59cd7fc-b623-4d93-87a4-d23bf411294c#:~:text=A%20função%20CONT.,ou%20uma%20matriz%20de%20números.) - Serve para contar a quantidade de células não vázias
    - [COUNTIF/CONT.SE()](https://support.microsoft.com/pt-br/office/função-cont-núm-a59cd7fc-b623-4d93-87a4-d23bf411294c#:~:text=A%20função%20CONT.,ou%20uma%20matriz%20de%20números.) - Serve para contar a quantidade de células não vázias, dentro de um certo critério
- Explicações de como criar um gráfico em Excel

### Analise de dados com Python

- Na aula foi usado o [Google Colab](https://colab.google)
    - Os arquivos do Colab não são salvos online, é necessário armazena-lós na sua maquina para utilização futura
- [Código](/python/aula2.ipynb);
- Estudo leve sobre como usar o pandas com base no Excel utilizado
- [SheetGPT](https://sheetgpt.ai), extensão de IA para o Google Sheets.
    - Ele usa o ChatGPT para criar informações
    - Um exemplo de comando seria: '= GPTLIST('Qualquer ideia de lista que você quiser')'

## 3º Aula: Manipulação de Dados e Criação de Gráficos com bibliotecas Python

- Nessa aula aprendemos como criar tabelas iguais as do Excel, mas usando a linguagem Python e a biblioteca Python
- Explicações da função [merge](https://medium.com/data-hackers/pandas-combinando-data-frames-com-merge-e-concat-10e7d07ca5ec)
- E no código python, tem comentários sobre as outras funções sendo utilizadas

## 4º Aula: Análises Avançadas de Ações e Gráficos de Velas

- [Compilador](https://onecompiler.com) online para várias linguagens diferentes
- Nessa aula foi explicado como criar uma gráfico usando a biblioteca Matplotlib, com os dados da API da bibiloteca yfinance
- [Código exemplo](/python/aula4.ipynb)
- O que são [tuplas](https://chat.openai.com/share/1614551f-f197-45f3-9cd8-2cbef1905d2d) em Python

## 5º Aula: Previsão de Séries Temporais de Ações e Carreiras no Mercado de Dados

- Nessa aula foi utilizado a biblioteca prophet (Prophet) para trabalhar com series temporais, que são conjunto de informações/observações avaliadas ao longo do tempo
- Foram abordados assuntos sobre maching learning, sendo estes artigos utilizados para aprofundar o assunto:  
    - [O que é Maching Learning?](https://www.alura.com.br/artigos/machine-learning?_gl=1*1uknx2h*_ga*MjU0MjA0MzAzLjE3MDQ4MTMzMjI.*_ga_1EPWSW3PCS*MTcxMTgwNjc0Ni40Mi4wLjE3MTE4MDY3NDYuMC4wLjA.*_fplc*aGNoJTJCQzRFQXQ3WTJOUTVFNzMlMkJpTzUyVzlaSGduJTJCRnlqJTJCczBWcjJwRzZKUjJGelFkNVBOeERZcHJVMzdzc21VRUhqdkpGM2IxcGJjTlRlbEx3MWlRS3M0djlGN1pUNFBYRkRNc0hMTFFTVDZPQ3JyZng1SVRFMUxQRWhDN2clM0QlM0Q.)
    - [Desmistificando termos em Machine Learning](https://www.alura.com.br/artigos/desmistificando-termos-machine-learning?_gl=1*u0q3zp*_ga*MjU0MjA0MzAzLjE3MDQ4MTMzMjI.*_ga_1EPWSW3PCS*MTcxMTgwNjc0Ni40Mi4xLjE3MTE4MDY4MjkuMC4wLjA.*_fplc*aGNoJTJCQzRFQXQ3WTJOUTVFNzMlMkJpTzUyVzlaSGduJTJCRnlqJTJCczBWcjJwRzZKUjJGelFkNVBOeERZcHJVMzdzc21VRUhqdkpGM2IxcGJjTlRlbEx3MWlRS3M0djlGN1pUNFBYRkRNc0hMTFFTVDZPQ3JyZng1SVRFMUxQRWhDN2clM0QlM0Q.)
    - [Os 4 tipos de aprendizagem na IA](https://www.alura.com.br/artigos/quais-sao-tipos-aprendizagem-ia-inteligencia-artificial?_gl=1*1ykiyy*_ga*MjU0MjA0MzAzLjE3MDQ4MTMzMjI.*_ga_1EPWSW3PCS*MTcxMTgwNjc0Ni40Mi4xLjE3MTE4MDY4MzcuMC4wLjA.*_fplc*aGNoJTJCQzRFQXQ3WTJOUTVFNzMlMkJpTzUyVzlaSGduJTJCRnlqJTJCczBWcjJwRzZKUjJGelFkNVBOeERZcHJVMzdzc21VRUhqdkpGM2IxcGJjTlRlbEx3MWlRS3M0djlGN1pUNFBYRkRNc0hMTFFTVDZPQ3JyZng1SVRFMUxQRWhDN2clM0QlM0Q.)