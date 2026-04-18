# Revisao critica do TCC

Data da revisao: 2026-04-17

Escopo analisado:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, que parece ser o rascunho mais recente porque tem alteracao nao commitada e uma secao nova de hipotese.
- `meu-tcc/tcc_matheus.tex`, que tem uma estrutura mais limpa e pode servir como referencia para reorganizacao.
- `meu-tcc/anotacoes/anotacoes-introducao.tex` e `meu-tcc/anotacoes/anotacoes-revi-bibli.tex`, que parecem conter partes preparatorias do texto.
- PDF de Raul Wazlawick, `Metodologia de Pesquisa para Ciencia da Computacao`, usado aqui como base metodologica.

Observacao importante: esta anotacao nao altera o seu TCC. Ela aponta problemas, riscos e caminhos de melhoria.

## Diagnostico geral

O tema e forte: comparar CNNs classicas com modelos hibridos quantico-classicos em mamografias e um recorte atual, com relevancia em Ciencia da Computacao e aplicacao em saude. O texto tambem ja tem bons elementos: revisao recente, preocupacao com reprodutibilidade, metricas de avaliacao e consciencia das limitacoes da computacao quantica atual.

O principal problema hoje nao e falta de assunto. E excesso de pecas ainda soltas. O rascunho mistura proposta, revisao bibliografica, referencial teorico, metodologia bibliografica e metodologia experimental sem deixar uma linha de raciocinio unica. Para a banca, isso pode parecer que o trabalho ainda nao sabe exatamente qual problema vai responder.

A melhoria mais importante e transformar o trabalho de "vou melhorar modelos" para "vou testar uma hipotese verificavel por meio de um protocolo experimental controlado".

## Pontos criticos e como corrigir

### 1. A estrutura do rascunho esta fragmentada e duplicada

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`: capitulos em `Introducao`, `Contexto`, `Justificativa`, `Objetivo`, `hipotese`, `Revisao bibliografica`, `Referencial teorico`, `Metodologia da pesquisa bibliografica` e `Desenvolvimento`.
- `meu-tcc/tcc_matheus.tex`: estrutura mais enxuta, com `Introducao`, `Revisao Bibliografica` e `Desenvolvimento`.

O problema:

No rascunho mais recente, `Contexto`, `Justificativa`, `Objetivo` e `hipotese` aparecem como capitulos separados. Para uma proposta de TCC1, esses elementos normalmente funcionam melhor dentro da Introducao. Alem disso, `Revisao bibliografica` e `Referencial teorico` estao muito parecidos e repetem assuntos.

Por que isso enfraquece o artigo:

A banca pode ter dificuldade para encontrar o problema, a pergunta de pesquisa e a contribuicao. Wazlawick reforca que objetivo, justificativa, metodo e revisao devem girar em torno do problema de pesquisa. Quando cada coisa aparece como um capitulo independente, o texto perde unidade.

Como melhorar:

Use a estrutura de `tcc_matheus.tex` como base, mas aproveite o conteudo mais rico de `tcc_math.tex`.

Estrutura sugerida:

```text
1 Introducao
  1.1 Contextualizacao
  1.2 Problema de pesquisa
  1.3 Justificativa
  1.4 Pergunta de pesquisa
  1.5 Hipotese
  1.6 Objetivos
  1.7 Limitacoes iniciais
  1.8 Organizacao do trabalho

2 Revisao bibliografica
  2.1 Mamografia e classificacao de cancer de mama
  2.2 CNNs em mamografia
  2.3 Bases de dados e benchmarks
  2.4 Modelos hibridos quantico-classicos
  2.5 Trabalhos relacionados
  2.6 Lacuna de pesquisa

3 Metodologia / Solucao proposta
  3.1 Tipo de pesquisa
  3.2 Base de dados
  3.3 Pre-processamento
  3.4 Modelos comparados
  3.5 Protocolo experimental
  3.6 Metricas
  3.7 Reprodutibilidade
  3.8 Riscos e limitacoes
  3.9 Cronograma
