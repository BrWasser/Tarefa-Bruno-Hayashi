# Tarefa-Bruno-Hayashi

Os resultados que obtive com o mediapipe mostraram um contraste claro entre a eficácia em humanos e a incapacidade de detecção em bovinos. O modelo foi bem-sucedido em identificar poses humanas, mas falhou completamente com os animais. Isso não é surpreendente, já que o mediapipe é treinado apenas com dados de poses humanas, o que limita muito sua aplicação em outros contextos.

Quando tentei aplicar o mediapipe nas imagens de bovinos, nenhuma pose foi detectada, mesmo nas imagens mais claras. Isso me levou a pesquisar outras alternativas mais adequadas para esse tipo de tarefa. Encontrei o DeepLabCut, uma ferramenta voltada especificamente para estimativa de poses em animais. Esse modelo é treinado com dados de várias espécies e pode ser customizado para detectar pontos-chave em bovinos com alta precisão. Seria uma ótima escolha caso o objetivo fosse realmente capturar detalhes da postura e movimento dos animais.

Já para humanos, o desempenho do mediapipe foi excelente na maioria das imagens. Ele conseguiu mapear as articulações e a orientação corporal com bastante precisão, exceto em situações em que partes do corpo estavam fora do enquadramento, como na imagem "LL.jpg". Isso me fez perceber a importância de trabalhar com imagens bem enquadradas e com visibilidade completa do corpo para obter resultados consistentes.

A partir desses testes, ficou claro que o mediapipe é muito eficiente dentro do seu escopo, mas é necessário buscar alternativas quando o contexto muda. Para animais, como os bovinos, o ideal seria treinar um modelo customizado ou explorar bibliotecas como o LEAP ou o DeepLabCut, que oferecem suporte a diversas espécies e permitem ajustes específicos para cada aplicação.

Além disso, percebi que a coleta de dados de qualidade é fundamental para qualquer tipo de análise em visão computacional. Pequenas variações na qualidade e no ângulo das imagens podem impactar muito o desempenho dos modelos. Para um trabalho futuro, garantir que todas as imagens sejam capturadas em condições ideais, com boa iluminação e visibilidade, seria um passo essencial.

Pensando em próximos passos, explorar a integração de diferentes modelos e técnicas para análise comportamental e monitoramento de saúde animal poderia trazer insights valiosos. Por exemplo, combinar estimativa de pose com segmentação de imagem ajudaria a monitorar o comportamento dos animais em tempo real, algo que seria extremamente útil em um ambiente de fazenda ou laboratório.

Essas são algumas das reflexões e aprendizados que tive ao longo desse processo. Se o objetivo for seguir com a estimativa de pose em animais, vale a pena investir em modelos mais especializados e robustos, capazes de lidar com as particularidades de cada espécie.
