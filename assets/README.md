# 3. Dataset de Imagens de Eletrocardiograma (ECG)

## Link de Acesso
<a href= "https://fiapcom-my.sharepoint.com/:f:/g/personal/rm559293_fiap_com_br/Es5sFzhOU-VGlCbu2wrbDbEBeU3EM0Z82-X_Jy_5BrzsSQ?e=RuWmTF"> One Drive </a>

## Link para Download
<a href= "https://www.kaggle.com/datasets/evilspirit05/ecg-analysis"> Dataset Online </a>

## Descrição do Dataset

Este conjunto de dados é composto por imagens de eletrocardiogramas (ECG) categorizadas em quatro classes distintas, destinadas a auxiliar no desenvolvimento e na valiação de modelos de aprendizado de máquina e visão computacional para diagnóstico cardíaco. As categorias são as seguintes:

- **ECG Images of Myocardial Infarction Patients**: 2.880 imagens  
  (240 pacientes × 12 derivações/imagens)
- **ECG Images of Patients with Abnormal Heartbeat**: 2.796 imagens  
  (233 pacientes × 12 derivações/imagens)
- **ECG Images of Patients with History of Myocardial Infarction (MI)**: 2.064 imagens  
  (172 pacientes × 12 derivações/imagens)
- **Normal Person ECG Images**: 3.408 imagens  
  (284 pacientes × 12 derivações/imagens)

## Justificativa para Análise por Visão Computacional

As imagens de ECG contêm padrões visuais ricos em informações clínicas, como morfologias de onda (P, QRS, T), segmentos (ST) e intervalos, que são críticos para o diagnóstico de condições cardíacas. Algoritmos de Visão Computacional (CV) podem ser aplicados para extrair automaticamente esses padrões e auxiliar na identificação de anomalias. Abaixo, descrevemos como técnicas de CV podem ser utilizadas:

### 1. **Detecção de Padrões**
   - Técnicas como extração de características (SIFT, HOG) ou redes neurais convolucionais (CNNs) podem identificar morfologias típicas de ECG, como elevação do segmento ST (comum em infarto agudo do miocárdio) ou alterações na onda T.
   - Esses padrões são fundamentais para distinguir entre classes normais e patológicas.

### 2. **Identificação de Bordas e Segmentação**
   - Algoritmos de detecção de bordas (como Canny ou Sobel) podem ser usados para delimitar regiões de interesse nos traçados de ECG, como o início e o fim de complexos QRS.
   - A segmentação precisa dessas regiões permite a medição automática de intervalos (e.g., intervalo QT) e amplitudes, essenciais para avaliação clínica.

### 3. **Reconhecimento de Anomalias**
   - Modelos de classificação de imagens (ex.: ResNet, EfficientNet) podem ser treinados para reconhecer padrões associados a doenças específicas, como arritmias ou infartos prévios.
   - Redes neurais recorrentes (RNNs) ou híbridas (CNN + RNN) também podem ser aplicadas para capturar dependências temporais em séries de ECG convertidas em imagens.

### 4. **Pré-processamento e Aumento de Dados**
   - Técnicas de augmentação (rotação, translação, ajuste de brilho/contraste) podem melhorar a generalização dos modelos, simulando variações na captura de ECG do mundo real.
   - A normalização de imagens (redimensionamento, equalização de histograma) garante consistência na entrada dos algoritmos.

## Importância para Projetos de IA na Área da Saúde

A aplicação de visão computacional e aprendizado de máquina em imagens de ECG tem grande potencial para impactar a área da saúde, principalmente por:

1. **Automação de Diagnósticos**:  
   Modelos precisos podem auxiliar médicos na triagem rápida de casos críticos (ex.: infarto agudo), reduzindo o tempo entre a aquisição do ECG e a intervenção.

2. **Escalabilidade e Acesso**:  
   Sistemas baseados em IA podem ser implantados em regiões com pouca expertise cardiológica, democratizando o acesso a diagnósticos de qualidade.

3. **Consistência na Análise**:  
   Algoritmos eliminam viéses humanos e variações interobservadores, oferecendo avaliações padronizadas e reprodutíveis.

4. **Integração com Fluxos de Trabalho Existentes**:  
   As imagens de ECG são amplamente utilizadas em prontuários eletrônicos e sistemas de telemedicina, facilitando a adoção de ferramentas de IA sem mudanças disruptivas.

5. **Pesquisa e Descoberta de Novos Padrões**:  
   Técnicas não supervisionadas podem revelar correlacões visuais ainda não documentadas na literatura médica, contribuindo para avanços na cardiologia.

## Considerações Éticas e Limitações

- Este dataset deve ser utilizado apenas para fins de pesquisa e desenvolvimento de algoritmos, não substituindo o diagnóstico clínico formal.
- É crucial validar modelos em datasets independentes e com supervisão de profissionais de saúde.
- Imagens devem ser anônimas e estar em conformidade com regulacões de proteção de dados (ex.: LGPD, GDPR).