```

### 2. A hipotese esta vazia

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, capitulo `\chapter{hipótese}`.

O problema:

Existe o capitulo, mas ele ainda nao tem conteudo. Isso e grave porque o seu trabalho e comparativo e experimental. Sem hipotese, o leitor nao sabe exatamente o que os experimentos vao tentar confirmar, refutar ou esclarecer.

Como melhorar:

Escreva a hipotese de forma testavel e mensuravel. Evite uma hipotese vaga como "o modelo quantico sera melhor". Para o seu caso, uma hipotese mais madura seria:

```text
Hipotese principal:
Modelos hibridos quantico-classicos podem apresentar desempenho preditivo comparavel ao de CNNs classicas na classificacao multiclasse de mamografias, mas tendem a apresentar maior custo computacional e maior sensibilidade a configuracoes de circuito e hiperparametros.
```

Se quiser formular de modo estatistico:

```text
H0: Nao ha diferenca estatisticamente significativa entre o desempenho da CNN classica e o modelo hibrido quantico-classico nas metricas macro-F1 e AUC macro, sob o mesmo protocolo experimental.

H1: Ha diferenca estatisticamente significativa entre os modelos nas metricas macro-F1 e AUC macro, sob o mesmo protocolo experimental.
```

Se a sua intencao for mostrar "comparavel", nao "superior", considere tratar como estudo de equivalencia ou nao inferioridade. Isso combina muito bem com a ideia de que o modelo quantico talvez nao ganhe em acuracia, mas pode revelar limites e trade-offs.

### 3. O objetivo geral esta bom, mas ainda amplo demais

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, objetivo principal.
- `meu-tcc/tcc_matheus.tex`, objetivo principal.

O problema:

O objetivo fala em desempenho preditivo, custo computacional, estabilidade experimental, viabilidade pratica, tres classes e possivel ampliacao para mais classes. Isso e interessante, mas pode ficar grande demais para TCC1/TCC2, principalmente porque modelos quanticos simulados ja sao custosos.

Como melhorar:

Deixe o objetivo geral mais fechado:

```text
Avaliar, em uma tarefa multiclasse de classificacao de mamografias nas classes Normal, Benigno e Maligno, se um modelo hibrido quantico-classico apresenta desempenho preditivo comparavel ao de uma CNN classica sob o mesmo protocolo experimental, considerando macro-F1, AUC macro, custo computacional e estabilidade entre execucoes.
```

Deixe a ampliacao para mais classes como possibilidade futura ou objetivo condicionado:

```text
Como analise complementar, investigar a viabilidade de ampliar a classificacao para maior granularidade caso a base selecionada apresente rotulos suficientes e confiaveis.
```

### 4. Os objetivos secundarios parecem etapas do metodo

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, lista de objetivos secundarios.

O problema:

Itens como "aprimorar a arquitetura", "estabelecer protocolo", "comparar metricas" e "avaliar custo" estao proximos de etapas do metodo. Wazlawick alerta que objetivos especificos nao devem ser apenas passos de execucao; eles devem ser subprodutos verificaveis do objetivo principal.

Tambem ha um erro textual direto:

- O item "Aprimorar a arquitetura classica de CNN para servir como;" esta incompleto.

Como melhorar:

Reescreva como subprodutos verificaveis:

```text
\begin{enumerate}
    \item Caracterizar a base de dados escolhida quanto a numero de imagens, classes, distribuicao dos rotulos e limitacoes de uso;
    \item Definir um baseline classico de CNN e medir seu desempenho sob um protocolo experimental reproduzivel;
    \item Definir um modelo hibrido quantico-classico compativel com as restricoes de simulacao e medir seu desempenho sob o mesmo protocolo;
    \item Comparar os modelos por macro-F1, AUC macro, acuracia balanceada, matriz de confusao, tempo de treinamento e tempo de inferencia;
    \item Analisar se eventuais diferencas de desempenho justificam o custo computacional adicional do modelo hibrido;
    \item Identificar limitacoes praticas da abordagem hibrida para classificacao de mamografias.
