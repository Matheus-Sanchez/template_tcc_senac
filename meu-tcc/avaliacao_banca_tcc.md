---
title: "Avaliação simulada de banca acadêmica - TCC"
subtitle: "Classificação de câncer de mama em mamografias: estudo comparativo entre CNNs clássicas e híbridas quântico-clássicas"
author: "Simulação de banca acadêmica"
date: "2026"
lang: pt-BR
geometry: margin=2.5cm
fontsize: 11pt
mainfont: DejaVu Serif
---

# Observação inicial

Este documento reúne a simulação de uma banca acadêmica composta por sete avaliadores, considerando apenas a parte apresentada do trabalho: **Introdução, Contexto, Justificativa, Objetivos, Hipótese e Delimitações**.

A avaliação foi organizada em rodadas individuais, com foco na melhoria acadêmica e metodológica do TCC. Ao final, há um parecer consolidado da banca.

A banca simulada foi composta por:

1. Professor especialista em Inteligência Artificial;
2. Professor especialista em Ciência da Computação;
3. Professor entusiasta em tecnologia e inovação;
4. Professor especialista em Computação Quântica;
5. Professor especialista em Física Quântica;
6. Professor especialista em Pesquisa Científica;
7. Professor especialista em Matemática Avançada.

---

# Rodada 1 - Professor especialista em Inteligência Artificial

## Avaliação individual

Como avaliador da área de Inteligência Artificial, considero que a proposta tem um recorte relevante e tecnicamente promissor: comparar uma CNN clássica com uma arquitetura híbrida quântico-clássica na classificação de mamografias. O texto já demonstra consciência de que o objetivo não deve ser "provar superioridade quântica", mas investigar desempenho, estabilidade, custo computacional e viabilidade prática em um ambiente controlado. Esse é um ponto forte importante, porque evita uma promessa excessiva sobre computação quântica.

## 1. Clareza do problema de pesquisa

O problema aparece de forma compreensível, mas ainda pode ser formulado com mais precisão. A introdução afirma que a pesquisa busca comparar uma arquitetura clássica baseada em CNN com uma arquitetura híbrida quântico-clássica aplicada à classificação de mamografias digitais, considerando desempenho preditivo, estabilidade, custo computacional e viabilidade prática.

Isso é adequado, mas falta explicitar melhor **qual é exatamente o problema científico central**. Hoje, o texto apresenta três problemas ao mesmo tempo:

1. a classificação de mamografias;
2. as limitações das CNNs clássicas;
3. a incerteza sobre a utilidade prática de modelos híbridos quântico-clássicos.

Esses três pontos são pertinentes, mas a banca pode perguntar: **o problema principal é melhorar a classificação de câncer de mama ou avaliar a viabilidade de modelos híbridos em comparação com CNNs?**

Minha recomendação é deixar claro que o núcleo do TCC não é propor um sistema clínico, nem necessariamente alcançar o maior desempenho possível, mas **avaliar experimentalmente se a inserção de um componente quântico simulado agrega algo mensurável em relação a uma CNN clássica sob o mesmo protocolo**.

## 2. Relevância do tema

A relevância social está bem construída. O texto justifica o câncer de mama como tema de impacto em saúde pública e conecta a mamografia à detecção precoce. Também é positivo o cuidado ao declarar que o trabalho **não possui objetivo de uso clínico imediato**, mas se insere em uma linha de pesquisa com potencial impacto na saúde.

Do ponto de vista de IA, a relevância acadêmica também é defensável. A justificativa afirma que o aprendizado profundo já é central em visão computacional, enquanto modelos híbridos quântico-clássicos ainda carecem de validação comparativa rigorosa, especialmente em aplicações médicas.

Esse argumento é bom, mas precisa ser reforçado com uma distinção mais clara entre:

- **aplicação de IA em saúde**, que já é amplamente estudada;
- **comparação metodológica entre IA clássica e IA híbrida quântico-clássica**, que é o diferencial real do trabalho.

Sem essa separação, há risco de o trabalho parecer apenas "mais um classificador de mamografia".

## 3. Qualidade da fundamentação teórica na parte avaliada

Considerando apenas Introdução, Contexto, Justificativa, Objetivos, Hipótese e Delimitações, a fundamentação inicial é adequada, mas ainda generalista em alguns pontos.

O texto acerta ao citar desafios como generalização, desbalanceamento de dados, custo computacional e confiabilidade em imagens médicas. Também acerta ao mencionar que aplicações híbridas quântico-clássicas em imagens médicas de alta dimensão ainda são exploratórias.

Porém, como professor de IA, eu esperaria uma formulação mais objetiva sobre **quais limitações das CNNs motivam a comparação**. Por exemplo:

- overfitting em bases médicas;
- dependência de grandes volumes de dados;
- sensibilidade a desbalanceamento;
- dificuldade de generalização entre bases;
- custo de processar imagens de alta resolução;
- necessidade de interpretabilidade em contexto médico.

O texto cita esses elementos, mas ainda de modo disperso. O ideal seria transformar isso em uma cadeia argumentativa:

> CNNs são fortes em extração espacial, mas enfrentam limitações X, Y e Z em mamografias. Modelos híbridos quântico-clássicos são investigados como alternativa experimental, mas ainda não há evidência suficiente de benefício prático. Portanto, este trabalho compara as duas abordagens sob protocolo controlado.

## 4. Coerência entre introdução, objetivos, hipótese e limitações

Há boa coerência geral. O objetivo geral declara a intenção de investigar comparativamente CNNs clássicas e modelos híbridos quântico-clássicos na classificação de câncer de mama, considerando desempenho, custo computacional, estabilidade e viabilidade prática.

Os objetivos específicos também estão alinhados, especialmente ao prever:

- definição da base e classes;
- protocolo de pré-processamento, divisão, treino, validação e teste;
- CNN clássica como referência;
- arquitetura híbrida compatível com limitações de simulação;
- análise de número de qubits, feature map, profundidade e codificação;
- comparação por métricas como acurácia, precisão, recall, F1-score, AUC e matriz de confusão;
- avaliação de tempo, memória, estabilidade e escalabilidade.

A hipótese é um dos pontos mais fortes da parte apresentada. Ela é cuidadosa ao afirmar que a arquitetura híbrida **pode apresentar desempenho competitivo**, mas que não se pressupõe superioridade geral da abordagem quântica. O texto também reconhece limitações como custo computacional, número reduzido de qubits, sensibilidade a hiperparâmetros, codificação de dados e restrições NISQ.

A fragilidade principal está nas delimitações. Elas delimitam a tarefa como classificação supervisionada em três classes - normal, benigno e maligno - e comparam CNN clássica e modelo híbrido mantendo constantes base, pré-processamento, divisão e métricas. Isso é bom, mas ainda falta delimitar melhor:

- se a divisão será por imagem, exame ou paciente;
- se haverá validação externa ou apenas teste interno;
- se o modelo usará imagem inteira, ROI ou patches;
- se as imagens serão analisadas por mama, por exame ou por imagem individual;
- qual será o critério mínimo para considerar o modelo híbrido "competitivo".

## 5. Viabilidade técnica e metodológica

A proposta é viável para TCC, mas com risco técnico elevado. O risco não está na CNN clássica; está no componente híbrido quântico-clássico.

A escolha de manter o modelo quântico como **simulado** e compatível com limitações de simulação é correta. O problema é que, se a metodologia não for muito bem controlada, a comparação pode ficar injusta. Uma CNN clássica pode ser muito mais expressiva e eficiente que um pequeno circuito variacional. Então a banca pode questionar se o modelo híbrido está sendo comparado em igualdade real ou apenas "encaixado" artificialmente depois de uma CNN.

Um ponto metodológico importante: a proposta precisa declarar com mais precisão **qual será a unidade de comparação**. Comparar apenas acurácia pode ser frágil. Para IA médica, a avaliação deve priorizar também recall da classe maligna, AUC por classe, matriz de confusão e análise de falsos negativos. O texto já menciona AUC, recall e matriz de confusão, mas ainda pode hierarquizar essas métricas: nem todas têm o mesmo peso em diagnóstico médico.

## 6. Pontos fortes do texto

Os principais pontos fortes são:

- **Tema relevante e interdisciplinar**, envolvendo IA, saúde, visão computacional e computação quântica.
- **Postura científica cautelosa**, sem prometer vantagem quântica definitiva.
- **Objetivo geral bem alinhado à hipótese**.
- **Objetivos específicos bem operacionalizados**, especialmente ao incluir métricas, custo computacional, estabilidade e escalabilidade.
- **Reconhecimento explícito das limitações de simulação e NISQ**, o que fortalece a honestidade metodológica.
- **Boa justificativa acadêmica**, ao apontar falta de validação comparativa rigorosa de modelos híbridos em aplicações médicas.

## 7. Fragilidades, lacunas ou ambiguidades

As fragilidades principais são:

1. **Pergunta de pesquisa pouco visível**  
   O texto diz que o capítulo apresenta a pergunta de pesquisa, mas na parte observada ela não aparece de forma destacada. Recomendo inserir uma pergunta explícita, por exemplo:

   > Em uma tarefa controlada de classificação de mamografias, uma arquitetura híbrida quântico-clássica apresenta desempenho competitivo, estabilidade e custo computacional justificáveis em comparação com uma CNN clássica?

2. **Critério de competitividade indefinido**  
   "Desempenho competitivo" precisa ser mensurável. Competitivo significa diferença menor que 5% em AUC? Melhor recall para maligno? Menor custo computacional? Maior estabilidade? Sem isso, a conclusão pode ficar subjetiva.

3. **Risco de escopo excessivo**  
   O objetivo geral menciona "possibilidade de ampliação para uma classificação mais detalhada". Para TCC1, isso pode ser visto como abertura excessiva. Melhor deixar essa ampliação como trabalho futuro, não como parte do objetivo central.

4. **Falta de explicitação sobre leakage**  
   Em mamografia, vazamento de dados por paciente é um risco crítico. Se imagens da mesma paciente aparecem em treino e teste, os resultados podem ser artificialmente altos. Isso precisa aparecer já nas delimitações ou no protocolo.

5. **Pouca definição da arquitetura híbrida na introdução**  
   A banca pode querer saber se o circuito quântico entra após a extração de atributos da CNN, se substitui uma camada densa, se atua como classificador variacional ou como camada intermediária.

## 8. Sugestões concretas de melhoria

Eu recomendaria os seguintes ajustes antes da próxima versão:

- Inserir uma **pergunta de pesquisa explícita** após a justificativa.
- Definir "competitivo" por critérios mensuráveis: AUC, recall da classe maligna, F1 macro, estabilidade entre execuções e custo computacional.
- Trocar "possibilidade de ampliação para classificação mais detalhada" por algo como "mantendo a ampliação de classes como possibilidade futura".
- Adicionar nas delimitações que o trabalho **não pretende gerar ferramenta diagnóstica clínica**.
- Declarar que a divisão dos dados deve evitar vazamento por paciente, quando a base permitir.
- Explicitar que a comparação deve usar o mesmo conjunto de treino, validação e teste para os dois modelos.
- Indicar qual métrica será principal. Minha sugestão seria **AUC macro/one-vs-rest e recall da classe maligna**, deixando acurácia como métrica secundária.
- Incluir uma frase deixando claro que o objetivo é avaliar **viabilidade experimental**, não superioridade tecnológica ampla.

## 9. Perguntas que uma banca real poderia fazer

1. O que exatamente significa "modelo híbrido competitivo" no seu trabalho?
2. Qual métrica será considerada principal para decidir se um modelo foi melhor que o outro?
3. Por que comparar com uma CNN própria e não com uma arquitetura consolidada, como ResNet, EfficientNet ou DenseNet?
4. Como você evitará vazamento de dados entre treino, validação e teste?
5. A divisão será por imagem, por exame ou por paciente?
6. A classe maligna terá peso especial na avaliação?
7. O componente quântico será realmente treinável ou apenas uma transformação fixa?
8. Como você vai separar ganho real do componente quântico de ganho causado pelas camadas clássicas?
9. O custo computacional do modelo híbrido será comparado de forma quantitativa?
10. O que faria você concluir que a abordagem híbrida é inviável?

## Parecer parcial do professor de Inteligência Artificial

A proposta é relevante, atual e adequada para um TCC experimental, desde que o aluno mantenha a postura crítica já indicada na hipótese. O texto tem boa direção, mas precisa transformar melhor a motivação em uma pergunta de pesquisa objetiva e operacional. O maior risco é metodológico: comparar modelos de naturezas muito diferentes sem critérios claros de equivalência, competitividade e controle experimental.

**Minha recomendação, nesta etapa, é aprovação da proposta com ajustes obrigatórios na formulação do problema, na definição da métrica principal, na delimitação do escopo e no controle de vazamento de dados.**

---

# Rodada 2 - Professor especialista em Ciência da Computação

## Avaliação individual

Como professor de Ciência da Computação, minha avaliação se concentra menos na promessa tecnológica da IA ou da computação quântica e mais na **estrutura computacional do problema**, na **viabilidade de implementação**, na **comparabilidade experimental**, na **reprodutibilidade** e no **controle metodológico**.

O trabalho tem uma proposta tecnicamente interessante: comparar CNNs clássicas e modelos híbridos quântico-clássicos na classificação de mamografias. A introdução deixa claro que a pesquisa pretende avaliar não apenas desempenho preditivo, mas também estabilidade, custo computacional e viabilidade prática em ambiente experimental controlado. Isso é positivo, porque mostra preocupação com engenharia experimental, não apenas com acurácia.

## 1. Clareza do problema de pesquisa

O problema está razoavelmente claro, mas ainda precisa ser formalizado de maneira mais computacional.

O texto afirma que o trabalho está na interseção entre visão computacional médica, aprendizado profundo e aprendizado de máquina quântico, propondo comparar CNNs clássicas e arquiteturas híbridas quântico-clássicas em mamografias. Essa formulação é adequada para contextualização, mas, do ponto de vista de Ciência da Computação, ainda falta transformar isso em um problema experimental mais preciso.

A banca pode querer ver algo como:

> Dado um conjunto de imagens mamográficas rotuladas em três classes, comparar uma CNN clássica e uma arquitetura híbrida quântico-clássica sob o mesmo protocolo de treino, validação e teste, avaliando desempenho preditivo, custo computacional, estabilidade e escalabilidade.

Essa formulação deixa mais claro:

- **entrada:** imagens de mamografia;
- **saída:** classe normal, benigna ou maligna;
- **métodos:** CNN clássica e modelo híbrido;
- **protocolo:** mesmo pré-processamento, mesma divisão e mesmas métricas;
- **critérios de comparação:** desempenho, custo, estabilidade e viabilidade.

Atualmente, esses elementos aparecem no texto, especialmente nos objetivos e na hipótese, mas poderiam ser reunidos em uma **pergunta de pesquisa formal**.

## 2. Relevância do tema para Ciência da Computação

O tema é relevante porque envolve problemas clássicos e atuais da área:

- classificação supervisionada;
- visão computacional;
- aprendizado profundo;
- processamento de imagens médicas;
- comparação entre arquiteturas;
- custo computacional;
- reprodutibilidade;
- limitação de hardware;
- integração entre computação clássica e computação quântica.

A justificativa é bem direcionada quando afirma que deep learning em mamografia apresenta desempenho promissor, mas ainda enfrenta limitações de reprodutibilidade e avaliação em condições realistas. Também é relevante o argumento de que modelos híbridos quântico-clássicos ainda dependem de cenários restritos, bases menores e simulação.

Esse ponto fortalece o trabalho como TCC de Ciência da Computação, porque a contribuição não precisa ser clínica; pode ser uma contribuição de **avaliação experimental de arquiteturas computacionais**.

Contudo, eu recomendaria que o texto deixasse mais explícito que o trabalho é uma pesquisa de **benchmarking experimental**, isto é, uma comparação controlada entre modelos. Isso ajudaria a banca a entender que o valor científico está no protocolo, na análise crítica e na reprodutibilidade.

## 3. Qualidade da fundamentação teórica na parte apresentada

A fundamentação inicial é satisfatória, mas ainda existe uma lacuna importante: a parte introdutória fala de CNNs, modelos híbridos e mamografias, mas ainda não explicita suficientemente **qual é o desafio computacional específico da tarefa**.

Do ponto de vista de Ciência da Computação, eu esperaria que a introdução antecipasse alguns problemas técnicos centrais:

| Problema computacional | Por que importa no TCC |
|---|---|
| Alta dimensionalidade das imagens | Mamografias podem ter resolução elevada e gerar alto custo de memória |
| Desbalanceamento de classes | Pode mascarar desempenho real se apenas acurácia for usada |
| Vazamento de dados | Pode invalidar resultados se imagens da mesma paciente caírem em treino e teste |
| Custo de simulação quântica | Pode limitar número de qubits, batch size e quantidade de experimentos |
| Comparação injusta entre modelos | Uma CNN pode ter muito mais parâmetros e capacidade que o circuito quântico |
| Reprodutibilidade | Sem seeds, versões de bibliotecas e protocolo fixo, o experimento fica frágil |

Alguns desses elementos já aparecem no texto, especialmente nos objetivos específicos, que mencionam protocolo padronizado de pré-processamento, divisão dos dados, treinamento, validação e teste, além de avaliação de tempo de treinamento, memória, estabilidade e escalabilidade. Porém, seria interessante trazê-los de forma mais explícita já na introdução ou na justificativa.

## 4. Coerência entre introdução, objetivos, hipótese e limitações

A coerência geral é boa.

O objetivo geral está alinhado com a proposta: investigar comparativamente CNNs clássicas e modelos híbridos quântico-clássicos, considerando desempenho preditivo, custo computacional, estabilidade experimental e viabilidade prática.

Os objetivos específicos são um ponto forte do texto. Eles indicam tarefas concretas:

- definir base e classes;
- preparar protocolo de pré-processamento, divisão, treinamento, validação e teste;
- aprimorar uma CNN clássica;
- projetar arquitetura híbrida compatível com limitações de simulação;
- investigar número de qubits, feature map, profundidade e codificação;
- comparar modelos com acurácia, precisão, recall, F1-score, AUC e matriz de confusão;
- avaliar tempo, memória, estabilidade e escalabilidade.

Essa lista é tecnicamente adequada.

A hipótese também é coerente, especialmente ao afirmar que a comparação será feita com mesma base de dados, critérios equivalentes de pré-processamento, divisão dos dados, métricas e ambiente computacional. Isso é um ponto muito positivo, pois indica preocupação com controle experimental.

A delimitação também contribui para a coerência ao definir a tarefa como classificação supervisionada em três classes - normal, benigno e maligno - e ao manter constantes base, pré-processamento, divisão e métricas.

A fragilidade é que a coerência ainda está em nível declarativo. O texto diz que haverá protocolo controlado, mas ainda não informa critérios técnicos essenciais, como:

- divisão por paciente ou por imagem;
- proporção treino/validação/teste;
- controle de aleatoriedade;
- número de execuções por modelo;
- critério de parada;
- critério de escolha do melhor checkpoint;
- tratamento de classes desbalanceadas;
- arquitetura mínima do baseline clássico;
- baseline clássico equivalente ao modelo híbrido.

Esses detalhes podem ficar para a metodologia, mas alguns deveriam ser antecipados nas delimitações.

## 5. Viabilidade técnica e metodológica

A proposta é viável, mas exige redução de escopo e controle rigoroso.

### Pontos viáveis

A CNN clássica é plenamente viável para TCC, especialmente se o aluno usar uma arquitetura própria ou uma arquitetura conhecida como baseline. A classificação em três classes também é viável, desde que o conjunto de dados seja bem organizado e a avaliação não dependa apenas de acurácia.

A arquitetura híbrida é viável como experimento exploratório, desde que o circuito quântico seja pequeno e a proposta não tente codificar diretamente imagens inteiras. O próprio texto reconhece que o modelo híbrido deve ser compatível com limitações de simulação.

### Pontos de risco

O risco maior é a **comparação entre modelos com capacidades muito diferentes**. Uma CNN clássica pode ter centenas de milhares ou milhões de parâmetros, enquanto o circuito quântico simulado pode ter poucos qubits e poucos parâmetros. Se a CNN vencer, isso não necessariamente invalida o modelo híbrido; se o híbrido vencer, também será necessário provar que o ganho não veio apenas da parte clássica.

Por isso, o trabalho precisa de pelo menos três comparações:

| Modelo | Função no experimento |
|---|---|
| CNN clássica completa | baseline principal |
| CNN com gargalo clássico equivalente | controle para comparar com o modelo híbrido |
| CNN + camada quântica | modelo híbrido proposto |

Sem esse baseline intermediário, a banca pode perguntar:

> Como você sabe que o ganho ou perda veio do circuito quântico e não apenas da redução dimensional ou da camada densa final?

Essa é uma pergunta muito provável em uma banca de Ciência da Computação.

## 6. Pontos fortes do texto

Os pontos fortes, pela perspectiva de Ciência da Computação, são:

1. **Objetivos específicos operacionalizáveis**  
   A lista de objetivos já aponta ações computacionais concretas: definir base, preparar protocolo, treinar modelos, comparar métricas e avaliar custo computacional.

2. **Preocupação com reprodutibilidade**  
   O texto menciona comparação controlada, mesma base, mesmo pré-processamento, mesma divisão e mesmo ambiente computacional. Isso é essencial para um estudo comparativo.

3. **Boa consciência de limitações de hardware e simulação**  
   O trabalho não trata o modelo quântico como solução mágica. Reconhece limitações de qubits, simulação, hiperparâmetros e codificação.

4. **Avaliação além da acurácia**  
   O texto propõe precisão, recall, F1-score, AUC e matriz de confusão, além de tempo, memória, estabilidade e escalabilidade.

5. **Delimitação inicial em três classes**  
   Normal, benigno e maligno é um recorte compreensível e viável para TCC1/TCC2.

## 7. Fragilidades, lacunas ou ambiguidades

As fragilidades principais são as seguintes.

### 7.1 A metodologia ainda não está tecnicamente especificada

Mesmo que o capítulo metodológico ainda venha depois, as seções iniciais deveriam deixar mais claro o tipo de estudo computacional. Recomendo nomear explicitamente como:

> estudo experimental comparativo, quantitativo e reprodutível.

### 7.2 Falta definição de unidade experimental

Em mamografia, isso é crítico. O trabalho precisa dizer se cada amostra é:

- uma imagem individual;
- uma mama;
- um exame completo;
- uma paciente;
- uma combinação de vistas CC/MLO.

Sem isso, a comparação fica metodologicamente ambígua.

### 7.3 Falta explicitação sobre vazamento de dados

Esse é talvez o maior risco computacional do TCC. Se imagens da mesma paciente aparecem em treino e teste, o modelo pode memorizar padrões e gerar métricas infladas. O texto precisa mencionar explicitamente que, quando os metadados permitirem, a divisão será feita por paciente ou exame, não apenas por imagem.

### 7.4 Falta baseline clássico equivalente ao híbrido

Comparar uma CNN completa contra uma CNN + circuito quântico não basta. É necessário comparar também contra uma CNN com uma camada densa ou gargalo clássico de dimensão equivalente ao número de qubits/observáveis.

### 7.5 O termo "aprimorar" é vago

O objetivo específico 3 diz "aprimorar uma CNN clássica". Em Ciência da Computação, isso precisa ser mensurável. Aprimorar como?

- alterar arquitetura?
- ajustar regularização?
- aumentar augmentation?
- trocar otimizador?
- usar normalização?
- aplicar early stopping?
- reduzir overfitting?

Sugiro substituir por algo mais objetivo:

> Implementar e ajustar uma CNN clássica de referência, documentando arquitetura, hiperparâmetros e critérios de seleção do melhor modelo.

### 7.6 O escopo pode ficar grande demais

O objetivo geral menciona "possibilidade de ampliação para uma classificação mais detalhada". Como avaliador, eu retiraria isso do objetivo geral. Para TCC2, manter três classes já é suficientemente desafiador. A ampliação pode aparecer como trabalho futuro.

## 8. Sugestões concretas de melhoria

Minhas recomendações são:

1. **Inserir uma pergunta computacional explícita**

   Exemplo:

   > Sob um protocolo experimental controlado, uma arquitetura híbrida quântico-clássica apresenta desempenho preditivo, estabilidade e custo computacional competitivos em relação a uma CNN clássica na classificação supervisionada de mamografias em três classes?

2. **Definir a unidade experimental**

   Informar se o modelo classificará imagem, exame, mama ou paciente.

3. **Adicionar critério de divisão dos dados**

   Recomendo declarar:

   > A divisão dos dados buscará evitar vazamento entre treino, validação e teste, priorizando separação por paciente ou exame quando os metadados permitirem.

4. **Definir métrica principal e métricas secundárias**

   Sugestão:

   - métrica principal: AUC macro ou AUC one-vs-rest;
   - métrica clínica crítica: recall da classe maligna;
   - métricas complementares: F1 macro, precisão, acurácia e matriz de confusão;
   - métricas computacionais: tempo por época, tempo total, uso de memória e estabilidade entre execuções.

5. **Incluir baseline clássico equivalente**

   Além da CNN clássica e do modelo híbrido, incluir:

   > CNN clássica com gargalo denso de mesma dimensão da entrada quântica.

6. **Definir o que significa estabilidade**

   Estabilidade pode ser medida por média e desvio-padrão em múltiplas execuções com seeds diferentes.

7. **Definir o que significa custo computacional**

   Especificar se será medido por:

   - tempo de treino;
   - tempo de inferência;
   - uso de GPU;
   - uso de RAM/VRAM;
   - número de parâmetros;
   - número de execuções do circuito;
   - crescimento do custo com número de qubits.

8. **Retirar ampliação de classes do objetivo geral**

   Deixar como possibilidade futura, não como compromisso do TCC.

## 9. Perguntas que uma banca real poderia fazer

1. Qual é exatamente a unidade de entrada do modelo: imagem, exame, mama ou paciente?
2. Como você garantirá que não haverá vazamento de dados entre treino e teste?
3. A divisão será estratificada por classe?
4. Quantas execuções serão feitas para medir estabilidade?
5. Qual será a métrica principal de comparação?
6. Por que a CNN escolhida é um baseline justo?
7. O modelo híbrido será comparado com uma versão clássica de mesma dimensionalidade?
8. Como você medirá custo computacional?
9. Como será registrado o ambiente experimental?
10. O código terá seeds fixas e versões documentadas das bibliotecas?
11. O modelo híbrido será treinado fim a fim ou em etapas?
12. Como você vai separar a contribuição da CNN da contribuição do circuito quântico?
13. Qual será o critério para dizer que o modelo híbrido é inviável?
14. A classe maligna terá prioridade na análise?
15. Como serão tratados rótulos ausentes, inconsistentes ou bases com distribuições diferentes?

## Parecer parcial do professor de Ciência da Computação

A proposta é adequada para um TCC de Ciência da Computação e possui bom potencial como estudo experimental comparativo. Os objetivos específicos estão bem direcionados e demonstram preocupação com protocolo, métricas, custo computacional e viabilidade. A hipótese é prudente e evita a alegação prematura de vantagem quântica.

