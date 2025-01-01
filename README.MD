# Mega-Sena: Análise Estatística e Simulação com Python

Este projeto é um exercício didático que combina conceitos de **matemática** (probabilidade, estatística, dispersão) com **programação em Python**. Ele utiliza dados reais da Mega-Sena para realizar análises estatísticas e criar simulações de apostas baseadas em diferentes estratégias.

## Funcionalidades do Projeto

- **Download de Dados Históricos**: Utiliza a biblioteca `requests` para baixar dados históricos diretamente do site [As Loterias](https://asloterias.com.br/download-todos-resultados-mega-sena).
- **Análise Estatística**: Frequência dos números sorteados, dispersão estatística entre os números mais e menos sorteados.
- **Simulação de Apostas**: Geração de jogos com combinações aleatórias e baseados nos números mais sorteados.
- **Exploração de Dados**: Manipulação de dados usando `pandas` e `numpy`.

---

## Objetivos

1. Baixar e processar dados históricos da Mega-Sena.
2. Realizar análises estatísticas para entender padrões e frequência de números sorteados.
3. Simular estratégias de apostas com base em dados históricos.
4. Fornecer um exemplo prático de uso de Python para resolver problemas do mundo real.

---

# Disclaimer: Exercício de Probabilidade e Frequência de Sorteio

Este exercício tem como objetivo demonstrar **como calcular a probabilidade e analisar a frequência dos números sorteados** na Mega-Sena utilizando conceitos matemáticos e estatísticos. A ideia central é ensinar como realizar cálculos de probabilidade, identificar padrões históricos e compreender a distribuição de números em eventos passados.

## Importante:
- **Este exercício não implica em prever os resultados do próximo sorteio da Mega-Sena.**
- A Mega-Sena é um sistema de sorteio **aleatório**, no qual cada número tem **igual probabilidade de ser sorteado** em cada rodada.
- O histórico de números sorteados não influencia os resultados futuros, pois cada sorteio é independente e não sofre interferência de eventos anteriores.

## Por que não é possível prever os próximos resultados?
De acordo com a **teoria das probabilidades** e a dinâmica dos sorteios:
- A Mega-Sena utiliza métodos calibrados para garantir que os números sejam sorteados de maneira totalmente aleatória.
- Não existem fatores conhecidos que possam alterar a probabilidade de um número ser sorteado em relação a outro.
- Qualquer padrão percebido nos resultados anteriores é meramente coincidência ou fruto da interpretação humana (viés de padrão).

## Finalidade do Exercício
O foco deste exercício é:
1. **Ensinar o conceito de probabilidade e frequências estatísticas.**
2. Analisar eventos passados como forma de explorar a matemática envolvida.
3. Fornecer uma ferramenta educacional para aprender a trabalhar com dados, simulações e probabilidades.

Por isso, use este exercício como um aprendizado matemático e estatístico e lembre-se de que **não existem garantias de vitória em jogos de azar como a Mega-Sena**. Jogue com responsabilidade!

Um site que explica esses conceitos mais detalhadamemte é o [sci-culture](ttp://m.sci-culture.com/br). O  artigo [Mega Sena: Um estudo de Probabilidades e Análise Combinatória](http://m.sci-culture.com/br/matematica/combinatoria-probabilidades/combinacoes-probabilidades-megasena.html) ilustra esses comceitos.

O site oficial da Caixa tambem fornece informações historicas sobre os sorteios, a metodologia e sobre a metodologia probalistica. Acesse aqui a sessão sobre [Probalidade](https://loterias.caixa.gov.br/Paginas/Mega-Sena.aspx)

---

## Requisitos do Ambiente

Certifique-se de ter instalados:

- **Python 3.8+**
- **Visual Studio Code** (recomendado) com extensões de suporte ao Python.
- **Jupyter Notebook** (opcional, para exploração interativa).

## Passo a Passo da Execução

### 1. Download dos Dados

Os dados históricos podem ser baixados automaticamente através do script usando a biblioteca `requests`. O script faz um POST para o site [As Loterias](https://asloterias.com.br/download-todos-resultados-mega-sena), salvando o arquivo `mega_sena_dados_brutos.xlsx`.

---

### 2. Limpeza e Preparação dos Dados

Os dados brutos são processados para remover linhas não numéricas, ajustar colunas e renomear cabeçalhos. Aqui é utilizada a biblioteca `pandas` para transformar os dados em um formato adequado para análise.

---

### 3. Análises Estatísticas

#### **Frequência dos Números Sorteados**
- Contagem de quantas vezes cada número foi sorteado.
- Ordenação por frequência decrescente.

#### **Dispersão**
- Comparação entre os números mais sorteados, menos sorteados e medianos.
- Avaliação da relevância estatística dos números.

---

### 4. Simulação de Apostas

O projeto inclui uma função para gerar apostas baseadas nos números mais sorteados. Também é possível ajustar parâmetros como o número de jogos, quantidade de números por jogo e o ranking dos números selecionados.

---

# Mega-Sena: Análise Estatística e Simulação com Python

Este projeto é um exercício didático que combina conceitos de **matemática** (probabilidade, estatística, dispersão) com **programação em Python**. Ele utiliza dados reais da Mega-Sena para realizar análises estatísticas e criar simulações de apostas baseadas em diferentes estratégias.

## Funcionalidades do Projeto

- **Download de Dados Históricos**: Utiliza a biblioteca `requests` para baixar dados históricos diretamente do site [As Loterias](https://asloterias.com.br/download-todos-resultados-mega-sena).
- **Análise Estatística**: Frequência dos números sorteados, dispersão estatística entre os números mais e menos sorteados.
- **Simulação de Apostas**: Geração de jogos com combinações aleatórias e baseados nos números mais sorteados.
- **Exploração de Dados**: Manipulação de dados usando `pandas` e `numpy`.

---

## Objetivos

1. Baixar e processar dados históricos da Mega-Sena.
2. Realizar análises estatísticas para entender padrões e frequência de números sorteados.
3. Simular estratégias de apostas com base em dados históricos.
4. Fornecer um exemplo prático de uso de Python para resolver problemas do mundo real.

---

## Requisitos do Ambiente

Certifique-se de ter instalados:

- **Python 3.8+**
- **Visual Studio Code** (recomendado) com extensões de suporte ao Python.
- **Jupyter Notebook** (opcional, para exploração interativa).

### Bibliotecas Necessárias

Instale as dependências com o seguinte comando:

```bash
pip install pandas numpy requests jupyter openpyxl
```

---

## Passo a Passo para Execução

### 1. Download dos Dados

Os dados históricos podem ser baixados automaticamente através do script usando a biblioteca `requests`. O script faz um POST para o site [As Loterias](https://asloterias.com.br/download-todos-resultados-mega-sena), salvando o arquivo `mega_sena_dados_brutos.xlsx`.

```python
import requests

url = "https://asloterias.com.br/download_excel.php"
output_file = "mega_sena_dados_brutos.xlsx"

response = requests.post(url)
with open(output_file, "wb") as file:
    file.write(response.content)

print(f"Arquivo salvo como: {output_file}")
```

---

### 2. Limpeza e Preparação dos Dados

Os dados brutos são processados para remover linhas não numéricas, ajustar colunas e renomear cabeçalhos. Aqui é utilizada a biblioteca `pandas` para transformar os dados em um formato adequado para análise.

---

### 3. Análises Estatísticas

#### **Frequência dos Números Sorteados**
- Contagem de quantas vezes cada número foi sorteado.
- Ordenação por frequência decrescente.

#### **Dispersão**
- Comparação entre os números mais sorteados, menos sorteados e medianos.
- Avaliação da relevância estatística dos números.

---

### 4. Simulação de Apostas

O projeto inclui uma função para gerar apostas baseadas nos números mais sorteados. Também é possível ajustar parâmetros como o número de jogos, quantidade de números por jogo e o ranking dos números selecionados.

---

## Como Rodar o Projeto com o Notebook

### Executando no Visual Studio Code

1. Certifique-se de que o **Python** e a extensão **Jupyter** estão instalados no VS Code.
   - Instale a extensão **Jupyter** diretamente no marketplace do VS Code.

2. Abra o arquivo `mega_sena_analysis.ipynb` no VS Code.

3. Clique em qualquer célula do notebook e selecione o kernel Python apropriado (versão 3.8 ou superior).

4. Execute as células sequencialmente clicando no botão de execução (▶) no topo de cada célula ou pressione `Shift + Enter`.

5. Siga as instruções no notebook para explorar os dados, realizar análises estatísticas e simular apostas.

### Executando no Google Colab

1. Faça login na sua conta do Google e acesse [Google Colab](https://colab.research.google.com/).

2. Faça upload do arquivo `mega_sena_analysis.ipynb` clicando em **File > Upload Notebook**.

3. Certifique-se de que as bibliotecas necessárias estão instaladas. Adicione uma célula no início do notebook com o seguinte comando e execute:

   ```python
   !pip install pandas numpy requests openpyxl
   ```

4. Execute as células do notebook sequencialmente clicando no botão de execução (▶) ao lado de cada célula.

5. Explore os dados e simulações de forma interativa, direto na nuvem!

---

## Próximos Passos

### Melhorias Sugeridas

1. **Adicionar suporte para diferentes tipos de jogos** (7, 8, 10 números).
2. **Simulação baseada em orçamento disponível**: sugerir apostas dentro de um limite financeiro.
3. **Estratégias combinadas**: criar simulações que misturem jogos simples, bolões e jogos de maior custo.

---

### Prompt Utilizado

Parte desse programa foi criado com o auxilio da IA, mais especificamente com o ChatGPT, modelo 4o. 

Da mesma forma que acredito que um dia todos usarão dados como usam o Excel, também acredito que a IA veio para ficar e ser um ótimo apoio para diversas áreas do conhecimento.

Caso queira consultar o prompt que originou este projeto, acesse o link abaixo:

[Prompt do ChatGPT](https://chatgpt.com/share/67744d1c-aa04-800d-b3d6-78db66bcf867)

---

## Notas Finais

Este projeto foi desenvolvido como uma ferramenta educacional para demonstrar como Python pode ser usado para análise de dados reais. Ele também explora como **Inteligência Artificial** pode ser integrada em processos analíticos para complementar a capacidade humana.

Se este projeto foi útil para você, deixe sua opinião ou compartilhe com outros entusiastas da área. Caso queira agradecer, pode me pagar um café! Meu PIX está no QR Code no repositório.

![QR Code Cafezinho Algo Megasena](qr_code_pix_bradesco.png)


---

### Autor

**Flavio Lopes**  
Disseminando conhecimento prático em dados para a tomada de decisão.

---

### Contato

Dúvidas, sugestões ou melhorias? Entre em contato ou contribua diretamente no repositório.

- **GitHub**: [dadosnapratica](https://github.com/orgs/dadosnapratica)
- **LinkedIn**: [Flavio Lopes](https://www.linkedin.com/in/flavionlopes/)
- **E-mail**: [flavio.lopes@ideiasfactory.tech](mailto:flavio.lopes@ideiasfactory.tech)
- **WhatsApp**: [+55 11 99635-4436](https://wa.me/5511996354436)
- **Instagram**: [@dadosnapratica](https://www.instagram.com/dadosnapratica/)

**Fique bem e continue aprendendo!**
