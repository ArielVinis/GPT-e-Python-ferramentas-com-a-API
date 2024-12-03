# OpenAI: GPT e Python: criando ferramentas com a API

Para isso, foi usado a biblioteca da openai:

    pip install openai python-dotenv pydub instabot Pillow

## 01. Playground e a API da OpenAI

* Ajustar os parâmetros do PlayGround como temperatura e comprimento máximo para controlar a criatividade e a saída do GPT, visando gerar respostas mais coerentes e adaptadas aos contextos desejados.

* Criar assistentes e threads no PlayGround para que seja possível ter ações personalizadas para criar respostas ao usuário.

* Utilizar a biblioteca da OpenAI para fazer requisições à API e gerar respostas de um modelo GPT-4, aprendendo a passar mensagens de sistema e usuário, assim como proteger a chave da API para garantir segurança.

* Esconder chaves de identificação em variáveis de ambiente para proteger informações sensíveis ao fazer integrações de API.

## 02. Prompt engineering e prompt template

* Aprendemos sobre um categorizador de produtos e ajustamos os parâmetros do GPT para obter diversas respostas para nossas solicitações.

* Exploramos também a documentação da API enquanto trabalhamos com os conceitos de prompt engineering e prompt template.

## 03. Custos, modelos e contagem de tokens

* Selecionar o modelo de linguagem adequado para nossas tarefas, considerando os limites de tokens, contexto e custo e escolhendo com base nas necessidades específicas do projeto.

* Utilizar a biblioteca TikToken para contar e estimar a quantidade de tokens em um texto para avaliar o uso de modelos de linguagem, entender a estrutura interna dos tokens e calcular custos de processamento.

* Escolher dinamicamente modelos de linguagem com base no número de tokens da entrada e a calcular o tamanho esperado da saída para garantir o funcionamento adequado da geração de texto.

## 04. Batch e controle de erros

* Usar modelos de linguagem para realizar análise de sentimentos em avaliações de produtos, resumindo as avaliações, determinando o sentimento geral (positivo, neutro ou negativo), identificando pontos fortes e pontos fracos e salvando os resultados em arquivos.

* Refatorar o código para processar análises de sentimentos em lotes, utilizando uma função para realizar a análise para cada produto da lista, e adicionar prints para acompanhar o progresso e identificar possíveis erros durante a análise em lote.

* Lidar com exceções ao realizar chamadas em lote para uma API utilizando blocos de código try e except para capturar e tratar diferentes tipos de erros.

* Implementar uma lógica de retentativa, na qual tentamos novamente a chamada após um curto intervalo de tempo em caso de erro, para lidar com problemas temporários.

* Lidar com os limites de taxa na utilização da API GPT, que são definidos pela quantidade de requisições por dia (RPD), requisições por minuto (RPM) e quantidade de tokens por minuto (TPM).

## 05. Praticando análise de fraudes

* Transformar o resultado da chamada do GPT em um objeto JSON estruturado, permitindo a iteração por cada transação, identificando justificativas para detectar uma fraude e construindo recomendações.

* Carregar uma lista de transações a partir de um arquivo de texto, criar uma função para analisar transações e formatar a saída das recomendações de forma legível.

## Conclusão

* Durante as aulas, aprendemos sobre como utilizar a API, abordando os principais conceitos e estruturas do seu uso. Aprendemos também a trabalhar com engenharia de prompts (solicitações), para criar solicitações cada vez mais sofisticadas, e a definir um conjunto de templates para as interações com a IA generativa.

* Nos dedicamos a utilizar um volume de tokens adequado para poder escolher um modelo mais assertivo para cada tipo de problema. Dessa forma, variamos entre os modelos da API utilizando o GPT 3.5, GPT 4 e também outras variações como o GPT 3.5 Turbo.

* Trabalhamos com o processamento de lotes, isto é, receber muitas informações e trabalhar com essas informações em cadeia. Isso garante que uma resposta gerada pela OpenAI possa alimentar outra pergunta para a IA generativa.

Ainda, aprendemos a agrupar todos esses conhecimentos em um projeto, que foi este projeto de verificação de fraude financeira.