Entretanto, o trabalho precisa melhorar a formalização computacional do problema. A banca provavelmente exigirá maior precisão sobre unidade experimental, divisão dos dados, prevenção de vazamento, baseline equivalente, métrica principal, controle de aleatoriedade e critérios de reprodutibilidade.

**Meu parecer é favorável à continuidade, com ajustes metodológicos obrigatórios. O projeto é viável, mas só será cientificamente forte se a comparação entre CNN clássica e modelo híbrido for justa, reprodutível e tecnicamente controlada.**

---

# Rodada 3 - Professor entusiasta em tecnologia e inovação

## Avaliação individual

Como professor entusiasta em tecnologia e inovação, minha avaliação parte de uma pergunta central: **este TCC apresenta uma proposta tecnicamente atual, socialmente relevante e com potencial de gerar aprendizado aplicado, mesmo que ainda não produza uma solução pronta para uso clínico?**

Minha resposta inicial é: **sim, o trabalho tem potencial inovador**, mas precisa tomar cuidado para não vender a computação quântica como uma promessa maior do que a metodologia conseguirá sustentar. A força do projeto está justamente em tratar a inovação com cautela: testar, comparar, medir e reconhecer limites.

## 1. Clareza do problema de pesquisa

O texto apresenta bem o cenário geral: IA aplicada à saúde, classificação de mamografias, CNNs clássicas e modelos híbridos quântico-clássicos. A introdução afirma que o trabalho propõe um estudo comparativo entre uma arquitetura clássica baseada em CNN e uma arquitetura híbrida quântico-clássica aplicada à classificação de mamografias digitais, avaliando desempenho preditivo, estabilidade, custo computacional e viabilidade prática.

Esse é um bom ponto de partida. Porém, como avaliador com foco em inovação, eu vejo uma fragilidade: **a proposta ainda não deixa totalmente explícito qual é a inovação principal**.

Existem pelo menos três possíveis leituras:

1. inovação na aplicação de IA em mamografias;
2. inovação na comparação entre CNN clássica e modelo híbrido quântico-clássico;
3. inovação na análise de viabilidade prática de uma abordagem emergente.

A terceira é, na minha visão, a mais forte. O TCC não deveria se apresentar como "um novo sistema para diagnóstico de câncer de mama", mas como:

> **um estudo experimental sobre a viabilidade de arquiteturas híbridas quântico-clássicas em uma tarefa realista de classificação de mamografias.**

Essa formulação é mais inovadora, mais honesta e mais defensável.

## 2. Relevância do tema

A relevância social está bem construída. O texto reconhece o câncer de mama como problema de alta incidência e dependente de estratégias de detecção precoce, justificando a investigação de métodos computacionais de apoio à análise de mamografias. Também é positivo o cuidado em dizer que o trabalho **não tem objetivo de uso clínico imediato**, mas se insere em uma linha de pesquisa com impacto potencial na saúde.

Esse cuidado é importante. Em projetos de inovação em saúde, existe uma diferença grande entre:

- protótipo acadêmico;
- modelo experimental;
- sistema de apoio à decisão;
- ferramenta validada clinicamente;
- produto regulado para uso médico.

O TCC está no primeiro ou segundo nível. Ele pode gerar conhecimento e protótipo experimental, mas ainda não deve prometer aplicação clínica.

Do ponto de vista de inovação, isso não enfraquece o trabalho. Pelo contrário: fortalece. Uma banca tende a valorizar mais uma proposta que entende seu estágio de maturidade do que uma proposta que promete transformação clínica sem validação suficiente.

## 3. Qualidade da fundamentação teórica na parte avaliada

A justificativa trabalha três dimensões: social, acadêmica e lacuna científica. Essa estrutura é boa. O texto afirma que deep learning em mamografia tem desempenho promissor, mas apresenta limitações de reprodutibilidade e avaliação realista; também afirma que trabalhos quânticos recentes ainda dependem de cenários restritos, bases menores e simulação.

Esse trecho é relevante porque sustenta o caráter inovador do trabalho: **não basta aplicar uma tecnologia nova; é preciso avaliar se ela realmente se sustenta em comparação com uma alternativa clássica**.

A fundamentação, porém, poderia melhorar em um aspecto: falta uma discussão mais clara sobre **maturidade tecnológica**. A computação quântica aparece como tecnologia emergente, mas seria útil deixar explícito que o trabalho está lidando com uma tecnologia em fase exploratória, especialmente quando aplicada a imagens médicas de alta dimensão.

Sugestão: incluir uma frase na justificativa ou nas delimitações dizendo que:

> A proposta deve ser compreendida como uma investigação experimental de viabilidade, e não como desenvolvimento de uma solução diagnóstica pronta para adoção clínica.

Isso evita interpretações exageradas.

## 4. Coerência entre introdução, objetivos, hipótese e limitações

A coerência é boa. O objetivo geral propõe investigar comparativamente CNNs clássicas e modelos híbridos quântico-clássicos, considerando desempenho preditivo, custo computacional, estabilidade experimental e viabilidade prática.

Os objetivos específicos estão alinhados com essa proposta, especialmente ao incluir a criação de protocolo padronizado, a CNN como referência, a arquitetura híbrida compatível com limitações de simulação, a investigação de número de qubits, feature map, profundidade do circuito e estratégia de codificação, além da comparação por métricas preditivas e computacionais.

A hipótese também é coerente e bem formulada. Ela não assume superioridade da abordagem quântica e reconhece que a viabilidade depende de custo computacional, número de qubits, sensibilidade a hiperparâmetros, codificação de dados e restrições NISQ.

Esse é um dos pontos mais positivos do texto: a inovação é tratada como hipótese investigável, não como afirmação promocional.

A fragilidade está no objetivo geral quando menciona "possibilidade de ampliação para uma classificação mais detalhada". Como professor de inovação, eu entendo a intenção de mostrar visão futura, mas isso pode parecer excesso de escopo. O trabalho já é ambicioso com três classes e comparação híbrida. Essa ampliação deveria aparecer como **perspectiva futura**, não como parte do objetivo principal.

## 5. Viabilidade técnica e metodológica

A proposta é viável se for apresentada como **prova de conceito experimental**. Ela se torna arriscada se for apresentada como solução diagnóstica ou como demonstração de vantagem quântica.

A computação quântica, nesse contexto, funciona mais como uma frente de investigação tecnológica do que como uma tecnologia pronta. O texto já reconhece que o modelo híbrido precisará respeitar limitações de simulação e que a hipótese não é demonstrar vantagem quântica definitiva.

Esse enquadramento é adequado.

No entanto, para inovação, a viabilidade não depende apenas de funcionar tecnicamente. Também depende de responder:

- O que será aprendido se o modelo híbrido for pior?
- O que será aprendido se ele empatar?
- O que será aprendido se ele for melhor em uma métrica, mas muito mais caro?
- O que será aprendido se ele tiver melhor recall, mas pior estabilidade?
- O que será aprendido se ele for inviável acima de poucos qubits?

Essas perguntas são importantes porque mostram que o valor do TCC não está apenas em obter alta acurácia. O valor está em mapear **condições de viabilidade e inviabilidade**.

## 6. Pontos fortes do texto

Os principais pontos fortes são:

1. **Tema com alto apelo social e tecnológico**  
   Câncer de mama, IA médica e computação quântica são temas atuais e relevantes.

2. **Boa postura diante da inovação**  
   O texto não promete uso clínico imediato e não assume superioridade quântica. Isso é academicamente maduro.

3. **Proposta comparativa clara**  
   A comparação entre CNN clássica e arquitetura híbrida dá ao trabalho um eixo objetivo.

4. **Critérios além da acurácia**  
   O texto inclui estabilidade, custo computacional, memória e escalabilidade. Isso torna a análise mais rica e mais próxima de uma discussão real de tecnologia.

5. **Lacuna científica bem posicionada**  
   A justificativa aponta que modelos híbridos ainda carecem de validação comparativa rigorosa em aplicações médicas.

6. **Potencial de continuidade**  
   O trabalho pode evoluir para artigo, IC, experimentos futuros, comparação com outras arquiteturas e discussão sobre computação quântica aplicada à saúde.

## 7. Fragilidades, lacunas ou ambiguidades

### 7.1 O diferencial inovador ainda precisa ser mais explícito

O texto fala de IA, mamografia e computação quântica, mas precisa declarar com mais força:

> A inovação do trabalho está na avaliação comparativa controlada de uma arquitetura híbrida quântico-clássica em uma tarefa de mamografia, considerando não apenas desempenho, mas também viabilidade computacional.

Essa frase, ou uma semelhante, ajudaria muito.

### 7.2 O resumo está mais fraco que a introdução

O resumo afirma que o objetivo é aprimorar uma arquitetura anterior que classificava imagens com cerca de 70% de precisão e fazer o modelo quântico obter resultados além do chute aleatório.

Esse resumo tem valor histórico, mas soa informal e defensivo. Para uma banca, ele pode dar a impressão de que o trabalho é apenas uma continuação de tentativa e erro. Sugiro reescrever com linguagem mais acadêmica, enfatizando comparação experimental, protocolo controlado, métricas, limitações e viabilidade.

### 7.3 Risco de "hype quântico"

Mesmo com a hipótese cautelosa, o tema pode gerar expectativa excessiva. A banca pode questionar se o componente quântico tem justificativa técnica real ou se foi incluído apenas por ser uma tecnologia emergente.

Para reduzir esse risco, o texto deve explicar melhor:

- por que testar uma camada quântica nesse problema;
- o que ela teoricamente poderia representar;
- por que a comparação com CNN clássica é adequada;
- quais resultados seriam considerados úteis mesmo sem superioridade.

### 7.4 Falta uma noção de maturidade da solução

Seria interessante classificar o trabalho como:

- estudo experimental;
- prova de conceito;
- comparação de arquiteturas;
- investigação de viabilidade.

Isso evita que o leitor espere uma ferramenta clínica.

### 7.5 A inovação precisa ser separada da aplicação

A aplicação é mamografia. A inovação está na comparação metodológica e na análise de viabilidade híbrida. Misturar as duas coisas pode deixar o argumento menos claro.

## 8. Sugestões concretas de melhoria

Minhas recomendações são:

1. **Adicionar uma frase explícita sobre o diferencial inovador**

   Sugestão:

   > O diferencial deste trabalho está em avaliar, de forma controlada e reprodutível, se a inserção de um componente quântico simulado em uma arquitetura de classificação de mamografias produz ganhos mensuráveis ou revela limitações práticas em comparação com uma CNN clássica.

2. **Reformular o resumo**

   Evitar expressões como "além do chute aleatório" e "melhoria nos dois tipos de modelos". Substituir por linguagem acadêmica:

   > Busca-se comparar uma CNN clássica e uma arquitetura híbrida quântico-clássica, analisando desempenho preditivo, estabilidade, custo computacional e limitações de escalabilidade.

3. **Definir o estágio da tecnologia**

   Inserir algo como:

   > O trabalho deve ser entendido como uma investigação experimental de viabilidade tecnológica, sem pretensão de validação clínica ou implantação em ambiente hospitalar.

4. **Explicitar os possíveis resultados úteis**

   O TCC será relevante mesmo se o modelo híbrido não superar a CNN, desde que mostre claramente:

   - onde ele falha;
   - quanto custa;
   - quando satura;
   - qual configuração é mais estável;
   - quais limitações aparecem na prática.

5. **Remover a ampliação de classes do objetivo geral**

   Manter três classes como escopo central e deixar classificações mais detalhadas como trabalho futuro.

6. **Criar uma pequena seção de "contribuições esperadas"**

   Isso ajudaria muito. Poderia conter:

   - protocolo comparativo entre CNN e modelo híbrido;
   - análise de desempenho e custo;
   - discussão crítica sobre viabilidade de QML em imagens médicas;
   - base para estudos futuros em arquiteturas híbridas.

## 9. Perguntas que uma banca real poderia fazer

1. Qual é exatamente a inovação do seu trabalho?
2. O que seu TCC entrega mesmo se o modelo quântico não superar a CNN?
3. Por que usar computação quântica nesse problema específico?
4. O trabalho pretende criar uma ferramenta clínica ou apenas uma prova de conceito?
5. Como você evitará exagerar as conclusões sobre computação quântica?
6. Qual seria um resultado positivo para você: vencer a CNN, empatar ou apenas entender os limites?
7. Como você vai comunicar os resultados negativos, caso eles ocorram?
8. O modelo híbrido tem potencial prático ou apenas valor exploratório?
9. Qual seria o próximo passo depois do TCC2?
10. Que tipo de contribuição esse trabalho poderia gerar para artigo científico?

## Parecer parcial do professor entusiasta em tecnologia e inovação

O trabalho tem um tema forte, atual e com bom potencial de inovação acadêmica. A combinação entre mamografia, CNNs e modelos híbridos quântico-clássicos é interessante e pode gerar uma discussão relevante sobre os limites de tecnologias emergentes em problemas reais.

Entretanto, o projeto precisa deixar mais claro que sua inovação não está em oferecer uma solução clínica pronta, mas em produzir uma **avaliação experimental crítica** de uma tecnologia emergente. A proposta será mais convincente se assumir explicitamente seu caráter de prova de conceito e se tratar resultados negativos ou limitados como contribuição científica válida.

**Meu parecer é favorável à continuidade, com a recomendação de reforçar o diferencial inovador, reduzir promessas implícitas e apresentar a computação quântica como objeto de investigação crítica, não como solução garantida.**

---

# Rodada 4 - Professor especialista em Computação Quântica

## Avaliação individual

Como professor especialista em Computação Quântica, minha avaliação se concentra na forma como o trabalho apresenta o componente quântico, na adequação das promessas feitas, na coerência com as limitações de dispositivos NISQ e na validade da comparação entre modelos clássicos e híbridos quântico-clássicos.

De modo geral, o trabalho demonstra uma postura prudente. O texto não afirma que a computação quântica será superior, mas propõe investigar em quais condições a abordagem híbrida pode ser competitiva, limitada ou inviável. Esse é um ponto positivo, porque a área de aprendizado de máquina quântico ainda exige bastante cautela, especialmente quando aplicada a imagens médicas de alta dimensão.

## 1. Clareza do problema de pesquisa

O problema geral está bem encaminhado: comparar CNNs clássicas e modelos híbridos quântico-clássicos na classificação de mamografias. O objetivo geral menciona desempenho preditivo, custo computacional, estabilidade experimental e viabilidade prática, o que é adequado para esse tipo de estudo.

Entretanto, do ponto de vista da computação quântica, ainda falta clareza sobre **qual é exatamente o papel do componente quântico**.

O texto diz que a arquitetura híbrida usará circuitos quânticos simulados como componente treinável complementar às camadas clássicas de uma rede neural. Essa formulação é correta, mas ainda genérica. Uma banca da área provavelmente perguntaria:

- o circuito quântico será usado como classificador final?
- será usado como camada intermediária?
- substituirá uma camada densa?
- atuará como feature map não linear?
- será treinado junto com a CNN ou separadamente?
- haverá emaranhamento entre qubits?
- quais observáveis serão medidos?
- qual codificação será usada para inserir os dados clássicos no circuito?

Essas definições não precisam aparecer todas na introdução, mas a introdução deveria antecipar minimamente a arquitetura. Hoje, a ideia "modelo híbrido quântico-clássico" aparece de modo conceitual, mas ainda não aparece como desenho experimental suficientemente delimitado.

## 2. Relevância do tema

A relevância é boa. O texto reconhece que modelos híbridos quântico-clássicos ainda carecem de validação comparativa rigorosa, principalmente em aplicações médicas, e propõe investigar se componentes quânticos trazem benefícios mensuráveis em um problema concreto.

Esse é um bom recorte. A relevância quântica do trabalho não está em construir um algoritmo quântico universal nem em demonstrar vantagem quântica. Está em avaliar uma arquitetura híbrida em um domínio difícil e realista.

O TCC também acerta ao dizer que os trabalhos recentes em classificação de imagens com modelos quânticos ainda aparecem em cenários restritos, com bases menores, forte dependência de simulação e poucas evidências em contextos próximos do uso aplicado.

Esse argumento é forte. Mas eu recomendaria deixar explícito que, em mamografias, o desafio não é apenas "usar qubits", e sim lidar com a discrepância entre:

- imagens de altíssima dimensão;
- poucos qubits simuláveis;
- circuitos rasos;
- necessidade de compressão clássica;
- risco de perda de informação diagnóstica;
- custo exponencial de simulação.

O próprio texto reconhece que uma mamografia 1024 x 1024 possui mais de um milhão de pixels e que codificar diretamente esses valores em um circuito quântico é impraticável nos dispositivos atuais e também em simuladores clássicos. Esse ponto é essencial e deveria estar mais conectado à justificativa inicial.

## 3. Qualidade da fundamentação teórica na parte avaliada

A fundamentação introdutória é boa em termos de prudência, mas ainda precisa diferenciar melhor alguns conceitos quânticos.

O texto menciona computação quântica, aprendizado de máquina quântico, modelos híbridos, circuitos parametrizados, codificação de dados, barren plateaus e restrições NISQ ao longo do trabalho. A revisão reconhece que modelos híbridos usam componentes clássicos com circuitos quânticos parametrizados, delegando ao computador clássico o pré-processamento, a extração de características, a otimização e a classificação final ou parcial.

Isso é adequado. Porém, nas seções iniciais, a fundamentação ficaria mais forte se fossem definidos com mais precisão três elementos:

### 3.1 Codificação dos dados

O maior gargalo de modelos quânticos aplicados a imagens é a codificação. O texto já reconhece que modelos híbridos normalmente precisam de extração ou compressão clássica antes da codificação quântica.

Mas a proposta precisa dizer qual tipo de codificação será investigada:

- **angle encoding**;
- **amplitude encoding**;
- **basis encoding**;
- **ZZFeatureMap**;
- **data re-uploading**;
- outra estratégia.

Sem isso, o componente quântico fica abstrato demais.

### 3.2 Ansatz variacional

Também é necessário dizer que tipo de ansatz será usado ou comparado. Um circuito variacional pode ter comportamentos muito diferentes dependendo de profundidade, padrão de emaranhamento e número de parâmetros.

A revisão já discute que circuitos muito expressivos ou aleatórios podem sofrer com barren plateaus, enquanto circuitos simples podem ter baixa capacidade de separação. Essa discussão é correta, mas precisa ser incorporada à metodologia e às delimitações.

### 3.3 Medição e saída do circuito

Em modelos híbridos, a saída do circuito normalmente vem de valores esperados de observáveis, por exemplo medições em Pauli-Z.

Na proposta, seria importante explicar se a saída quântica terá:

- uma medida por qubit;
- uma medida agregada;
- probabilidades de estados;
- valores esperados usados como features;
- conexão direta com camada densa final.

Esse detalhe é técnico, mas decisivo para a clareza do TCC.

## 4. Coerência entre introdução, objetivos, hipótese e limitações

A coerência é um dos pontos mais fortes.

Os objetivos específicos indicam que o aluno pretende projetar uma arquitetura híbrida compatível com limitações de simulação, investigar número de qubits, feature map, profundidade do circuito e estratégia de codificação, além de avaliar tempo de treinamento, memória, estabilidade e escalabilidade.

Isso está muito alinhado com a realidade da computação quântica atual.

A hipótese também é bem formulada. O texto afirma que não se pressupõe superioridade geral da abordagem quântica e que a viabilidade prática será condicionada por custo computacional, número reduzido de qubits, sensibilidade a hiperparâmetros, estratégia de codificação e restrições NISQ.

Esse cuidado é academicamente correto.

A delimitação também está bem direcionada ao tratar o trabalho como estudo experimental comparativo em visão computacional, com classificação supervisionada em três classes - normal, benigno e maligno - e comparação entre CNN clássica e arquitetura híbrida sob a mesma base, pré-processamento, divisão e métricas.

Minha ressalva é que a delimitação deveria ser ainda mais rígida no componente quântico. Sugiro especificar:

> O componente quântico será avaliado apenas em simulação, com número reduzido de qubits e circuitos rasos, sem alegação de vantagem quântica ou execução em hardware quântico real.

Essa frase evitaria questionamentos indevidos.

## 5. Viabilidade técnica e metodológica

A proposta é viável, mas com forte risco de complexidade.

A estratégia mais viável é usar a CNN como extratora de características e projetar o vetor extraído para um número pequeno de qubits. A revisão já descreve essa estrutura: uma rede clássica extrai características, essas características são projetadas para uma dimensão compatível com os qubits, codificadas em circuito quântico e depois processadas por camadas clássicas para classificação final.

Esse caminho é tecnicamente correto.

O que não seria viável é tentar codificar a imagem inteira em um circuito quântico. O texto reconhece isso ao afirmar que codificar diretamente todos os pixels de uma mamografia é impraticável, exigindo compressão, extração de características ou processamento local.

### Riscos técnicos principais

1. **Custo de simulação**  
   Em simulação statevector, o custo cresce rapidamente com o número de qubits. Mesmo circuitos pequenos podem se tornar lentos se forem executados muitas vezes durante o treinamento.

2. **Medições probabilísticas**  
   Se forem usados shots, será necessário repetir execuções para estimar valores esperados. Isso aumenta custo e variância.

3. **Barren plateaus**  
   Em certas famílias de circuitos, a variância dos gradientes pode decair exponencialmente com o número de qubits, dificultando a otimização.

4. **Compressão excessiva**  
   Ao reduzir uma mamografia de alta dimensão para poucos qubits, informações pequenas e clinicamente relevantes podem desaparecer. Isso é crítico em microcalcificações e lesões sutis.

5. **Comparação injusta com CNN**  
   Se a CNN clássica tiver muito mais capacidade que o modelo híbrido, a comparação pode apenas mostrar que modelos maiores performam melhor. Por outro lado, se o híbrido tiver uma CNN clássica forte antes do circuito, pode ser difícil saber se o ganho veio da parte clássica ou da quântica.

## 6. Pontos fortes do texto

Os principais pontos fortes, pela perspectiva de computação quântica, são:

1. **Cautela conceitual**  
   O texto não promete vantagem quântica definitiva.

2. **Reconhecimento das limitações NISQ**  
   O trabalho menciona poucos qubits, simulação, sensibilidade a hiperparâmetros, codificação e custo computacional.

3. **Boa formulação da hipótese**  
   A hipótese permite três resultados cientificamente válidos: competitivo, limitado ou inviável.

4. **Preocupação com escalabilidade**  
   O texto propõe avaliar tempo de treinamento, memória, estabilidade e limitações de escalabilidade.

5. **Integração correta entre CNN e circuito quântico**  
   A abordagem de usar etapas clássicas para reduzir a dimensão antes do circuito quântico é coerente com o estado atual da tecnologia.

6. **Boa consciência sobre imagens de alta dimensão**  
   O trabalho reconhece que mamografias tornam as limitações quânticas mais evidentes, especialmente pela impossibilidade de codificação direta dos pixels.

## 7. Fragilidades, lacunas ou ambiguidades

### 7.1 O termo "modelo quântico" ainda está genérico

O texto fala em "modelo híbrido quântico-clássico", mas ainda precisa nomear com precisão o tipo de componente:

- VQC?
- QNN?
- circuito variacional?
- quantum layer?
- quanvolutional layer?
- quantum kernel?
- quantum classifier?

Pela proposta descrita, parece mais adequado chamar de **modelo híbrido com circuito variacional quântico simulado**.

### 7.2 Falta definição da codificação

A codificação é o núcleo do problema. Sem ela, o modelo híbrido não está metodologicamente definido.

### 7.3 Falta definição do ansatz

O texto precisa indicar se usará RealAmplitudes, EfficientSU2, ZZFeatureMap + ansatz, camadas RY/CNOT, ou outro circuito.

### 7.4 Falta critério para número de qubits

O objetivo menciona investigar número de qubits, mas seria importante estabelecer uma faixa realista, por exemplo 4, 6, 8 ou 10 qubits, dependendo do simulador e do hardware disponível.

### 7.5 Falta baseline para isolar contribuição quântica

É essencial comparar contra uma camada clássica de mesma dimensão. Caso contrário, não será possível saber se o circuito quântico contribuiu ou se apenas funcionou como gargalo/regularizador.

### 7.6 Falta explicação sobre ruído

O trabalho cita NISQ, mas parece que os experimentos serão em simulação. Se a simulação for ideal, sem ruído, então é necessário deixar claro que o estudo avalia **viabilidade algorítmica simulada**, não comportamento real em hardware NISQ ruidoso.

## 8. Sugestões concretas de melhoria

Minhas recomendações são:

1. **Especificar o tipo de modelo quântico**

   Sugestão de redação:

   > O modelo híbrido será composto por uma CNN clássica para extração de características, uma camada de projeção para reduzir o vetor de atributos ao número de qubits e um circuito quântico variacional simulado, cujas medições serão encaminhadas a uma cabeça clássica de classificação.

2. **Definir a estratégia de codificação**

   Mesmo que depois você teste variações, escolha uma principal. Por exemplo:

   > angle encoding com rotações RY ou RZ.

3. **Definir o ansatz**

   Indicar a arquitetura do circuito:

   - camadas de rotações parametrizadas;
   - padrão de CNOTs;
   - profundidade;
   - número de parâmetros;
   - observáveis medidos.

4. **Definir faixa de qubits**

   Exemplo:

   > Serão avaliadas configurações com 4, 6 e 8 qubits, respeitando o limite de simulação disponível.

5. **Adicionar baselines de ablação**

   Recomendo pelo menos:

   - CNN completa;
   - CNN com gargalo clássico de mesma dimensão;
   - CNN + circuito quântico sem emaranhamento;
   - CNN + circuito quântico com emaranhamento;
   - se possível, circuito com parâmetros congelados para verificar se o treino quântico importa.

6. **Definir o critério de viabilidade quântica**

   Por exemplo:

   > O modelo será considerado inviável se apresentar custo computacional muito superior sem ganho em AUC, recall da classe maligna ou estabilidade.

7. **Evitar qualquer linguagem de vantagem quântica forte**

   Usar termos como:

   - "potencial";
   - "investigação experimental";
   - "componente quântico simulado";
   - "viabilidade limitada";
   - "modelo híbrido em cenário controlado".

8. **Separar simulação ideal de hardware real**

   Se não houver execução em hardware real, diga explicitamente:

   > O trabalho não avalia ruído físico real, decoerência ou limitações de conectividade de dispositivos quânticos reais.

## 9. Perguntas que uma banca real poderia fazer

1. Qual codificação de dados clássicos em estados quânticos será usada?
2. Por que essa codificação é adequada para características extraídas de mamografias?
3. Quantos qubits você pretende usar e por quê?
4. Qual será o ansatz do circuito variacional?
5. O circuito terá emaranhamento? Como?
6. Quais observáveis serão medidos na saída?
7. O circuito será treinado junto com a CNN ou depois dela?
8. Como você calculará gradientes do circuito quântico?
9. Usará statevector, shots ou backend ruidoso?
10. Como o custo cresce quando o número de qubits aumenta?
11. Como você pretende evitar ou diagnosticar barren plateaus?
12. Como saberá se o circuito quântico agregou algo além de uma camada densa clássica?
13. Qual baseline clássico terá a mesma dimensão do circuito quântico?
14. O que significa "vantagem" ou "competitividade" no seu experimento?
15. Seu trabalho avalia computação quântica real ou apenas simulação de circuitos quânticos?

