
# Projeto Integrador – Análise de Conteúdo e Contagem de Palavras

Este repositório contém cinco notebooks Jupyter, cada um implementando etapas do fluxo de coleta, limpeza, análise e exportação de dados textuais extraídos da web.

---

## Cópia_de_Garotas_Estupidas_2_FINAL.ipynb
1. **Web scraping**: navega e coleta artigos do site “Garotas Estúpidas” até determinado limite de caracteres.
2. **Limpeza de texto**: retira tags HTML, converte para minúsculas, remove pontuação e stopwords, aplicar tokenização básica.
3. **Contagem de frases/expressões**: define uma lista de frases-alvo e contabiliza quantas vezes cada expressão aparece em cada texto.
4. **Geração de nuvem de palavras**: produz nuvem de palavras com as palavras mais frequentes encontradas.
5. **Exportação para Excel**: salva tabelas de frequências e resultados em planilha `.xlsx`.

## PalavrasPréSelecionadas_Fragântica.ipynb
1. **Coleta de URLs**: acessa a página de lançamentos de perfumes no Fragrantica Brasil e extrai links para cada review.
2. **Extração de reviews**: para cada URL, coleta título do perfume, autor, data e texto completo da avaliação.
3. **Contagem de palavras-chave**: a partir de uma lista pré-selecionada de termos, computa ocorrências em cada review.
4. **Visualização leve**: plota nuvem de palavras e exibe tabelas de contagem interativas.
5. **Construção de DataFrame final**: consolida todas as informações em um único `pandas.DataFrame`.

## Perfumes_Importados_Fragántica.ipynb
1. **Importação de dados**: lê arquivo CSV/Excel contendo reviews de perfumes importados.
2. **Normalização de texto**: remove acentos, converte a minúsculas, aplica expressões regulares para limpar caracteres indesejados.
3. **Filtro de termos irrelevantes**: remove stopwords customizadas e palavras de pouco valor analítico.
4. **Contagem de frequência**: calcula a frequência de cada termo relevante na base de reviews.
5. **Gráficos de frequência**: gera gráficos de barras para as palavras mais frequentes.

## Still_the_Look.ipynb
1. **Configuração do pipeline**: importa funções de scraping, limpeza e contagem dos notebooks anteriores.
2. **Fluxo orquestrado**:
   - Executa scraping de artigos ou reviews.
   - Aplica limpeza em batch nos textos coletados.
   - Realiza contagem de termos específicos.
   - Gera nuvens de palavras.
3. **Exportação unificada**: consolida e salva todos os resultados em formatos estruturados.

## TransformandoExcel.ipynb
1. **Leitura de planilha Excel**: carrega dados em `pandas.DataFrame`.
2. **Transformação de dados**: renomeia colunas, filtra linhas, calcula novas colunas conforme regras simples.
3. **Gravação em Excel**: salva o DataFrame transformado em um novo arquivo `.xlsx`.

---

## Como Executar
1. Clone o repositório:
   ```bash
   git clone https://github.com/SEU_USUARIO/seu-repo.git
   cd seu-repo
````

2. Instale dependências necessárias (por notebook):

   ```bash
   pip install pandas nltk matplotlib openpyxl cloudscraper beautifulsoup4 requests pyspark wordcloud unidecode
   ```
3. Abra o Jupyter Lab ou Notebook e execute os notebooks conforme a ordem acima.

```
```
