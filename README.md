# Fase1Cap1-FIAP-ITIAOR2

## 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/in/bruno-castro-dias/">Bruno Castro - RM558359</a>
- <a href="https://www.linkedin.com/in/hugomariano191628150/">Hugo Mariano - RM560688</a>
- <a href="https://www.linkedin.com/in/matheus-castro-63644b224/">Matheus Castro - RM559293</a> 


## 👩‍🏫 Professores:
### Tutor(a) 
- <a href="https://www.linkedin.com/in/lucas-gomes-moreira-15a8452a/">Lucas Gomesr</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/in/profandregodoi/">Andre Godoi</a>


## 📜 Descrição

# 1. Análise de Dados de Doenças Cardíacas

## Origem dos Dados

Este conjunto de dados foi obtido do **Kaggle**, uma plataforma conhecida por hospedar conjuntos de dados para projetos de ciência de dados e machine learning. O dataset específico utilizado é o [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset), que contém informações relacionadas a pacientes e a presença ou ausência de doenças cardíacas.

### Natureza dos Dados
Os dados são **reais** e foram coletados de múltiplas fontes, incluindo hospitais e instituições de pesquisa. Eles são amplamente utilizados para prever a probabilidade de um paciente ter uma doença cardíaca com base em diversos atributos clínicos e demográficos.

## Variáveis Relevantes do Ponto de Vista Clínico

Do ponto de vista clínico, as seguintes variáveis são consideradas **mais relevantes** para um projeto de IA voltado à saúde:

### 1. **Idade (`age`)**
- **Justificativa**: A idade é um fator de risco significativo para doenças cardíacas. Pacientes mais velhos tendem a ter maior predisposição a problemas cardiovasculares.

### 2. **Sexo (`sex`)**
- **Justificativa**: Homens e mulheres podem apresentar diferenças significativas na manifestação de doenças cardíacas. O sexo é um fator importante para estratificação de risco.

### 3. **Tipo de Dor no Peito (`cp`)**
- **Justificativa**: O tipo de dor no peito (ex.: angina típica, atípica, não anginosa, assintomática) é um indicador crucial para diagnóstico de isquemia miocárdica.

### 4. **Pressão Arterial em Repouso (`trestbps`)**
- **Justificativa**: A hipertensão arterial é um dos principais fatores de risco para doenças cardiovasculares. Valores elevados aumentam significativamente o risco.

### 5. **Colesterol Sérico (`chol`)**
- **Justificativa**: Níveis elevados de colesterol estão associados ao acúmulo de placas nas artérias, aumentando o risco de infarto and acidente vascular cerebral.

### 6. **Açúcar no Sangue em Jejum (`fbs`)**
- **Justificativa**: Valores elevados de glicose em jejum podem indicar diabetes, que é um fator de risco independente para doenças cardíacas.

### 7. **Resultado de Eletrocardiograma em Repouso (`restecg`)**
- **Justificativa**: Alterações no ECG podem indicar isquemia, hipertrofia ventricular ou arritmias, all of which are relevant for cardiac assessment.

### 8. **Frequência Cardíaca Máxima Alcançada (`thalach`)**
- **Justificativa**: Uma frequência cardíaca máxima baixa durante o teste de esforço pode indicar doença arterial coronariana.

### 9. **Angina Induzida por Exercício (`exang`)**
- **Justificativa**: A presença de angina durante o exercício é um sintoma clássico de doença arterial coronariana.

### 10. **Depressão do Segmento ST (`oldpeak`)**
- **Justificativa**: Alterações no segmento ST durante o teste de esforço são indicativas de isquemia miocárdica.

### 11. **Inclinação do Segmento ST (`slope`)**
- **Justificativa**: A inclinação do segmento ST durante o pico do exercício ajuda a classificar a resposta isquêmica.

### 12. **Número de Vasos Principais Coloridos por Fluoroscopia (`ca`)**
- **Justificativa**: Indica o número de vasos sanguíneos principais com estreitamento significativo, diretamente relacionado à gravidade da doença.

### 13. **Talassemia (`thal`)**
- **Justificativa**: A talassemia pode afetar a capacidade de transporte de oxigênio no sangue, impactando a saúde cardiovascular.

### 14. **Presença de Doença Cardíaca (`target`)**
- **Justificativa**: Variável alvo que indica se o paciente tem (1) ou não (0) doença cardíaca. É o objetivo principal da predição.

## Importância para Projetos de IA em Saúde

Essas variáveis são **criticamente importantes** porque:

1. **Permitem a construção de modelos preditivos** robustos para identificar pacientes em risco.
2. **Facilitam a estratificação de risco** com base em evidências clínicas consolidadas.
3. **Podem ser integradas a sistemas de apoio à decisão clínica** para auxiliar médicos no diagnóstico precoce.
4. **Contribuem para a personalização de tratamentos** com base nas características individuais dos pacientes.

## Link para o Dataset

🔗 [Heart Disease Dataset no Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)

---

Este *dataset* é uma ferramenta valiosa para desenvolver soluções de IA que possam melhorar a detecção e o manejo de doenças cardíacas, ajudando a contribuir para melhores resultados de consultas cardiovasculares de pacientes e melhores tomadas de decisões por parte dos médicos

# 2. Análise de Textos Médicos em Cardiologia com Técnicas de NLP

## Origem dos Dados

Os documentos fornecidos são artigos científicos brasileiros da área de cardiologia:
1. **"Assessment of detraining through a six-minute walk test in patients with heart disease"** - Estudo de coorte retrospectivo sobre destreinamento em pacientes cardíacos
2. **"Hospitalizações e Mortalidade Hospitalar por Insuficiência Cardíaca no Brasil"** - Minieditorial sobre tendências epidemiológicas da insuficiência cardíaca no Brasil

Estes textos representam produções científicas reais publicadas em periódicos médicos brasileiros, contendo dados clínicos, metodologias de pesquisa e resultados estatisticamente validados.

## Potencial de Análise com NLP

### 1. Extração de Entidades Nomeadas (NER)
- **Sintomas e condições**: "insuficiência cardíaca", "hipertensão arterial", "diabetes mellitus"
- **Intervenções**: "reabilitação cardiovascular", "teste de caminhada de 6 minutos"
- **Medicações**: Podem ser identificadas mesmo quando não explicitamente listadas
- **Métricas clínicas**: "pressão arterial", "frequência cardíaca", "distância percorrida"

### 2. Análise de Tendências Temporais
- Identificação de padrões temporais em: "2000-2021", "22 anos", "última década"
- Extração de estatísticas temporais: "redução de 6,7%", "aumento de 3,5%"

### 3. Mineração de Resultados Estatísticos
- Extração de valores p: "P = 0,03", "P = 0,01"
- Captura de intervalos de confiança e medidas de dispersão: "64,1 ± 9,3 anos"
- Identificação de significância estatística: "diferença significativa", "redução significativa"

### 4. Classificação de Tópicos
- Categorização automática por: tipo de estudo, população-alvo, condições médicas
- Identificação de desfechos primários e secundários

### 5. Extração de Relações Semânticas
- Associação entre intervenções e resultados: "reabilitação cardiovascular → melhora da capacidade funcional"
- Conexões entre condições e complicações: "hipertensão → insuficiência cardíaca"

### 6. Análise Comparativa entre Estudos
- Identificação de concordâncias e discordâncias entre diferentes pesquisas
- Síntese automática de evidências conflitantes ou convergentes

## Relevância para Projetos de IA em Saúde

### 1. **Construção de Bases de Conhecimento**
- Os textos podem alimentar knowledge graphs para sistemas de apoio à decisão clínica
- Permitem mapear relações entre condições, tratamentos e desfechos na população brasileira

### 2. **Treinamento de Modelos de Linguagem Especializados**
- Fornecem corpus de treinamento em português com terminologia médica precisa
- Permitem desenvolver modelos específicos para cardiologia com contexto local

### 3. **Monitoramento de Tendências em Saúde Pública**
- Análise automática de mudanças epidemiológicas ao longo do tempo
- Detecção precoce de tendências emergentes em doenças cardiovasculares

### 4. **Automação de Revisões Sistemáticas**
- Extração automática de dados de estudos científicos para meta-análises
- Aceleração do processo de síntese de evidências científicas

### 5. **Personalização de Cuidados**
- Identificação de subpopulações específicas (por idade, sexo, comorbidades)
- Suporte à medicina de precisão com dados da população brasileira

### 6. **Otimização de Alocações de Recursos**
- Análise preditiva de demandas hospitalares baseada em tendências extraídas
- Planejamento de serviços de saúde baseado em evidências locais

## Exemplos de Aplicações Práticas

1. **Sistema de alerta precoce** para tendências de aumento de mortalidade hospitalar
2. **Assistente virtual** para prescrição de exercícios em reabilitação cardíaca
3. **Ferramenta de análise** para comissões de controle de infecção hospitalar
4. **Sistema de triagem** automática baseado em sintomas extraídos de literature

## Limitações e Considerações

- Os textos estão em português, requerendo modelos especializados para processamento
- A terminologia médica exige validação por profissionais de saúde
- Dados retrospectivos podem conter viéses que devem ser considerados nas análises

## Conclusão

Estes textos representam uma fonte valiosa para desenvolver soluções de NLP aplicadas à cardiologia no contexto brasileiro. A extração sistemática de informações permite não apenas compreender melhor o panorama atual das doenças cardíacas no Brasil, mas também construir ferramentas de IA que possam melhorar diretamente o cuidado ao paciente e a alocação de recursos em saúde.

**Referências dos Documentos Analisados:**
1. Silva VM et al. Assessment of detraining through a six-minute walk test in patients with heart disease. Sao Paulo Med J. 2025;143(1):e2023334
2. Latado AL. Hospitalizações e Mortalidade Hospitalar por Insuficiência Cardíaca no Brasil: Um Panorama Atualizado. Arq Bras Cardiol. 2025;122(6):e20250284



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