## Parecer parcial do professor de Computação Quântica

A proposta é pertinente e bem posicionada para uma investigação experimental de TCC. O texto demonstra maturidade ao não assumir superioridade quântica e ao reconhecer limitações de simulação, número reduzido de qubits, sensibilidade a hiperparâmetros, codificação de dados e restrições NISQ.

Contudo, para ficar tecnicamente robusto, o trabalho precisa especificar melhor o componente quântico: codificação, ansatz, número de qubits, medições, backend, uso ou não de shots, estratégia de treinamento e baselines clássicos equivalentes. Sem isso, a expressão "modelo híbrido quântico-clássico" permanece ampla demais.

**Meu parecer é favorável à continuidade, desde que o TCC trate o componente quântico como objeto de investigação crítica e metodologicamente controlada, não como garantia de melhoria. A proposta é viável se permanecer restrita a circuitos pequenos, simulação controlada e comparação justa com baselines clássicos equivalentes.**

---

# Rodada 5 - Professor especialista em Física Quântica

## Avaliação individual

Como professor especialista em Física Quântica, minha avaliação se concentra menos na implementação computacional do circuito e mais na **correção conceitual dos princípios quânticos utilizados**, no cuidado com as interpretações físicas e na forma como o texto relaciona mecânica quântica, computação quântica e aprendizado de máquina.

Minha impressão geral é positiva: o trabalho trata a computação quântica com cautela e reconhece limitações importantes. Entretanto, há um risco típico em trabalhos interdisciplinares: usar conceitos como **superposição**, **emaranhamento**, **espaço de Hilbert** e **medição** de forma correta na revisão, mas ainda pouco conectada à hipótese física que justificaria o uso do componente quântico no modelo.

## 1. Clareza do problema de pesquisa

O problema geral está compreensível: comparar uma CNN clássica com uma arquitetura híbrida quântico-clássica na classificação de mamografias. A hipótese é formulada de maneira prudente, afirmando que a abordagem híbrida pode ser competitiva em algumas condições, mas sem pressupor superioridade geral da computação quântica. O texto também reconhece fatores limitantes como custo computacional, número reduzido de qubits, hiperparâmetros, codificação de dados e restrições NISQ.

Do ponto de vista da Física Quântica, isso é adequado. O problema não deve ser formulado como:

> A computação quântica é mais poderosa, logo deve melhorar a classificação.

Essa formulação seria frágil.

A formulação mais correta é:

> Um circuito quântico parametrizado, quando inserido em uma arquitetura híbrida, pode transformar uma representação clássica compacta em um espaço de estados cuja dinâmica e medições produzam atributos úteis para classificação?

Essa segunda formulação é mais próxima da física do problema. Ela coloca o foco na **representação**, na **evolução unitária**, na **medição** e na **capacidade expressiva** do circuito, sem afirmar vantagem quântica automaticamente.

## 2. Relevância do tema

A relevância é boa, principalmente porque o trabalho não tenta tratar a Física Quântica como ornamento tecnológico. O texto reconhece que modelos híbridos são adequados ao cenário NISQ porque usam circuitos pequenos e delegam ao computador clássico tarefas como pré-processamento, extração de características, otimização e classificação final.

Isso é importante. Em Física, a computação quântica não é uma "camada mágica"; ela é uma forma específica de manipular estados em espaços vetoriais complexos, sob restrições físicas reais. Portanto, é correto que o trabalho reconheça:

- número limitado de qubits;
- ruído;
- profundidade limitada;
- medições probabilísticas;
- dificuldade de simulação clássica;
- necessidade de redução dimensional antes da codificação.

O tema é relevante porque testa uma tecnologia emergente em um problema difícil, mas será ainda mais forte se o texto deixar claro que o interesse físico está em investigar **como a estrutura do circuito quântico altera a representação dos dados**, não apenas se a acurácia final melhora.

## 3. Qualidade da fundamentação teórica na parte avaliada

A fundamentação quântica do trabalho está bem encaminhada. O texto define a computação quântica como paradigma baseado em superposição, emaranhamento, interferência e medição probabilística; também apresenta o qubit como combinação linear dos estados $|0\rangle$ e $|1\rangle$, com amplitudes complexas normalizadas.

Esse é um ponto forte.

Também é positivo o texto indicar que, para $n$ qubits, o estado pertence a um espaço de dimensão $2^n$, mas que esse mesmo crescimento torna a simulação clássica rapidamente custosa. Essa observação é importante porque evita um erro comum: apresentar o crescimento exponencial do espaço de Hilbert apenas como vantagem, sem reconhecer o custo de simulação e controle.

Entretanto, eu faria três ressalvas conceituais.

### 3.1 Superposição não é "armazenar vários valores ao mesmo tempo" de forma simples

O texto parece correto, mas na apresentação oral você deve evitar dizer que o qubit "testa todas as respostas ao mesmo tempo" ou que "guarda infinitas possibilidades". Essa simplificação costuma ser malvista por uma banca com alguém de física.

A formulação mais segura é:

> O qubit é descrito por uma combinação linear de estados base, e os resultados observáveis aparecem por meio de medições probabilísticas.

### 3.2 Emaranhamento precisa ter função no circuito

Se o trabalho menciona emaranhamento, a banca pode perguntar: **onde ele aparece no circuito?**

Se o circuito usa portas CNOT, CZ ou blocos de entanglement, isso deve ser explicitado. Se não houver emaranhamento, então é melhor não apresentar o emaranhamento como recurso central do modelo.

### 3.3 Medição probabilística deve entrar na análise de custo

O texto reconhece que medições quânticas são probabilísticas e podem exigir múltiplas execuções, chamadas shots, para estimar valores esperados com precisão. Esse ponto deve aparecer na metodologia, porque tem impacto direto em custo, estabilidade e ruído estatístico.

## 4. Coerência entre introdução, objetivos, hipótese e limitações

A coerência é boa.

A hipótese está bem formulada porque diz que a superioridade quântica não é pressuposta e que o objetivo é investigar em quais condições a abordagem híbrida pode ser competitiva, limitada ou inviável.

A delimitação também é adequada ao definir o trabalho como estudo experimental comparativo em visão computacional, com classificação supervisionada em três classes e comparação entre CNN clássica e arquitetura híbrida mantendo constantes base, pré-processamento, divisão dos dados e métricas.

Do ponto de vista físico, porém, falta uma delimitação adicional:

> O trabalho utiliza simulação de circuitos quânticos, não hardware quântico físico.

Essa frase é importante. Se você não vai executar em um processador quântico real, o trabalho não mede efeitos físicos reais como decoerência, erros de porta, conectividade limitada, relaxação $T_1$, descoerência $T_2$ ou ruído de leitura. Ele avalia a viabilidade algorítmica de uma arquitetura inspirada em computação quântica, simulada em computador clássico.

Isso não é um problema. Mas precisa estar declarado.

## 5. Viabilidade técnica e conceitual

A proposta é viável, desde que o texto evite duas interpretações problemáticas:

1. **Achar que alta dimensionalidade do espaço de Hilbert implica automaticamente vantagem.**
2. **Achar que um circuito quântico pequeno consegue representar diretamente uma mamografia de alta resolução.**

O próprio TCC reconhece que uma mamografia 1024 x 1024 possui 1.048.576 pixels e que codificar diretamente todos esses valores em um circuito quântico é impraticável nos dispositivos atuais e também em simuladores clássicos.

Esse é um dos pontos mais importantes da proposta. Em Física Quântica, o espaço de Hilbert cresce exponencialmente, mas acessar, controlar, preparar e medir estados nesse espaço é uma tarefa altamente restrita. Portanto, o trabalho está correto ao propor redução dimensional ou extração clássica de características antes do circuito quântico.

A arquitetura híbrida descrita também é fisicamente plausível: uma rede clássica extrai características, projeta o vetor para uma dimensão compatível com o número de qubits, codifica o vetor em um circuito quântico, aplica um circuito variacional e extrai valores esperados de observáveis, como operadores de Pauli-Z.

Essa formulação é adequada e deve ser usada como base para explicar o modelo na defesa.

## 6. Pontos fortes do texto

Os principais pontos fortes são:

1. **Postura cautelosa sobre computação quântica**  
   O texto não promete vantagem quântica definitiva.

2. **Reconhecimento das limitações físicas e computacionais**  
   O trabalho menciona qubits limitados, circuitos rasos, custo de simulação, ruído e barren plateaus.

3. **Boa introdução dos conceitos fundamentais**  
   Qubits, superposição, medição e espaço de Hilbert são apresentados de forma adequada.

4. **Consciência da diferença entre simulação e realidade física**  
   O texto trata a abordagem híbrida como compatível com NISQ, mas ainda precisa delimitar melhor se os experimentos serão ideais, ruidosos ou em hardware real.

5. **Atenção ao problema da codificação**  
   O trabalho reconhece que a codificação direta de imagens médicas é impraticável e que a compressão pode remover informações relevantes.

6. **Formulação correta do circuito como parte de um pipeline maior**  
   O circuito é descrito como uma camada treinável dentro de uma arquitetura híbrida, e não como substituto completo de todo o processamento clássico.

## 7. Fragilidades, lacunas ou ambiguidades

### 7.1 Falta explicitar qual fenômeno físico é explorado

O texto menciona superposição, emaranhamento e medição, mas ainda falta responder:

> Qual desses recursos é de fato usado pelo modelo proposto?

Se o circuito usa apenas rotações independentes sem emaranhamento, a contribuição física é diferente de um circuito com portas de dois qubits. Se o circuito tem CNOTs, CZs ou blocos entanglers, isso deve ser mencionado.

### 7.2 Risco de confundir simulação com computação quântica física

Se tudo for executado em simulador, você deve evitar frases como "o computador quântico processa". Mais correto:

> O circuito quântico simulado processa uma representação compacta dos dados.

### 7.3 Falta discutir ruído físico

Como o trabalho menciona NISQ, a banca pode esperar alguma discussão de ruído. Se você não pretende simular ruído, delimite isso. Se pretende, diga qual ruído:

- depolarizing noise;
- amplitude damping;
- phase damping;
- readout error;
- finite shots.

### 7.4 Falta separar "vantagem quântica" de "efeito regularizador"

Um circuito quântico pequeno pode melhorar ou estabilizar o modelo não por vantagem quântica física, mas por atuar como um gargalo não linear ou regularizador. Essa distinção é importante.

### 7.5 Codificação pode destruir informação física relevante da imagem

Lesões pequenas, microcalcificações e alterações sutis podem desaparecer na compressão. O texto já reconhece esse risco. Agora é preciso mostrar como ele será mitigado ou, pelo menos, monitorado.

## 8. Sugestões concretas de melhoria

Minhas recomendações são:

1. **Adicionar uma delimitação explícita sobre simulação**

   Sugestão:

   > Os experimentos quânticos serão realizados em simulador clássico de circuitos quânticos, não em hardware quântico real. Assim, o estudo avalia a viabilidade algorítmica da arquitetura híbrida, sem medir diretamente efeitos físicos de ruído, decoerência ou limitações de conectividade de dispositivos reais.

2. **Explicitar os recursos quânticos usados**

   Exemplo:

   > O circuito explorará superposição por meio da codificação em rotações e, quando aplicável, correlações entre qubits por portas de emaranhamento.

3. **Evitar linguagem exagerada**

   Evitar expressões como:

   - "processa todas as possibilidades ao mesmo tempo";
   - "explora infinitas combinações";
   - "garante ganho por usar qubits";
   - "simula o comportamento do cérebro quântico" ou qualquer formulação semelhante.

4. **Definir se haverá simulação com shots**

   Se usar statevector ideal, diga isso. Se usar shots, explique que haverá ruído estatístico de medição.

5. **Discutir o papel físico da medição**

   A saída do circuito deve ser descrita como valor esperado de observáveis, por exemplo $\langle Z_j\rangle$, e não como uma simples "saída mágica" do circuito.

6. **Incluir uma comparação com camada clássica equivalente**

   Isso é importante também para Física: ajuda a diferenciar comportamento quântico simulado de uma simples transformação matemática clássica de baixa dimensão.

7. **Reforçar que espaço de Hilbert não significa vantagem automática**

   Sugestão de frase:

   > Embora o espaço de estados cresça exponencialmente com o número de qubits, a obtenção de vantagem prática depende da preparação dos estados, da estrutura do circuito, da medição e da comparação com métodos clássicos adequados.

## 9. Perguntas que uma banca real poderia fazer

1. Qual recurso físico quântico o seu circuito realmente utiliza?
2. O circuito possui emaranhamento? Quais portas geram esse emaranhamento?
3. Você usará simulador ideal, simulador com ruído ou hardware quântico real?
4. Qual a diferença entre simular um circuito quântico e executar em um processador quântico real?
5. O que significa medir um qubit no seu modelo?
6. A saída do circuito será probabilidade, valor esperado ou vetor de medições?
7. Como o número de shots afeta a estabilidade do modelo?
8. O seu circuito explora interferência quântica de alguma forma?
9. Por que um espaço de Hilbert maior poderia ajudar na separação das classes?
10. Como evitar a afirmação incorreta de vantagem quântica?
11. Se o modelo híbrido for melhor, como você saberá que não foi apenas efeito de regularização?
12. Se o modelo híbrido for pior, isso invalida a hipótese física?
13. Como a compressão clássica afeta informações pequenas da mamografia?
14. O modelo usa conceitos físicos reais ou apenas uma simulação matemática de circuitos?
15. Quais limitações físicas dos dispositivos NISQ não serão avaliadas no TCC?