\end{enumerate}
```

As atividades de implementar, ajustar hiperparametros e treinar modelos entram na metodologia, nao precisam ser objetivos.

### 5. O resumo esta informal e nao vende bem a contribuicao

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, resumo.

Problemas encontrados:

- Usa linguagem informal: "chute aleatorio".
- Tem erros de acentuacao e digitacao: "cancer", "precisao", "media", "classico", "clasificar", "radiograficos".
- Fala que "deve ser feito", mas nao apresenta claramente problema, metodo, contribuicao e resultados esperados.
- Foca em "melhorar arquitetura" sem explicar o criterio cientifico de melhoria.

Como melhorar:

Para TCC1, o resumo pode apresentar proposta e resultado esperado, sem fingir que os experimentos ja foram concluidos:

```text
Este trabalho propoe um estudo experimental comparativo entre redes neurais convolucionais classicas e modelos hibridos quantico-classicos para a classificacao de mamografias nas classes Normal, Benigno e Maligno. O problema de pesquisa consiste em avaliar se a inclusao de componentes quanticos oferece desempenho preditivo comparavel ao de uma CNN classica quando ambos os modelos sao treinados e testados sob o mesmo protocolo experimental. A pesquisa sera conduzida com base em uma base publica de mamografias, com pre-processamento padronizado, particionamento controlado dos dados e avaliacao por metricas como macro-F1, AUC macro, acuracia balanceada, matriz de confusao, tempo de treinamento e estabilidade entre execucoes. Espera-se produzir uma analise reprodutivel sobre as vantagens, limitacoes e custos computacionais da abordagem hibrida em relacao ao baseline classico, contribuindo para a discussao sobre o uso de aprendizado de maquina quantico em tarefas de visao computacional medica.
```

Depois dos resultados reais, troque "sera conduzida" e "espera-se" por resultados obtidos.

### 6. Falta uma metodologia experimental completa

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, capitulo `Metodologia da pesquisa bibliografica`.
- `meu-tcc/tcc_matheus.tex`, secao `Metodologia da pesquisa bibliografica` e secao `Fundamentos`.

O problema:

O texto descreve como sera feita a pesquisa bibliografica, mas o coracao do seu TCC e experimental. A banca vai querer saber exatamente como a comparacao sera feita.

Como melhorar:

Crie uma secao chamada `Metodo de pesquisa` ou `Metodologia experimental`. Ela deve responder:

- Qual base sera usada?
- Quantas imagens existem em cada classe?
- A divisao treino/validacao/teste sera por imagem ou por paciente? Em saude, o ideal e por paciente para evitar vazamento de dados.
- Quais pre-processamentos serao aplicados?
- Quais modelos serao comparados?
- Como os hiperparametros serao escolhidos?
- Quantas repeticoes com sementes diferentes serao feitas?
- Quais metricas serao usadas?
- Como sera avaliado custo computacional?
- Havera teste estatistico?
- Como garantir reprodutibilidade?

Modelo de roteiro:

```text
A pesquisa sera experimental e comparativa. Sera utilizada uma base publica de mamografias, inicialmente organizada nas classes Normal, Benigno e Maligno. As imagens passarao por padronizacao de tamanho, normalizacao de intensidade e tratamento de desbalanceamento quando necessario. Os dados serao divididos em treino, validacao e teste, preferencialmente por paciente, evitando que imagens da mesma paciente aparecam em mais de uma particao.

