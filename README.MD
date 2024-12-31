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

## Passo a Passo para Execução

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