## Parecer parcial do professor de Física Quântica

O trabalho apresenta uma base conceitual adequada e uma postura científica prudente. A proposta reconhece que modelos híbridos quântico-clássicos são limitados por número de qubits, profundidade, ruído, simulação e codificação dos dados, o que é essencial para evitar conclusões exageradas.

A principal melhoria necessária é explicitar melhor o papel físico do componente quântico: quais recursos são usados, como ocorre a codificação, que tipo de medição produz a saída e se haverá ou não simulação de ruído. Também é indispensável separar com clareza **simulação de circuito quântico** de **execução em hardware quântico real**.

**Meu parecer é favorável à continuidade, desde que o texto mantenha rigor conceitual e evite afirmações fortes sobre vantagem quântica. O projeto é válido como investigação experimental de uma arquitetura híbrida simulada, não como demonstração de superioridade física da computação quântica.**

---

# Rodada 6 - Professor especialista em Pesquisa Científica

## Avaliação individual

Como professor especialista em pesquisa científica, minha análise se concentra na qualidade do projeto como investigação acadêmica: problema, pergunta, hipótese, objetivos, justificativa, delimitação, coerência interna e possibilidade de produzir conhecimento verificável.

De forma geral, o trabalho está bem encaminhado. A proposta demonstra maturidade ao reconhecer que o objetivo não é provar superioridade quântica, mas comparar abordagens clássicas e híbridas sob condições controladas. Essa postura é adequada para um TCC experimental.

## 1. Clareza do problema de pesquisa

O problema de pesquisa está presente, mas ainda precisa ser mais explicitamente formulado.

A introdução afirma que o trabalho propõe um estudo comparativo entre uma arquitetura clássica baseada em CNN e uma arquitetura híbrida quântico-clássica aplicada à classificação de mamografias digitais, avaliando desempenho preditivo, estabilidade, custo computacional e viabilidade prática em ambiente experimental controlado.

Esse trecho é bom, mas ainda funciona mais como **descrição da proposta** do que como **formulação direta do problema de pesquisa**.

Como avaliador de metodologia científica, eu esperaria encontrar uma pergunta de pesquisa destacada, por exemplo:

> **Uma arquitetura híbrida quântico-clássica, baseada em circuitos quânticos simulados, apresenta desempenho, estabilidade e custo computacional competitivos em relação a uma CNN clássica na classificação supervisionada de mamografias em três classes?**

Essa pergunta ajudaria a conectar diretamente:

- o problema;
- o objetivo geral;
- a hipótese;
- as métricas;
- as limitações;
- a conclusão esperada.

Atualmente, o texto diz que o capítulo apresenta a pergunta de pesquisa, mas ela não aparece com destaque suficiente. Isso pode ser apontado por uma banca.

## 2. Relevância do tema

A relevância está bem defendida em três dimensões: social, acadêmica e científica.

A justificativa afirma que o câncer de mama possui alta incidência e depende de estratégias de detecção precoce e apoio à decisão clínica, mas também deixa claro que o trabalho não tem objetivo de uso clínico imediato. Esse cuidado é metodologicamente importante, porque evita extrapolação indevida dos resultados.

A relevância acadêmica também está bem construída. O texto afirma que o aprendizado profundo já está consolidado em visão computacional, mas que modelos híbridos quântico-clássicos ainda carecem de validação comparativa rigorosa, principalmente em aplicações médicas.

A justificativa ainda aponta uma lacuna científica: estudos de deep learning em mamografia têm desempenho promissor, mas apresentam limitações de reprodutibilidade e avaliação em condições realistas; já modelos quânticos aparecem em cenários restritos, com bases menores, forte dependência de simulação e poucas evidências próximas de uso aplicado.

Esse é um ponto forte. A lacuna não é apenas "falta usar computação quântica em mamografia", mas sim **falta avaliar de forma controlada e reprodutível se a abordagem híbrida tem viabilidade comparativa**.

## 3. Qualidade da fundamentação teórica na parte avaliada

Considerando apenas as seções iniciais, a fundamentação é adequada, mas ainda pode ser mais direcionada.

O texto apresenta o contexto médico, a complexidade da interpretação mamográfica e os desafios computacionais. Também menciona que achados como massas, microcalcificações, assimetrias e distorções arquiteturais podem ser sutis e difíceis de distinguir do tecido normal.

Isso fundamenta bem a relevância da tarefa.

No entanto, como projeto científico, o texto precisa tomar cuidado com uma questão: **a fundamentação não deve crescer apenas como revisão de conceitos; ela deve conduzir logicamente à lacuna e à hipótese**.

A sequência ideal seria:

1. câncer de mama e mamografia são relevantes;
2. interpretação de mamografias é difícil;
3. CNNs são úteis, mas têm limitações;
4. modelos híbridos quântico-clássicos são promissores, mas ainda pouco validados;
5. imagens médicas de alta dimensão tornam essa validação especialmente difícil;
6. portanto, é necessário um estudo comparativo controlado.

O texto já contém esses elementos, mas pode deixá-los mais encadeados.

## 4. Coerência entre objetivos, hipótese e delimitações

A coerência geral é boa.

O objetivo geral propõe investigar comparativamente CNNs clássicas e modelos híbridos quântico-clássicos na classificação de câncer de mama em mamografias, considerando desempenho preditivo, custo computacional, estabilidade experimental e viabilidade prática.

Os objetivos específicos são bem organizados e metodologicamente úteis. Eles incluem definição da base e das classes, protocolo de pré-processamento, divisão dos dados, treinamento, validação e teste, aprimoramento da CNN clássica, projeto da arquitetura híbrida, investigação de qubits, feature map, profundidade e codificação, além da comparação por métricas e avaliação de custo, memória, estabilidade e escalabilidade.

A hipótese também está bem alinhada. Ela declara que a arquitetura híbrida pode apresentar desempenho competitivo, mas que a comparação será feita sob protocolo controlado, com mesma base, critérios equivalentes de pré-processamento, divisão dos dados, métricas e ambiente computacional.

Esse é um dos melhores trechos do projeto, porque mostra consciência metodológica.

A delimitação também é adequada ao definir o trabalho como estudo experimental comparativo em visão computacional, com classificação supervisionada inicialmente em três classes: normal, benigno e maligno.

A principal fragilidade é que as delimitações ainda não deixam claro **o que será considerado evidência suficiente** para aceitar, rejeitar ou relativizar a hipótese.

## 5. Viabilidade científica e metodológica

A proposta é viável como TCC, mas precisa transformar algumas intenções em critérios verificáveis.

Hoje, o texto diz que serão avaliados desempenho, estabilidade, custo computacional e viabilidade prática. Isso é correto. Mas, cientificamente, cada um desses termos precisa ser operacionalizado.

### Exemplo de operacionalização necessária

| Conceito citado no TCC | Como deveria ser medido |
|---|---|
| Desempenho preditivo | AUC, F1 macro, recall da classe maligna, matriz de confusão |
| Estabilidade | média e desvio-padrão em múltiplas execuções |
| Custo computacional | tempo de treino, tempo de inferência, RAM/VRAM, número de parâmetros |
| Viabilidade prática | relação entre desempenho, custo e escalabilidade |
| Competitividade | diferença máxima aceitável em relação à CNN clássica |

Sem essas definições, há risco de a conclusão ficar opinativa. Por exemplo, dizer "o modelo híbrido foi competitivo" exige um critério anterior.

A banca pode perguntar:

> Competitivo em qual métrica? Com qual margem? Em relação a qual baseline?

Essa pergunta precisa estar respondida antes dos experimentos.

## 6. Pontos fortes do texto

Os principais pontos fortes são:

1. **Tema bem justificado social e academicamente**  
   O trabalho conecta câncer de mama, mamografia, IA e computação quântica de forma coerente.

2. **Lacuna científica identificável**  
   A comparação controlada entre CNN clássica e modelo híbrido em mamografia é apresentada como necessidade metodológica, não como mera aplicação de tecnologia nova.

3. **Hipótese cautelosa e verificável**  
   A hipótese não pressupõe superioridade da abordagem quântica e admite cenários de competitividade, limitação ou inviabilidade.

4. **Objetivos específicos com caráter operacional**  
   A lista de objetivos já indica etapas executáveis da pesquisa.

5. **Boa delimitação inicial**  
   A escolha de três classes evita que o escopo fique excessivamente amplo.

6. **Preocupação com reprodutibilidade**  
   O texto menciona protocolo controlado, mesma base, mesmo pré-processamento, mesmas métricas e mesmo ambiente computacional.

## 7. Fragilidades, lacunas ou ambiguidades

### 7.1 Falta uma pergunta de pesquisa destacada

O texto anuncia que haverá pergunta de pesquisa, mas ela não aparece claramente isolada. Isso deve ser corrigido.

### 7.2 A hipótese ainda depende de termos vagos

"Desempenho competitivo" e "viabilidade prática" precisam de definição operacional.

### 7.3 Objetivo geral ainda está um pouco amplo

A expressão "possibilidade de ampliação para uma classificação mais detalhada" aumenta o escopo. Para TCC1, eu recomendaria retirar essa parte do objetivo geral e colocar como trabalho futuro.

### 7.4 Falta explicitar critérios de exclusão metodológica

O texto delimita o que será feito, mas ainda não declara com força o que **não** será feito. Por exemplo:

- não será realizada validação clínica;
- não será feito diagnóstico médico;
- não será executado em hardware quântico real, se esse for o caso;
- não será proposta ferramenta hospitalar;
- não será feita inferência sobre pacientes reais;
- não será afirmada vantagem quântica ampla.

### 7.5 Falta definir unidade de análise

Do ponto de vista científico, este é um ponto crítico. A unidade de análise será:

- imagem individual?
- exame?
- mama?
- paciente?
- vista CC/MLO?

Sem isso, a metodologia pode ficar vulnerável.

### 7.6 Falta indicar controle de vieses

O trabalho menciona desbalanceamento e generalização, mas as seções avaliadas ainda poderiam antecipar riscos como:

- vazamento de dados;
- duplicidade de imagens;
- diferenças entre bases;
- distribuição desigual por origem;
- rótulos inconsistentes;
- classes minoritárias;
- avaliação enviesada por acurácia.

## 8. Sugestões concretas de melhoria

Minhas recomendações são:

1. **Inserir uma pergunta de pesquisa explícita**

   Sugestão:

   > Em um protocolo experimental controlado, uma arquitetura híbrida quântico-clássica baseada em circuitos quânticos simulados apresenta desempenho preditivo, estabilidade e custo computacional competitivos em relação a uma CNN clássica na classificação supervisionada de mamografias em três classes?

2. **Transformar a hipótese em hipótese operacional**

   Exemplo:

   > A hipótese será avaliada por meio de métricas preditivas, como AUC, F1-score e recall da classe maligna, e por métricas computacionais, como tempo de treinamento, uso de memória e variação entre execuções.

3. **Definir critério de competitividade**

   Exemplo:

   > Neste trabalho, um modelo será considerado competitivo quando apresentar desempenho estatisticamente próximo ao baseline clássico em métricas principais, sem custo computacional desproporcional.

4. **Retirar ampliação de classes do objetivo geral**

   Manter o foco em três classes e deixar ampliações como trabalho futuro.

5. **Adicionar uma subseção curta de contribuições esperadas**

   Sugestão de contribuições:

   - protocolo comparativo entre CNN clássica e modelo híbrido;
   - análise crítica de desempenho e custo;
   - avaliação de estabilidade experimental;
   - discussão sobre limitações de QML em imagens médicas;
   - base metodológica para estudos futuros.

6. **Adicionar delimitações negativas**

   Exemplo:

   > O trabalho não pretende realizar diagnóstico clínico, substituir especialistas, validar ferramenta médica ou demonstrar vantagem quântica ampla.

7. **Definir unidade de análise e divisão dos dados**

   Mesmo que os detalhes fiquem na metodologia, as delimitações devem indicar que a pesquisa buscará evitar vazamento de dados, preferencialmente separando por paciente ou exame quando os metadados permitirem.

8. **Prever análise de resultados negativos**

   O texto deveria dizer que resultados negativos ou inferiores do modelo híbrido serão interpretados como parte da contribuição científica, desde que analisados em termos de custo, estabilidade, escalabilidade e limitações de codificação.

## 9. Perguntas que uma banca real poderia fazer

1. Qual é a pergunta de pesquisa central do TCC?
2. Qual é a hipótese testável?
3. Como você saberá se a hipótese foi confirmada, parcialmente confirmada ou rejeitada?
4. O que significa "competitivo" no seu estudo?
5. Qual será a métrica principal?
6. Por que a acurácia não é suficiente para avaliar esse problema?
7. Qual é a unidade de análise: imagem, exame, mama ou paciente?
8. Como você evitará vazamento de dados?
9. Como será controlado o desbalanceamento entre classes?
10. Quantas execuções serão feitas para avaliar estabilidade?
11. Como serão tratados resultados negativos?
12. O que exatamente seu TCC contribui se o modelo híbrido for pior que a CNN?
13. Que parte do estudo é exploratória e que parte é confirmatória?
14. O trabalho é uma prova de conceito, um benchmark ou uma proposta de sistema?
15. Quais conclusões você não poderá tirar com esse desenho metodológico?

## Parecer parcial do professor de Pesquisa Científica

O TCC apresenta uma proposta relevante, atual e cientificamente defensável. A justificativa está bem estruturada, os objetivos específicos são operacionalizáveis e a hipótese é cautelosa. O trabalho tem potencial para produzir contribuição válida mesmo que o modelo híbrido não supere a CNN clássica, desde que os resultados sejam analisados de forma crítica e metodologicamente controlada.

