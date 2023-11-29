# Natural Language Processing (NLP)

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

## NLP Neural

Aprendem com os dados e podem começar do zero para a construção do modelo, obtendo informações relevantes dos dados invés de usar regras e modelos feitos outrora

Uma rede neural é composta de regras matemáticas que são baseadas na informação que é armazenada em sua memória, por isso precisam de MUITOS dados (não dá pra fazer em casa pois precisa de um hardware poderoso e de poder de processamento)

A partir do momento que os textos passaram a ser convertidos para vetores, houve a mudança de tudo que conhecemos. A partir de 2010 a mudança de performance nos resultados foi gigantesca

Deverá ser usado o que resolve melhor o case do projeto, com custo-benefício e computacional, investimento, tempo gasto, complexidade, etc

"Não se faz um chatgpt com uma matriz de coocorrência"
