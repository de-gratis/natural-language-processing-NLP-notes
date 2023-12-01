# Natural Language Processing (NLP)

Uma sub-área da Inteligência Artificial conhecida por processar o texto e a voz

Compreender um texto em NLP significa um conjunto de ações: entender, interpretar e manipular a linguagem humana

Seu processo para esta compreensão se dá por um processo automatizado para reconhecer padrões em texto, recebendo dados e criando um modelo para estes dados, permitindo futuras previsões

Análise Sintática (estrutura de uma frase) e Análise Semântica (compreensão do significado de palavras e frases)

Entender o contexto de uma frase, bem como as relações entre as palavras e frases, devendo ser capaz de lidar com ambiguidade e uma grande quantidade de dados

"Uma era de pré e pós os modelos de linguagem"

![image-20231128223257049](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231128223257049.png)

![image-20231128224523210](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231128224523210.png)

Os clientes precisam do tipo de inteligência do chatgpt (geral) só que para os seus dados (privado), não disponíveis na web

O problema não é o chatgpt, mas para qual dado ele está apontando, o seu modelo de linguagem

Efeito caixa preta, se você não entende o que está acontecendo dentro da API, e você não gostou do so seu  retorno, não há nada a ser feito. Caso saiba, pode-se mudar seu input, e aplicar várias técnicas

As 3 eras da NLP: 

- Simbólica (1950-1980): Basicamente uma junção de if's e else's 
- Estatística (1980-2010): Separar seu texto em palavras (bag of words). Tem o problema das palavras que aparecem muito mas não significam nada (stop words)
- Neural (2010-Presente): NLP clássico e NLP baseado em Deep-Learning, ambos com vários tipos de processos

![image-20231129003833880](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231129003833880.png)

## Estatística 

No método bag of words, é possível inferir quais palavras fazem parte de um mesmo contexto pois as mesmas aparecerão juntas com mais frequência

Pode reconhecer o caminho que o texto está seguindo, e não precisamente sobre o quê o texto está falando



## NLP Neural

Aprendem com os dados e podem começar do zero para a construção do modelo, obtendo informações relevantes dos dados invés de usar regras e modelos feitos outrora

Uma rede neural é composta de regras matemáticas que são baseadas na informação que é armazenada em sua memória, por isso precisam de MUITOS dados (não dá pra fazer em casa pois precisa de um hardware poderoso e de poder de processamento)

A partir do momento que os textos passaram a ser convertidos para vetores, houve a mudança de tudo que conhecemos. A partir de 2010 a mudança de performance nos resultados foi gigantesca

Deverá ser usado o que resolve melhor o case do projeto, com custo-benefício e computacional, investimento, tempo gasto, complexidade, etc

"Não se faz um chatgpt com uma matriz de coocorrência"



Com Machine Learning, pega-se os campos categóricos, os textuais e os converte para numérico

Não terá uma representação um para um de cada palavra para cada número, pois no começo pode até ser assim, mas conforme o modelo vai processando, mais informações vão surgindo com números explicando tais relações, por normalização, para explicar contextos

Machine Learning leva em conta os tamanhos dos números, trazendo vieses que não queremos, devendo tomar cuidado com estas tomadas de decisão

Inclui-se a normalização entre 0 e 1 para que a diferença reconhecida pelo modelo não seja tão significativa

Valores de múltiplas dimensões em um espaço vetorial, Result Embedding, Sentence Transforming

Não se olha para o significado das palavras, e sim para uma representação vetorial dos textos para que seja possível calcular a distância dos outros pontos do vetor. Não se entende a língua, entende-se a distância entre a semântica das palavras

Há diferentes tipos de similaridades, como de contexto, tempo verbal, significado, mas sempre sobre sintática ou semântica

![image-20231201030434549](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231201030434549.png)





No Collab, é recomendado mudar o ambiente de execução para GPU e checar a mesma com `!nvidia-smi`

A tokenização é o processo de dividir a frase, podendo ser palavra por palavra, ou dividir por subpalavras ( como "learn ...ing, ...ed", sendo o "ing" e o "ed" comum para outras palavras), quebrando ainda mais os tokens

A importância de limpar as stopwords para não poluir o modelo:

![image-20231201042703840](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231201042703840.png)

Stemmimg: transformar a palavra para o seu radical

![image-20231201042937786](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231201042937786.png)

As palavras da esquerda teoricamente não significam a mesma coisa, mas a da direita sim



Lemmatization: mesmo do Stemming, mas puxa para o verbo mais próximo

![image-20231201043153685](C:\Users\Home\AppData\Roaming\Typora\typora-user-images\image-20231201043153685.png)

Normalização Unicode: normalizar os dados para "corrigir"caracteres especiais, palavras como café, por causa do acento



POS Tagging: Part of Speech, entende o que é um pronome, verbo, substantivo, etc

Ner: Named Entity Recognition, reconhece-se no texto o que é reconhecido como uma pessoa, organização, data, etc por meio das relações das palavras



As palavras que tem um significado parecido elas começam a criar clusters no espaço vetorial, se clusterizando

É possível instanciar um modelo de ML localmente em sua própria máquina

Sempre que você tokenizar usando um modelo específico, ele sempre terá um número x de caracteres para representar o encode daquele modelo, completando com paddings quando não tiver palavras suficientes



Redact: limpar informações críticas como e-mail, cpf, etc