As principais correções necessárias estão na formulação explícita da pergunta de pesquisa, na definição operacional de termos como "competitivo" e "viabilidade prática", na delimitação da unidade de análise, no controle de vieses e na definição prévia dos critérios de avaliação da hipótese.

**Meu parecer é favorável à continuidade, com ajustes metodológicos obrigatórios. O projeto é cientificamente viável, mas precisa transformar melhor sua proposta em um desenho de pesquisa verificável, reprodutível e criteriosamente delimitado.**

---

# Rodada 7 - Professor especialista em Matemática Avançada

## Avaliação individual

Como professor especialista em matemática avançada, minha avaliação se concentra na **formalização do problema**, na coerência entre hipótese e métricas, na definição matemática dos modelos, na escolha das funções de perda, na interpretação estatística dos resultados e na solidez dos critérios de comparação.

Minha avaliação geral é favorável, mas com uma ressalva importante: o TCC já demonstra preocupação matemática na revisão bibliográfica, especialmente na parte de métricas, perda, matriz de confusão, AUC e formulação de modelos híbridos. Porém, nas seções iniciais - Introdução, Contexto, Justificativa, Objetivos, Hipótese e Limitações - essa base matemática ainda não aparece com força suficiente para sustentar a comparação experimental.

## 1. Clareza do problema de pesquisa

O problema geral é compreensível: comparar CNNs clássicas e modelos híbridos quântico-clássicos na classificação de mamografias. A introdução afirma que a pesquisa avaliará desempenho preditivo, estabilidade, custo computacional e viabilidade prática em ambiente experimental controlado.

Do ponto de vista matemático, entretanto, a formulação ainda está verbal. Falta transformar o problema em uma formulação mais precisa:

> dado um conjunto de amostras rotuladas $D = \{(x_i, y_i)\}_{i=1}^{N}$, com $x_i$ representando uma mamografia e $y_i \in \{\text{Normal}, \text{Benign}, \text{Malignant}\}$, comparar duas famílias de funções parametrizadas, uma clássica e outra híbrida, segundo métricas preditivas e computacionais.

A revisão já apresenta a formulação supervisionada nesse espírito, definindo um conjunto de exemplos rotulados em que $x_i$ corresponde à imagem mamográfica e $y_i$ pertence ao conjunto de classes diagnósticas. O que falta é antecipar essa formalização no capítulo inicial, ainda que de modo breve.

Isso ajudaria bastante, porque a banca entenderia que a comparação não é apenas narrativa; ela será tratada como comparação entre funções, perdas, métricas e critérios de generalização.

## 2. Relevância do tema

A relevância está bem justificada. O texto mostra que o problema envolve imagens médicas, classes diagnósticas, desbalanceamento, custo computacional e confiabilidade. Também reconhece que modelos híbridos ainda são exploratórios em imagens médicas de alta dimensão.

Sob a ótica matemática, a relevância maior está em três dificuldades:

1. **alta dimensionalidade da entrada**;
2. **desbalanceamento e assimetria de custo entre erros**;
3. **comparação entre modelos com estruturas matemáticas diferentes**.

A primeira dificuldade é importante porque uma mamografia não é apenas uma "imagem"; ela é um vetor ou tensor de alta dimensão. Se a imagem tem $1024 \times 1024$ pixels em escala de cinza, ela possui mais de um milhão de entradas numéricas. O próprio trabalho reconhece essa dificuldade ao discutir que uma mamografia $1024 \times 1024$ possui 1.048.576 pixels e que a aplicação de modelos híbridos em imagens médicas de alta dimensão enfrenta desafios específicos.

A segunda dificuldade é crítica porque, em contexto médico, os erros não têm o mesmo peso. Um falso negativo para a classe maligna tem implicação diferente de um falso positivo. O texto já reconhece que, para a classe Malignant, a revocação é especialmente importante, pois baixa revocação significa muitos casos malignos classificados incorretamente como normais ou benignos.

A terceira dificuldade é talvez a mais importante para este TCC: comparar uma CNN clássica com uma arquitetura híbrida não é comparar apenas duas implementações. É comparar duas classes de funções com parametrizações, dimensões, custos e restrições distintas.

## 3. Qualidade da fundamentação matemática na parte apresentada

A fundamentação matemática geral do trabalho é promissora, mas sua conexão com as seções iniciais ainda precisa ser reforçada.

O texto já apresenta corretamente a ideia de minimização do risco empírico, com uma função de perda média sobre o conjunto de treinamento, e também apresenta a entropia cruzada categórica para classificação multiclasse. Isso é muito positivo. Também há formulação da matriz de confusão como uma matriz $C \in \mathbb{N}^{K \times K}$, em que cada elemento $C_{ij}$ representa a quantidade de exemplos cuja classe verdadeira é $i$ e cuja classe prevista é $j$.

Além disso, o trabalho discute que a acurácia pode ser insuficiente em bases desbalanceadas e que métricas como precisão, revocação, F1-score, matriz de confusão e AUC fornecem uma análise mais completa. Essa é uma base matemática adequada para um problema de classificação médica.

O ponto fraco é que a introdução, a hipótese e os objetivos ainda não dizem **qual métrica terá prioridade matemática na decisão**. O objetivo específico lista acurácia, precisão, recall, F1-score, AUC e matriz de confusão. Isso é adequado como conjunto de métricas, mas ainda falta hierarquia.

Como avaliador de matemática, eu perguntaria:

> Qual função objetivo treinará o modelo e qual métrica decidirá a comparação final?

Essas duas coisas não precisam ser iguais. O modelo pode ser treinado com entropia cruzada, mas escolhido por AUC macro, recall da classe maligna ou F1 macro. O TCC precisa deixar isso claro.

## 4. Coerência entre objetivos, hipótese e limitações

A coerência geral é boa. O objetivo geral afirma que o trabalho investigará comparativamente CNNs clássicas e modelos híbridos quântico-clássicos, considerando desempenho preditivo, custo computacional, estabilidade experimental e viabilidade prática.

Os objetivos específicos são compatíveis com essa formulação, especialmente ao incluir:

- definição da base e classes;
- protocolo de pré-processamento, divisão, treinamento, validação e teste;
- CNN clássica como referência;
- arquitetura híbrida compatível com limitações de simulação;
- investigação de qubits, feature map, profundidade e codificação;
- comparação por métricas;
- avaliação de tempo, memória, estabilidade e escalabilidade.

A hipótese também é adequada, porque declara que a arquitetura híbrida pode ter desempenho competitivo em relação à CNN clássica, mas sem pressupor superioridade geral da abordagem quântica. Ela também prevê que a viabilidade será condicionada por custo computacional, número de qubits, hiperparâmetros, codificação e restrições NISQ.

A principal fragilidade matemática está na palavra **competitivo**. Ela é qualitativa. Para virar hipótese testável, precisa ser operacionalizada.

Por exemplo, "competitivo" poderia significar:

- AUC macro com diferença menor que uma margem $\delta$ em relação à CNN;
- recall da classe maligna não inferior ao baseline clássico;
- F1 macro comparável, com custo computacional aceitável;
- desempenho médio próximo em múltiplas execuções, considerando desvio-padrão;
- ausência de degradação estatisticamente relevante em relação ao baseline clássico com gargalo equivalente.

Sem uma definição como essa, o resultado final pode ficar interpretativo demais.

## 5. Viabilidade matemática e estatística

A proposta é viável, mas precisa tratar melhor a variabilidade dos resultados.

Redes neurais não produzem um único resultado absoluto. Elas dependem de inicialização aleatória, embaralhamento dos dados, divisão treino/validação/teste, augmentation, otimizador, taxa de aprendizado, batch size e seeds. Modelos híbridos quânticos ainda acrescentam sensibilidade a número de qubits, profundidade, codificação e medições.

Portanto, um único treinamento por modelo não é suficiente para sustentar uma conclusão forte. O objetivo específico menciona "estabilidade entre execuções". Esse ponto deve ser levado a sério matematicamente.

A forma mais correta seria relatar:

- média;
- desvio-padrão;
- intervalo de confiança, se possível;
- melhor e pior execução;
- curva de treino e validação;
- matriz de confusão por melhor modelo e, se possível, agregada;
- comparação de custo computacional médio.

Também recomendo cuidado com "precisão média de 70%" mencionada no resumo. O resumo afirma que uma arquitetura anterior classificava três classes com cerca de 70% de precisão média. Esse dado precisa ser reescrito com rigor: era acurácia? precisão macro? média por classe? validação ou teste? Uma banca de matemática questionaria imediatamente essa ambiguidade.

## 6. Pontos fortes do texto

Os principais pontos fortes são:

1. **Boa consciência sobre métricas de classificação**  
   O trabalho reconhece que acurácia isolada é insuficiente em bases desbalanceadas e propõe matriz de confusão, precisão, recall, F1-score, acurácia balanceada e AUC.

2. **Reconhecimento da importância da classe maligna**  
   O texto percebe que falsos negativos em Malignant são especialmente graves.

3. **Formulação matemática já iniciada na revisão**  
   A revisão apresenta risco empírico, entropia cruzada, matriz de confusão, F1, AUC e formulação de modelos híbridos.

4. **Hipótese cautelosa**  
   A hipótese não força uma conclusão de superioridade quântica.

5. **Preocupação com estabilidade e custo computacional**  
   Isso torna o trabalho mais matematicamente comparável, desde que esses conceitos sejam medidos de modo objetivo.

6. **Boa formulação do modelo híbrido na revisão**  
   O texto descreve o fluxo matemático de um modelo híbrido: extração clássica $v = g_\phi(x)$, projeção $u = Wv + b$, codificação quântica, circuito variacional, valores esperados e saída softmax. Essa é uma das melhores partes matemáticas do trabalho e deveria dialogar mais com a introdução e os objetivos.

## 7. Fragilidades, lacunas ou ambiguidades

### 7.1 Métrica principal indefinida

A lista de métricas é boa, mas falta dizer qual decide a comparação. Para imagens médicas, eu não recomendaria acurácia como métrica principal.

### 7.2 "Competitivo" não está formalizado

O termo aparece na hipótese, mas sem margem, critério ou teste comparativo.

### 7.3 Falta plano estatístico mínimo

Não há indicação clara, nas seções iniciais, de quantas execuções serão feitas, como será medida a variabilidade e se haverá média/desvio-padrão.

### 7.4 Falta distinguir erro de treino, erro de validação e erro de teste

A revisão fala sobre generalização, mas a hipótese poderia deixar mais claro que a comparação final deve ser feita no conjunto de teste, não no treino.

### 7.5 Falta explicitar o tratamento do desbalanceamento

Se as classes forem balanceadas artificialmente, isso precisa ser dito. Se não forem, as métricas macro e balanceadas tornam-se ainda mais importantes.

### 7.6 Falta baseline matematicamente equivalente

Comparar CNN completa com CNN + circuito quântico não isola o efeito do circuito. É necessário comparar contra uma camada clássica com mesma dimensão de entrada/saída do bloco quântico.

### 7.7 O resumo está matematicamente impreciso

"Precisão de cerca de 70 por cento na média para as três classes" é uma frase ambígua. Precisa ser substituída por uma métrica bem definida.

## 8. Sugestões concretas de melhoria

Minha recomendação é incluir uma pequena formalização no final da introdução ou na transição para os objetivos:

> O problema será formulado como classificação supervisionada multiclasse, em que cada imagem $x_i$ é associada a um rótulo $y_i \in \{\text{Normal}, \text{Benign}, \text{Malignant}\}$. Os modelos serão treinados por minimização de uma função de perda de classificação e avaliados por métricas preditivas e computacionais em conjuntos separados de validação e teste.

Também recomendo definir uma hierarquia de métricas:

| Papel | Métrica recomendada |
|---|---|
| Métrica principal | AUC macro ou AUC one-vs-rest média |
| Métrica clínica crítica | Recall da classe Malignant |
| Métrica de equilíbrio | F1 macro ou balanced accuracy |
| Métrica diagnóstica complementar | Matriz de confusão |
| Métrica secundária | Acurácia |
| Métricas computacionais | tempo, memória, número de parâmetros, custo por época |

Além disso, recomendo definir "competitividade" previamente:

> Será considerado competitivo o modelo cuja métrica principal permaneça dentro de uma margem previamente definida em relação ao baseline clássico, desde que não apresente degradação relevante no recall da classe maligna nem custo computacional desproporcional.

Para estabilidade, sugiro:

> Cada configuração será executada múltiplas vezes com sementes diferentes, e os resultados serão reportados por média e desvio-padrão.

E para a comparação com o componente quântico:

> Será incluído um baseline clássico com gargalo de mesma dimensão da entrada/saída do circuito quântico, a fim de isolar se eventuais ganhos decorrem do bloco quântico ou apenas da redução dimensional.

## 9. Perguntas que uma banca real poderia fazer

1. Qual é a formulação matemática exata do problema de classificação?
2. Qual função de perda será minimizada?
3. A saída do modelo será softmax? Como as probabilidades serão interpretadas?
4. Qual será a métrica principal para comparar CNN e modelo híbrido?
5. Por que acurácia não basta?
6. O que significa "competitivo" matematicamente?
7. Qual margem de diferença será aceitável entre os modelos?
8. Quantas execuções serão feitas para calcular estabilidade?
9. Você reportará média e desvio-padrão?
10. Como será avaliado o recall da classe maligna?
11. Como a matriz de confusão será interpretada?
12. Haverá AUC one-vs-rest para cada classe?
13. Como você tratará classes desbalanceadas?
14. Como diferenciará overfitting de boa generalização?
15. Como saberá se o circuito quântico contribuiu mais do que uma camada clássica equivalente?
16. O custo computacional será normalizado por época, por amostra ou por treinamento completo?
17. A comparação será feita no conjunto de validação ou no conjunto de teste?
18. Como evitar conclusões baseadas em uma única execução favorável?

