### Objetivo:
Detetar anomalias ou incoerências em transações, utilizando um algoritmo baseado em machine learning para análise de comportamento das mesmas.
<h4>Machine learning</h4>
<u>Machine Learning (ML)</u> estudo baseado em AI(inteligência artificial) que se preocupa com o desenvolvimento e o estudo de algoritmos estatísticos tentando reproduzir o raciocínio e a lógica humana.

### Publico-alvo:
Entidades bancárias que procuram a análise de risco de cada transação podendo assim alertar de imediato os seus clientes.

### Requisitos e Funcionalidades:

Para este projeto seria necessário a integração de um LLM (Large language Model) como um algoritmo que tenha conexão em tempo-real com os dados bancários de cada cliente.

Para o LLM decidimos usar o AWS amazon fraud detector que é um Machine learning que deteta comportamento e padrões fora do normal, classificando-os pelo risco.
Como o LLM iria ter poucas referências de fraude, iremos introduzir uma (técnica de sobreamostragem minoritária sintética) ou <u>SMOTE</u> que criaria dados sintéticos da classe minoritária até que a base de treino atinja o equilíbrio de 50%.

Posteriormente precisaríamos de uma ferramenta que avise o cliente de imediato após a deteção da ocorrência.

### Restrições:

- Falsos negativos e falsos positivos, a AI apesar de muito bem treinada pode errar;
- Necessidade de dados bancários de qualidade;
- Apelar ao máximo para o mínimo de latência possível para avisar o cliente o quanto antes;
- Complexidade de implementação;
- Privacidade e regulamentação;
- Orçamento Alto.

### Critérios de sucesso:
O sucesso irá ser medido tendo em conta a nossa taxa de acerto em casos realmente fraudulentos acima de 99% (Verificar métrica AUC) e trabalhar com uma empresa grande em um espaço de tempo máximo de 1 ano.

### Comunicação:

