# Tarefa-Bruno-Hayashi

O objetivo desta tarefa foi analisar a estimativa de pose em bovinos utilizando um subconjunto do ANIMAL-POSE DATASET. A tarefa principal consistiu em identificar e avaliar a distribuição de keypoints nas imagens disponíveis, com foco na categoria "bovino". Embora o dataset contivesse 842 anotações para bovinos, apenas 200 imagens estavam acessíveis, o que limitou a análise a esse subconjunto. A análise exploratória incluiu a distribuição das coordenadas dos keypoints, variabilidade entre eles e a correlação dos pontos ao longo do corpo dos bovinos, fornecendo insights sobre a consistência das anotações e a qualidade dos dados. Mesmo com as limitações do dataset, a análise mostrou o potencial da estimativa de pose para monitoramento de saúde e comportamento na pecuária.

Conclusões e Reflexões Pessoais
Com base nos resultados obtidos, ficou claro que o mediapipe, embora excelente para estimativa de pose em humanos, não é aplicável para animais como bovinos. A incapacidade do modelo de detectar poses nas imagens dos bovinos não foi surpreendente, já que o modelo foi treinado exclusivamente com dados humanos. Isso me levou a buscar alternativas e a considerar o uso de modelos específicos para animais, como o DeepLabCut, que oferece uma abordagem mais ajustada para capturar a morfologia e os movimentos de diferentes espécies.

Para as imagens humanas, o desempenho do mediapipe foi bastante satisfatório, com a detecção precisa das poses na maioria dos casos. A única exceção foi na imagem "LL.jpg" (removida do dataset após o teste por conta da privacidade do indivíduo que teve a foto utilizada), onde o corte do corpo dificultou a detecção completa da pose. Isso reforça a importância de usar imagens bem enquadradas e com visibilidade total do corpo para resultados precisos. Essa experiência mostrou que, mesmo com modelos bem treinados, a qualidade do dataset ainda desempenha um papel fundamental na precisão dos resultados.

A análise dos bovinos trouxe algumas reflexões importantes. A distribuição desigual dos keypoints e a presença de outliers apontam para problemas nas anotações, que, se não corrigidos, podem comprometer o treinamento de modelos mais robustos. Outro ponto relevante foi a falta de 642 imagens mencionadas no JSON, o que comprometeu a completude e robustez da análise. Garantir que o dataset esteja completo e bem anotado é essencial para a confiabilidade dos resultados.

Para o futuro, acredito que seria interessante explorar o treinamento de modelos customizados com transfer learning, utilizando um dataset completo e bem anotado. Outra abordagem seria combinar estimativa de pose com técnicas de visão computacional como segmentação semântica, para monitorar o comportamento e a saúde dos bovinos em tempo real. Aplicações práticas como essas podem trazer um impacto significativo para o monitoramento de animais em fazendas e contribuir para a pecuária de precisão.

Além disso, fica claro que o uso de ferramentas como o mediapipe deve ser bem direcionado e adaptado ao contexto específico. Para humanos, a ferramenta é robusta e eficiente, mas para animais, é essencial buscar soluções que considerem as particularidades de cada espécie. Esse aprendizado ressalta a importância de uma abordagem cuidadosa e adaptativa ao aplicar tecnologias de visão computacional em diferentes áreas.

Essas foram algumas das minhas observações e aprendizados com este projeto. O processo me permitiu explorar as limitações e as potencialidades das tecnologias atuais, e acredito que o próximo passo seria focar em adaptar essas ferramentas para contextos específicos, como o monitoramento de saúde e comportamento de animais em ambientes controlados.