Serao comparados dois modelos: uma CNN classica usada como baseline e um modelo hibrido quantico-classico com numero limitado de qubits, adequado a simulacao disponivel. Ambos serao avaliados sob as mesmas particoes, metricas e condicoes de execucao. Os experimentos serao repetidos com diferentes sementes aleatorias para estimar estabilidade. As metricas principais serao macro-F1 e AUC macro, complementadas por acuracia balanceada, matriz de confusao, tempo de treinamento, tempo de inferencia e consumo aproximado de recursos computacionais.
```

### 7. A solucao proposta e o desenvolvimento estao vazios no rascunho mais recente

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, `\chapter{Desenvolvimento}`, `\section{Solução proposta}` e `\section{Cronograma de trabalho}`.

O problema:

Essas secoes ainda nao tem conteudo. Isso passa a impressao de que o trabalho esta forte na revisao, mas fraco no plano de execucao.

Como melhorar:

Reaproveite a secao de solucao proposta e o cronograma que ja aparecem em `meu-tcc/tcc_matheus.tex`. Esse arquivo tem uma versao mais completa de:

- solucao proposta;
- pergunta de pesquisa;
- hipotese inicial;
- plano de validacao;
- riscos e limitacoes;
- cronograma em Gantt.

Sugestao pratica: usar `tcc_matheus.tex` como "esqueleto" e inserir nele os paragrafos mais ricos da introducao/revisao de `tcc_math.tex`.

### 8. Ha citacoes em formato manual que devem virar citacoes LaTeX

Onde aparece:

- Na introducao de `meu-tcc/primeiras-entregas/tcc_math.tex`, varios trechos usam "(Autor et al., ano)" em texto puro.
- Exemplos: Abdelhafiz, Elias-Cabot, Szegedy, Wu, Pesapane, Camurdan, Yoshitsugu, Bhole, Schetakis, Watkins, Long, Daka e Egginger.

O problema:

Quando voce escreve "(Wu et al., 2020)" manualmente, o BibTeX nao controla a referencia naquele ponto. Isso prejudica padronizacao ABNT e pode deixar referencias fora do controle automatico.

Como melhorar:

Troque por comandos ABNT:

```latex
\citeonline{wu2020}
\cite{wu2020}
```

Exemplo:

```latex
Segundo \citeonline{wu2020}, ...
```

ou:

```latex
... conforme observado em estudos recentes \cite{wu2020,eliascabot2024}.
```

Ponto extra: `Pesapane et al. (2023)` aparece na introducao, mas nao encontrei entrada `pesapane2023` nos arquivos `.bib` analisados. Adicione a referencia ou remova esse autor ate ter o BibTeX correto.

### 9. Cuidado com arquivos `.bib` diferentes

Onde aparece:

- `meu-tcc/tcc_matheus.tex` usa `bibliografia_matheus`.
- `meu-tcc/primeiras-entregas/tcc_math.tex` usa `bibliografia`.
- `meu-tcc/anotacoes/anotacoes-revi-bibli.tex` usa chaves que tambem aparecem em `anotacoes.bib`.

O problema:

Se voce copiar texto entre os arquivos, algumas citacoes podem quebrar dependendo do `.bib` associado. O rascunho `tcc_math.tex` esta melhor nesse ponto porque `primeiras-entregas/bibliografia.bib` contem tanto as referencias antigas quanto as novas. Ja `bibliografia_matheus.bib` e mais curto.

Como melhorar:

Escolha um unico arquivo `.bib` principal para o TCC e concentre as referencias nele. Minha sugestao:

- Se o arquivo final for `meu-tcc/primeiras-entregas/tcc_math.tex`, mantenha `meu-tcc/primeiras-entregas/bibliografia.bib` como base.
- Se o arquivo final for `meu-tcc/tcc_matheus.tex`, copie para `bibliografia_matheus.bib` todas as referencias novas de `primeiras-entregas/bibliografia.bib`.

Evite manter a mesma referencia com duas chaves diferentes, como `Bhole2025MammoBench` e `bhole2025`, a menos que haja um motivo claro.

### 10. O problema de pesquisa precisa ficar mais explicito

Onde aparece:

- A ideia aparece espalhada na introducao, contexto, justificativa e sintese da revisao.

O problema:

O leitor entende que voce quer comparar CNNs classicas e modelos hibridos, mas a formulacao do problema ainda pode ficar mais direta. Em Wazlawick, um problema de pesquisa precisa deixar claro:

- qual questao sera tratada;
- como a bibliografia mostra que ela ainda nao foi suficientemente resolvida;
- por que vale a pena tratar essa questao.

Como melhorar:

Inclua uma subseccao `Problema de pesquisa` na Introducao:

```text
Embora CNNs classicas ja apresentem resultados relevantes em mamografia, os modelos hibridos quantico-classicos ainda possuem evidencias limitadas, muitas vezes baseadas em bases pequenas, tarefas simplificadas ou simulacoes. Assim, ainda nao esta claro se a inclusao de componentes quanticos traz ganho mensuravel, desempenho comparavel ou apenas aumento de custo computacional em uma tarefa realista de classificacao mamografica. O problema deste trabalho e avaliar essa relacao em um protocolo controlado, usando as mesmas classes, particoes, metricas e condicoes experimentais para os dois tipos de modelo.
```

Depois disso, coloque a pergunta:

```text
Modelos hibridos quantico-classicos apresentam desempenho preditivo comparavel ao de CNNs classicas na classificacao de mamografias em Normal, Benigno e Maligno quando avaliados sob o mesmo protocolo experimental?
```

### 11. O escopo pode estar grande demais

Onde aparece:

- Objetivo geral fala em tres classes e possibilidade de maior granularidade.
- Revisao bibliografica fala de IA clinica, ROI, anotacao, explicabilidade, controle de qualidade, QML, kernels, reforco quantico e quantizacao.

O problema:

O trabalho pode ficar com cara de "quero falar de tudo". Isso e perigoso porque o TCC precisa concluir algo verificavel. Computacao quantica simulada ja pode limitar tamanho de imagem, numero de qubits, batch size e tempo de treino.

Como melhorar:

Defina o nucleo obrigatorio:

- Tarefa: classificacao Normal / Benigno / Maligno.
- Dataset: uma base principal, preferencialmente Mammo-Bench se for viavel.
- Modelos: uma CNN classica e um modelo hibrido.
- Metricas: macro-F1 e AUC macro como principais; custo computacional e estabilidade como complementares.

Defina como fora de escopo ou futuro:

- uso clinico real;
- diagnostico medico;
- muitas arquiteturas classicas;
- muitas arquiteturas quanticas;
- classificacao com mais classes, se nao houver tempo ou rotulos confiaveis;
- explicabilidade profunda, se nao for parte central do objetivo.

### 12. A revisao bibliografica tem trabalhos bons, mas precisa ser mais seletiva

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, revisao bibliografica.
- `meu-tcc/anotacoes/anotacoes-revi-bibli.tex`, revisao preparatoria.

Pontos fortes:

- Abdelhafiz, Bhalla, Wu, Elias-Cabot, Bhole/Mammo-Bench, Long, Daka, Gupta e Egginger ajudam a sustentar o tema.
- A sintese sobre lacuna entre maturidade das CNNs e carater exploratorio do QML esta no caminho certo.

Pontos fracos:

- Kugelman/OCT, Sundell/controle de qualidade, Dalla Pozza/labirinto e Zandieh/TurboQuant parecem laterais demais para o foco atual.
- Esses trabalhos so devem ficar se voce explicar exatamente por que eles sao necessarios para o argumento.

Como melhorar:

Organize a revisao em torno da pergunta do TCC:

1. O que ja sabemos sobre CNNs em mamografia?
2. Quais bases e protocolos sao usados?
3. O que falta em reprodutibilidade e comparacao justa?
4. O que QML/hibrido promete?
5. Quais limitacoes atuais impedem alegar vantagem pratica?
6. Qual lacuna exatamente o seu experimento vai atacar?

Sugestao de tabela obrigatoria:

```text
Autor/ano | Tipo de estudo | Base/tarefa | Modelo | Metricas | Limitacao | Como ajuda este TCC
```

Essa tabela vai deixar a lacuna muito mais convincente.

### 13. A linguagem precisa ficar mais academica e padronizada

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex`, resumo.
- `meu-tcc/anotacoes/anotacoes-revi-bibli.tex`, primeiros paragrafos.