## Parecer parcial do professor de Matemática Avançada

O trabalho apresenta uma boa base conceitual e já contém elementos matemáticos relevantes, especialmente na revisão de métricas, função de perda, matriz de confusão, AUC, F1-score e modelos híbridos. A hipótese é cautelosa e coerente, mas ainda precisa ser transformada em uma hipótese operacional mensurável.

A maior fragilidade matemática está na ausência de uma métrica principal, de uma definição formal de "competitividade" e de um plano mínimo para tratar variabilidade experimental. Sem esses elementos, o resultado final pode depender demais de interpretação qualitativa.

**Meu parecer é favorável à continuidade, com ajustes obrigatórios na formalização matemática do problema, na hierarquia das métricas, na definição de critérios de comparação e no tratamento estatístico das execuções.**

---

# Parecer final consolidado da banca

**Relator:** Professor especialista em Pesquisa Científica  
**Escopo avaliado:** Introdução, Contexto, Justificativa, Objetivos, Hipótese e Delimitações.

## 1. Resumo geral da avaliação

A banca considera que o TCC apresenta uma proposta **relevante, atual e viável**, com bom potencial acadêmico para continuidade no TCC2. O tema articula três campos de alta relevância: **visão computacional médica**, **redes neurais convolucionais** e **modelos híbridos quântico-clássicos** aplicados à classificação de mamografias.

O texto deixa claro que o trabalho pretende comparar uma arquitetura clássica baseada em CNN com uma arquitetura híbrida quântico-clássica, avaliando não apenas desempenho preditivo, mas também estabilidade, custo computacional e viabilidade prática em ambiente experimental controlado. Esse enquadramento é positivo, pois afasta a proposta de uma simples aplicação de IA e aproxima o TCC de um estudo experimental comparativo.

A justificativa está bem estruturada ao apresentar relevância social, acadêmica e científica. O texto reconhece que o aprendizado profundo já é consolidado em visão computacional, enquanto modelos híbridos quântico-clássicos ainda carecem de validação comparativa rigorosa em aplicações médicas. Também identifica uma lacuna relevante: estudos de deep learning em mamografia apresentam limitações de reprodutibilidade e avaliação realista, enquanto trabalhos quânticos ainda dependem de bases menores, simulação e cenários restritos.

A hipótese é um dos pontos mais fortes do trabalho. Ela é cautelosa e metodologicamente adequada, pois não assume superioridade geral da abordagem quântica. Em vez disso, propõe investigar em quais condições o modelo híbrido pode ser competitivo, limitado ou inviável em comparação com CNNs clássicas.

O parecer consolidado da banca é: **projeto aprovado para continuidade, com ajustes metodológicos obrigatórios antes do TCC2**.

## 2. Principais pontos fortes

### 2.1 Tema relevante e interdisciplinar

O trabalho aborda um problema de relevância social - o câncer de mama - e o conecta a uma investigação computacional atual. A escolha da mamografia como domínio de aplicação é adequada, pois o próprio texto reconhece que esse exame envolve achados sutis, como massas, microcalcificações, assimetrias e distorções arquiteturais, nem sempre facilmente distinguíveis do tecido normal.

### 2.2 Boa postura científica sobre computação quântica

A banca considera muito positivo que o trabalho **não prometa vantagem quântica definitiva**. A hipótese reconhece limitações atuais da computação quântica e da simulação de circuitos, incluindo custo computacional, número reduzido de qubits, sensibilidade a hiperparâmetros, estratégia de codificação e restrições NISQ.

Essa cautela aumenta a credibilidade do projeto.

### 2.3 Objetivos específicos bem direcionados

Os objetivos específicos já indicam etapas executáveis: definir base e classes, preparar protocolo de pré-processamento, treinar CNN clássica, projetar arquitetura híbrida, investigar qubits, feature map, profundidade e codificação, comparar métricas e avaliar tempo, memória, estabilidade e escalabilidade.

Essa estrutura é adequada para um TCC experimental.

### 2.4 Delimitação inicial coerente

O trabalho delimita a tarefa como classificação supervisionada de mamografias em três classes: **normal, benigno e maligno**. Também propõe comparar CNN clássica e arquitetura híbrida mantendo constantes base de dados, pré-processamento, divisão dos dados e métricas de avaliação.

Esse recorte é viável e adequado para TCC2.

### 2.5 Boa base matemática e computacional já presente no texto

Embora a avaliação tenha focado nas seções iniciais, a banca observou que a revisão já apresenta formulações úteis para sustentar o trabalho, como a representação supervisionada $D = \{(x_i, y_i)\}$, a definição de classes, a função parametrizada do modelo e a saída por softmax. Isso deve ser melhor conectado à introdução e à hipótese.

## 3. Principais pontos fracos

### 3.1 Pergunta de pesquisa ainda pouco explícita

O texto afirma que o capítulo apresenta a pergunta de pesquisa, mas ela não aparece de forma destacada. A banca recomenda inserir uma pergunta clara, objetiva e operacional.

Sugestão:

> **Em um protocolo experimental controlado, uma arquitetura híbrida quântico-clássica baseada em circuitos quânticos simulados apresenta desempenho preditivo, estabilidade e custo computacional competitivos em relação a uma CNN clássica na classificação supervisionada de mamografias em três classes?**

Essa pergunta conecta tema, método, métrica e hipótese.

### 3.2 O termo "competitivo" ainda é vago

A hipótese afirma que o modelo híbrido pode apresentar desempenho competitivo. Isso é aceitável como ideia inicial, mas precisa de definição operacional.

A banca recomenda definir previamente o que será considerado competitivo. Por exemplo:

- AUC macro próxima à CNN clássica;
- recall da classe maligna não inferior ao baseline;
- F1 macro dentro de uma margem aceitável;
- custo computacional não desproporcional;
- estabilidade semelhante entre execuções.

Sem esse critério, a conclusão pode ficar subjetiva.

### 3.3 Falta definição de métrica principal

O trabalho lista acurácia, precisão, recall, F1-score, AUC e matriz de confusão. A lista é adequada, mas falta hierarquia.

Para imagens médicas, a banca não recomenda usar **acurácia** como métrica principal. A sugestão é:

| Função | Métrica recomendada |
|---|---|
| Métrica principal | AUC macro ou AUC one-vs-rest |
| Métrica clínica crítica | Recall da classe maligna |
| Métrica de equilíbrio | F1 macro ou balanced accuracy |
| Métrica complementar | Matriz de confusão |
| Métrica secundária | Acurácia |

### 3.4 Unidade experimental indefinida

A banca identificou uma lacuna metodológica importante: o texto ainda não define claramente se a amostra será:

- imagem individual;
- mama;
- exame;
- paciente;
- vista CC/MLO;
- conjunto de imagens por paciente.

Essa definição é essencial para evitar interpretações ambíguas e riscos de vazamento de dados.

### 3.5 Risco de vazamento de dados

Em mamografia, é metodologicamente crítico evitar que imagens da mesma paciente, do mesmo exame ou de exames correlacionados apareçam simultaneamente em treino e teste.

A banca recomenda incluir já nas delimitações:

> A divisão dos dados buscará evitar vazamento entre treino, validação e teste, priorizando separação por paciente ou por exame quando os metadados permitirem.

### 3.6 Componente quântico ainda precisa ser mais especificado

O texto menciona circuitos quânticos simulados como componente treinável complementar. Porém, para TCC2 será necessário definir:

- tipo de codificação dos dados clássicos;
- número de qubits;
- ansatz variacional;
- profundidade do circuito;
- uso ou não de emaranhamento;
- observáveis medidos;
- uso de statevector, shots ou simulador ruidoso;
- treinamento conjunto ou separado da CNN;
- baseline clássico equivalente.

Sem esses detalhes, "modelo híbrido quântico-clássico" permanece amplo demais.

### 3.7 Escopo levemente excessivo no objetivo geral

O objetivo geral menciona "possibilidade de ampliação para uma classificação mais detalhada". A banca recomenda retirar essa parte do objetivo central.

A classificação em três classes já é suficientemente desafiadora para TCC2. A ampliação pode aparecer como **trabalho futuro**.

## 4. Mudanças recomendadas

### 4.1 Reescrever a pergunta de pesquisa

Inserir uma pergunta objetiva após a justificativa ou antes dos objetivos.

Versão sugerida:

> **Este trabalho busca responder se, em uma tarefa controlada de classificação de mamografias em três classes, uma arquitetura híbrida quântico-clássica baseada em circuitos simulados apresenta desempenho preditivo, estabilidade e custo computacional competitivos em relação a uma CNN clássica.**

### 4.2 Ajustar o objetivo geral

Versão sugerida:

> **Investigar comparativamente o desempenho de uma CNN clássica e de uma arquitetura híbrida quântico-clássica simulada na classificação supervisionada de mamografias em três classes - normal, benigno e maligno - considerando métricas preditivas, estabilidade experimental, custo computacional e viabilidade prática.**

Remover a ampliação para classificação mais detalhada do objetivo geral.

### 4.3 Reformular a hipótese de modo mais operacional

A hipótese atual é boa, mas pode ficar mais objetiva:

> **Parte-se da hipótese de que uma arquitetura híbrida quântico-clássica, composta por extração clássica de características, projeção dimensional e circuito quântico variacional simulado, pode apresentar desempenho competitivo em relação a uma CNN clássica em métricas como AUC macro, F1 macro e recall da classe maligna. Contudo, espera-se que sua viabilidade seja limitada por custo de simulação, número de qubits, estratégia de codificação, estabilidade de treinamento e escalabilidade.**

### 4.4 Incluir delimitações negativas

Adicionar explicitamente que o trabalho:

- não pretende realizar diagnóstico clínico;
- não substitui especialistas;
- não valida uma ferramenta médica;
- não demonstra vantagem quântica ampla;
- não executa necessariamente em hardware quântico real;
- não pretende generalizar resultados para todos os cenários de mamografia.

### 4.5 Criar critérios de avaliação da hipótese

Antes dos experimentos, definir:

- métrica principal;
- métrica crítica para malignidade;
- margem de competitividade;
- número mínimo de execuções;
- critério de estabilidade;
- critério de custo computacional;
- baseline clássico equivalente ao modelo híbrido.

## 5. Ajustes prioritários antes do TCC2

A banca recomenda priorizar os ajustes nesta ordem:

### Prioridade 1 - Formalização do problema

Definir claramente:

- pergunta de pesquisa;
- hipótese operacional;
- unidade experimental;
- tarefa exata;
- classes utilizadas.

### Prioridade 2 - Protocolo experimental

Especificar:

- divisão treino/validação/teste;
- critério para evitar leakage;
- balanceamento ou ponderação de classes;
- seeds;
- número de execuções;
- ambiente computacional;
- critério de escolha do melhor checkpoint.

### Prioridade 3 - Métricas e critérios de decisão

Definir:

- métrica principal;
- recall da classe maligna como métrica crítica;
- F1 macro ou balanced accuracy;
- matriz de confusão;
- AUC one-vs-rest;
- tempo de treinamento;
- uso de memória;
- estabilidade entre execuções.

### Prioridade 4 - Baselines justos

A banca recomenda, no mínimo, três modelos:

| Modelo | Função |
|---|---|
| CNN clássica completa | baseline principal |
| CNN com gargalo clássico equivalente | controle da redução dimensional |
| CNN + circuito quântico simulado | modelo híbrido proposto |

Esse baseline intermediário é essencial para verificar se o circuito quântico agrega algo além de uma camada densa ou de um gargalo regularizador.

### Prioridade 5 - Especificação do circuito quântico

Definir:

- número de qubits;
- feature map;
- ansatz;
- portas de emaranhamento;
- profundidade;
- observáveis;
- backend;
- uso de shots ou statevector;
- estratégia de treinamento.

### Prioridade 6 - Reescrita do resumo

O resumo atual usa linguagem ainda informal, como "além do chute aleatório" e "precisão de cerca de 70 por cento na média". A banca recomenda reescrever em tom acadêmico, substituindo por termos como:

- desempenho basal;
- classificação multiclasse;
- protocolo comparativo;
- métricas preditivas;
- estabilidade;
- custo computacional;
- limitações de simulação.

## 6. Parecer final sobre a continuidade do projeto

A banca emite parecer **favorável à continuidade do TCC para o TCC2**, com ressalvas metodológicas.

O projeto é adequado para um curso de Ciência da Computação, possui boa relevância social e acadêmica, e demonstra potencial de contribuição científica. A proposta é especialmente forte porque não se limita a buscar alta acurácia, mas pretende analisar desempenho, custo, estabilidade e viabilidade de uma abordagem híbrida em comparação com CNNs clássicas.

Entretanto, a continuidade deve estar condicionada a ajustes antes da execução experimental. O aluno precisa transformar melhor a proposta em um desenho de pesquisa verificável, com pergunta explícita, hipótese operacional, métrica principal, unidade experimental definida, prevenção de vazamento de dados e baseline clássico equivalente.

## Parecer consolidado

**Aprovado para continuidade, com ajustes obrigatórios.**

A banca considera que o trabalho tem mérito acadêmico e viabilidade técnica, desde que o TCC2 mantenha o foco em uma comparação experimental controlada e não extrapole conclusões sobre uso clínico ou vantagem quântica. O resultado será cientificamente válido mesmo que o modelo híbrido não supere a CNN clássica, desde que as limitações sejam medidas, discutidas e relacionadas a custo, escalabilidade, estabilidade e codificação dos dados.
