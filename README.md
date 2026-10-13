# Deveshu Pathak

I train models and build the software around them: a speech model small enough to run on a
laptop, credit and fraud models with calibrated and reproducible evaluation, and desktop tools
that keep your data on your machine.

BS in Data Science and Applications, IIT Madras.

---

## Butterfly Labs

Local-first tools for Windows. No account, no upload, no telemetry. Your recordings and
transcripts are plain files on your disk.

| | | |
| :-- | :-- | :-- |
| **[Butterfly Speak](https://github.com/Deveshu04/Butterfly-Speak)** | Rust · Tauri | Hold `Ctrl+Win`, speak, release, and the text is typed where your cursor already is. English and 22 Indian languages, on-device or with your own key. |
| **[Butterfly Record](https://github.com/Deveshu04/Butterfly-Record)** | TypeScript · Rust | Screen recorder for Windows and Chrome. Recordings stay as ordinary files; transcription runs on your PC. |
| **[Butterfly Code CLI](https://github.com/Deveshu04/Butterfly-Code-CLI)** | TypeScript · Bun | An agentic coding CLI with a terminal UI, tuned for accuracy and low token use on any model. |

→ [butterflylabs](https://deveshu04.github.io/)

---

## Research

**[turn-detector](https://github.com/Deveshu04/turn-detector)** is a 7.9M-parameter audio-only
classifier that decides whether a speaker has finished or is only pausing, from the last 8
seconds of speech. It is built for Indian Hinglish: code-switched Hindi and English in both
Devanagari and romanized script, Indian-accented prosody, filler words and trailing
conjunctions.

Trained with 2,157 synthetic code-switched clips, it reaches **95.1%** on held-out Hinglish, a
gain of 32.0 points, while holding English accuracy flat at 0.938.

---

## Applied machine learning

Each project fixes its evaluation holdout before any model exists, and every number below comes
from a single scored run on that holdout.

| Project | Approach | Evaluated on | Result |
| :-- | :-- | :-- | :-- |
| **[Credit Risk + Explainable AI](https://github.com/Deveshu04/Credit-Risk-Modeling-with-Explainable-AI)** | LightGBM and XGBoost blended in log-odds, exact SHAP, Basel III master scale with IRB capital by segment | 61,503-applicant stratified holdout, fixed before modelling | **AUC 0.799**, Gini 0.598, KS 0.455 |
| **[Illicit Bitcoin Detection](https://github.com/Deveshu04/Illicit-Bitcoin-Transaction-Detection-via-Graph-Neural-Networks)** | GraphSAGE with focal loss and graph-aware sampling, stacked into LightGBM over NetworkX neighbourhood features | Strict temporal split, scored once on 16,670 later transactions | **AUC 0.950**, illicit-class F1 0.819 |
| **[EV Purchase Prediction](https://github.com/Deveshu04/Predicting-Electric-Vehicle-Purchases)** | LightGBM, XGBoost and logistic regression stacked on fold-safe target encoding | Kaggle Playground S6E9, 286,571 test rows | **320th of 3,575 teams**, top 9% |
| **[FinBERT Sentiment](https://github.com/Deveshu04/Financial-Sentiment-Classification-via-Fine-tuned-FinBERT)** | FinBERT fine-tuned on the Financial PhraseBank, served as an 8-bit ONNX model behind a Flask API | 484 held-out sentences, then 32,692 Reuters headlines | **83.5% accuracy**, macro F1 0.821 |

---

## Also here

**[roleflow](https://github.com/Deveshu04/roleflow)** is an open-source job-application agent:
live search, per-job resume tailoring, and a browser agent that fills real applications. You
approve every submission.

**[Genetic Disorder Prediction](https://github.com/Deveshu04/Genetic-Disorder-Prediction-App)**
is my earliest public project, and still the one people fork.

---

## Skills

**Languages**<br>
Python · Java · Rust · TypeScript · JavaScript · SQL · Bash · PowerShell

**Machine learning**<br>
Supervised learning · Unsupervised learning · Classification · Regression · Clustering ·
Ensemble methods · Gradient boosting · LightGBM · XGBoost · CatBoost · Random forests ·
Decision trees · Support vector machines · k-nearest neighbours · Naive Bayes ·
Logistic regression · Stacking and blending · Feature engineering · Feature selection ·
Target encoding · Dimensionality reduction · PCA · t-SNE · UMAP · Hyperparameter optimisation ·
Optuna · Cross-validation · Imbalanced learning · SMOTE · Focal loss · Class weighting ·
Model calibration · Threshold tuning · ROC-AUC · PR-AUC · Gini · KS statistic · F1 ·
Confusion matrices · Bootstrap confidence intervals

**Deep learning**<br>
Neural networks · Feedforward networks · Backpropagation · Convolutional neural networks ·
Recurrent neural networks · LSTM · GRU · Transformers · Self-attention · Encoder-decoder
architectures · Autoencoders · Variational autoencoders · Generative adversarial networks ·
Diffusion models · Residual networks · Batch and layer normalisation · Dropout ·
Regularisation · Transfer learning · Fine-tuning · Knowledge distillation · Quantisation ·
Pruning · Mixed-precision training · Learning-rate scheduling · PyTorch · TensorFlow · Keras ·
Hugging Face Transformers

**Graph machine learning**<br>
Graph neural networks · GraphSAGE · Graph convolutional networks · Graph attention networks ·
Message passing · Node classification · Link prediction · Graph embeddings ·
Neighbourhood sampling · Community detection · Centrality measures · NetworkX ·
PyTorch Geometric · Deep Graph Library

**Natural language processing**<br>
Text classification · Sentiment analysis · Named entity recognition · Tokenisation ·
Word embeddings · Word2Vec · GloVe · Sentence transformers · BERT · RoBERTa · FinBERT ·
DistilBERT · Topic modelling · Summarisation · Machine translation · Question answering ·
TF-IDF · n-gram models · Text preprocessing · Semantic similarity

**Speech and audio**<br>
Automatic speech recognition · Whisper · Turn detection · Voice activity detection ·
Speaker diarisation · Audio classification · Keyword spotting · Text to speech ·
Spectrograms · Mel-frequency cepstral coefficients · Prosody modelling ·
Code-switched and multilingual speech · Synthetic data generation

**Computer vision**<br>
Image classification · Object detection · Image segmentation · Face and gesture recognition ·
Feature extraction · Data augmentation · ResNet · EfficientNet · YOLO · Vision transformers ·
OpenCV · Pillow

**Generative AI and LLM engineering**<br>
Large language models · Prompt engineering · Retrieval-augmented generation · Vector databases ·
pgvector · FAISS · Chroma · Pinecone · Semantic search · Embeddings · Chunking strategies ·
Reranking · AI agents · Multi-agent systems · Tool and function calling ·
Model Context Protocol · Agentic workflows · Structured output · Streaming responses ·
Context-window management · Token optimisation · LLM evaluation and evals · Guardrails ·
Hallucination mitigation · LoRA and PEFT · Instruction tuning · RLHF · Model routing ·
LangChain · LlamaIndex · Vercel AI SDK · OpenAI · Anthropic · Hugging Face

**MLOps and deployment**<br>
Model serving · REST APIs · Flask · FastAPI · ONNX · ONNX Runtime · Experiment tracking ·
MLflow · Weights & Biases · Reproducible pipelines · Model versioning · Model monitoring ·
Drift detection · Docker · CI/CD · GitHub Actions · Batch and real-time inference ·
Edge and on-device inference · Inference optimisation

**Data engineering and analytics**<br>
SQL · PostgreSQL · MySQL · SQLite · MongoDB · Supabase · pandas · NumPy · Polars · Dask ·
Apache Spark · Apache Kafka · ETL and ELT pipelines · Data modelling · Data cleaning ·
Data validation · Web scraping · Exploratory data analysis · Matplotlib · Seaborn · Plotly ·
Power BI · Excel

**Statistics and experimentation**<br>
Descriptive statistics · Probability · Hypothesis testing · Confidence intervals · A/B testing ·
Experimental design · Bayesian inference · Regression analysis · Time-series analysis ·
Forecasting · ARIMA · Survival analysis · Causal inference · Monte Carlo simulation ·
Sampling methods

**Explainability and responsible AI**<br>
SHAP · LIME · Feature importance · Partial dependence plots · Counterfactual explanations ·
Model interpretability · Fairness assessment · Bias detection · Model risk documentation ·
Basel III · IRB capital modelling · Scorecard development

**Software and product**<br>
Next.js · React · Svelte · Node.js · Tauri · Tailwind CSS · REST API design · Playwright ·
Pytest · Vitest · Git · Linux · Windows desktop applications · Browser extensions ·
System design · Technical writing

---

[LinkedIn](https://www.linkedin.com/in/deveshupathak/) · [butterflylabs](https://deveshu04.github.io/)