Problemas diretos:

- "chute aleatorio" deve virar "desempenho proximo ao acaso" ou "desempenho inferior ao baseline".
- "estado da arte + tratamento de dados criado" deve virar "baseline representativo" ou "protocolo de pre-processamento proposto".
- "classico conseguir clasificar mais exames radiograficos" deve ser reescrito com precisao, porque mamografia nao deve ser chamada genericamente de exame radiografico no objetivo.
- "a principio", "princio", "arquigos", "cdataset", "otimizacao", "pre treinamento" precisam de revisao.

Como melhorar:

Use linguagem impessoal:

```text
Este trabalho avalia...
Este estudo compara...
Pretende-se investigar...
Os resultados serao analisados por...
```

Evite:

```text
eu mesmo apliquei...
mais tarde no artigo sera mostrado...
chute aleatorio...
estado da arte criado dentro do TensorFlow...
```

### 14. A secao sobre dataset ainda esta fraca

Onde aparece:

- `meu-tcc/anotacoes/anotacoes-revi-bibli.tex`, linhas iniciais sobre Mammo-Bench.
- `meu-tcc/primeiras-entregas/tcc_math.tex`, bases de dados em mamografia e metodologia.

O problema:

O texto diz que o dataset junta bases de varios paises e que voce aplicou tratamento de dados, mas ainda nao explica o suficiente para um leitor reproduzir ou confiar no estudo.

