### Output (Saída)

O objetivo final do projeto é utilizar Variational Autoencoders (VAEs) para:
- Gerar imagens de cachorros de raças novas a partir da combinação de características de raças existentes no dataset.
- Potencialmente identificar combinações que poderiam representar o "vira-lata caramelo" ou o mascote "Pythinho" através da geração de novas raças de cachorros.

### Input (Entrada)

- **Dataset**: Utilização do dataset [Dog Breed Identification](https://www.kaggle.com/c/dog-breed-identification/data) disponível no Kaggle, que contém imagens de diferentes raças de cachorros.
- **Imagens de Referência**: Duas imagens de cachorros fornecidas como exemplos de novas raças potenciais a serem geradas pelo modelo.

### Process (Processo)

1. **Preparação dos Dados**:
   - Download do dataset do Kaggle.
   - Pré-processamento das imagens (redimensionamento para um tamanho padrão, normalização, etc.).
   - Divisão do dataset em conjuntos de treinamento, validação e teste.

2. **Construção do Modelo VAE**:
   - Desenvolvimento do Variational Autoencoder, que inclui a construção de um encoder para mapear as imagens de entrada para um espaço latente, e um decoder para reconstruir as imagens a partir do espaço latente.
   - Utilizar frameworks como TensorFlow + Keras ou PyTorch para a implementação.

3. **Treinamento do Modelo**:
   - Treinar o VAE no dataset de cachorros, ajustando os parâmetros para minimizar a diferença entre as imagens originais e as imagens reconstruídas, bem como para garantir que o espaço latente seja bem-organizado e contínuo.

4. **Exploração do Espaço Latente e Geração de Novas Imagens**:
   - Explorar o espaço latente gerado pelo encoder para entender como as diferentes raças são representadas.
   - Gerar novas imagens por meio da interpolação entre pontos no espaço latente que representam características distintas das raças de cachorros, visando criar imagens de novas raças.
   - Utilizar técnicas de interpolação para misturar características de diferentes raças e gerar as imagens alvo, como o "vira-lata caramelo" e o "Pythinho".

5. **Avaliação e Ajustes**:
   - Avaliar visualmente as imagens geradas e ajustar o modelo conforme necessário para melhorar a qualidade das imagens produzidas.
   - Considerar ajustes no modelo, no espaço latente ou no processo de interpolação baseado no feedback visual e nos objetivos específicos do projeto.

6. **Documentação e Preparação para Produção**:
   - Documentar todo o processo, incluindo a arquitetura do modelo, o processo de treinamento e as técnicas de interpolação utilizadas.
   - Preparar o modelo para ser utilizado em aplicações práticas, se necessário.