Como melhorar:

Inclua:

- nome exato da base;
- origem;
- numero total de imagens;
- numero de pacientes;
- classes usadas;
- distribuicao por classe;
- criterio de inclusao/exclusao;
- formato das imagens;
- tamanho final usado no modelo;
- normalizacao;
- tratamento de desbalanceamento;
- divisao treino/validacao/teste;
- cuidado para evitar vazamento por paciente;
- limitacoes da base.

Modelo:

```text
A base escolhida sera descrita quanto a origem, numero de imagens, numero de pacientes, classes disponiveis e distribuicao dos rotulos. Inicialmente serao consideradas as classes Normal, Benigno e Maligno. As imagens serao redimensionadas para dimensao compativel com os modelos avaliados e normalizadas antes do treinamento. Quando houver multiplas imagens da mesma paciente, a divisao treino/validacao/teste devera preservar a separacao por paciente, evitando vazamento de informacao entre particoes.
```

### 15. Falta separar contribuicao de Computacao e contribuicao medica

Onde aparece:

- Introducao e justificativa.

O problema:

O tema e de saude, mas o TCC e de Ciencia da Computacao. O texto precisa deixar claro que a contribuicao principal nao e diagnosticar melhor pacientes, e sim avaliar modelos computacionais sob um protocolo experimental.

Como melhorar:

Inclua uma frase de delimitacao:

```text
O trabalho nao tem como objetivo propor uma ferramenta clinica pronta para uso diagnostico, mas avaliar, em ambiente experimental, o comportamento comparativo de modelos classicos e hibridos aplicados a uma tarefa de classificacao mamografica.
```

Isso protege o texto contra cobrancas clinicas excessivas e deixa o foco na Computacao.

### 16. Falta explicitar reprodutibilidade

Onde aparece:

- Ja aparece de forma geral em alguns trechos, mas ainda nao como protocolo.

Como melhorar:

Inclua no metodo:

- versao de Python;
- TensorFlow/PyTorch;
- PennyLane/Qiskit;
- GPU/CPU;
- numero de epocas;
- otimizador;
- taxa de aprendizado;
- batch size;
- seeds;
- criterio de parada;
- configuracao de qubits;
- numero de camadas variacionais;
- encoding usado;
- repositorio/codigo, se aplicavel.

Sem isso, a comparacao pode parecer dificil de reproduzir.

### 17. Falta planejar a comparacao estatistica

Onde aparece:

- `tcc_matheus.tex` menciona "testes estatisticos sempre que possivel", mas o rascunho mais recente ainda nao desenvolve isso.

O problema:

Se voce comparar so uma execucao de cada modelo, a diferenca pode ser sorte de inicializacao, divisao dos dados ou ruido.

Como melhorar:

Use repeticoes:

```text
Cada modelo sera treinado em N execucoes independentes com sementes aleatorias distintas. As metricas serao apresentadas por media e desvio-padrao. Quando apropriado, sera aplicado teste estatistico para comparar o desempenho dos modelos.
```

Se o tempo for curto, use ao menos 3 sementes. Se der, 5 ou 10.

### 18. O cronograma precisa voltar para o rascunho mais recente

Onde aparece:

- `meu-tcc/primeiras-entregas/tcc_math.tex` tem secao de cronograma vazia.
- `meu-tcc/tcc_matheus.tex` tem um cronograma completo em Gantt.

Como melhorar:

Reaproveite o cronograma de `tcc_matheus.tex`, mas ajuste para as tarefas reais:

1. Consolidacao da revisao e pergunta de pesquisa.
2. Definicao da base e protocolo.
3. Pre-processamento e particionamento.
4. Implementacao da CNN baseline.
5. Implementacao do modelo hibrido.
6. Execucao dos experimentos.
7. Analise estatistica e tabelas.
8. Redacao final e revisao.

### 19. O titulo esta bom, mas pode ficar mais preciso

Titulo atual:

```text
Classificacao de cancer de mama em mamografias: um estudo comparativo entre CNNs classicas e hibridas quantico-classicas
```

Problema:

Esta adequado, mas pode sugerir que o foco e diagnostico de cancer de mama em geral. Seu recorte real e classificacao de imagens de mamografia com modelos computacionais.

Alternativas:

```text
Comparacao entre CNNs classicas e modelos hibridos quantico-classicos na classificacao multiclasse de mamografias
```

ou:

```text
Classificacao multiclasse de mamografias com CNNs classicas e modelos hibridos quantico-classicos: um estudo experimental comparativo
```

### 20. O texto precisa de uma ordem de revisao

Minha ordem recomendada para corrigir sem se perder:

1. Escolher qual arquivo sera o principal: `tcc_math.tex` ou `tcc_matheus.tex`.
2. Unificar a estrutura em tres capitulos principais: Introducao, Revisao, Metodologia/Solucao.
3. Escrever problema, pergunta e hipotese antes de mexer no resto.
4. Reescrever objetivo geral e objetivos especificos.
5. Completar metodologia experimental.
6. Corrigir citacoes manuais para `\cite` e `\citeonline`.
7. Adicionar a referencia de Pesapane ou remover a mencao.
8. Cortar trabalhos laterais da revisao ou justificar sua presenca.
9. Preencher solucao proposta e cronograma.
10. Revisar linguagem, acentos e padronizacao ABNT.

## Versao curta do que mais esta "errado"

- O rascunho mais recente tem uma hipotese vazia.
- O resumo esta informal e pouco academico.
- O objetivo ainda mistura pesquisa, implementacao e expansao futura.
- Os objetivos especificos parecem etapas do metodo.
- A metodologia experimental ainda nao esta suficientemente descrita.
- Ha duplicacao entre revisao bibliografica e referencial teorico.
- A introducao tem citacoes escritas manualmente, fora do padrao LaTeX/ABNT.
- Existe mencao a Pesapane sem entrada BibTeX encontrada.
- A solucao proposta e o cronograma estao vazios no arquivo mais recente.
- O escopo pode ficar grande demais se voce mantiver CNN, QML, granularidade maior, explicabilidade, ROI, controle de qualidade e eficiencia computacional ao mesmo tempo.

## Prioridade maxima para a proxima versao

Se voce so puder corrigir poucas coisas agora, corrija nesta ordem:

1. Preencher a hipotese.
2. Reescrever resumo, problema, pergunta de pesquisa e objetivo geral.
3. Transformar `Contexto`, `Justificativa`, `Objetivo` e `hipotese` em secoes dentro da Introducao.
4. Unificar `Revisao bibliografica` e `Referencial teorico`.
5. Completar a metodologia experimental.
6. Corrigir citacoes e bibliografia.

Com esses ajustes, o TCC deixa de parecer um conjunto de textos bons porem soltos e passa a parecer uma proposta de pesquisa controlada, verificavel e defensavel.
