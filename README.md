```mermaid
graph TB
    A[Input Layer: CSV, Text, Image]:::input
    B[Preprocessing: Cleaning, Tokenization]:::process
    C[Feature Engineering or Embedding]:::process

    D1[ML Model: Decision Tree]:::mlmodel
    D2[DL Model: CNN, RNN, LSTM]:::dlmodel
    D3[Transformer Model: Encoder-Decoder]:::transformer

    E1[ML Output: Report or Prediction]:::output
    E2[DL Output: Class, Score, Forecast]:::output
    E3[Transformer Output: Text, Answer, Translation]:::output

    A --> B --> C
    C --> D1 --> E1
    C --> D2 --> E2
    C --> D3 --> E3

    classDef input fill:#dbeafe,stroke:#3b82f6,color:#1e3a8a;
    classDef process fill:#fef3c7,stroke:#facc15,color:#92400e;
    classDef mlmodel fill:#e0f2fe,stroke:#0284c7,color:#0c4a6e,font-weight:bold;
    classDef dlmodel fill:#ede9fe,stroke:#7c3aed,color:#4c1d95,font-weight:bold;
    classDef transformer fill:#ecfdf5,stroke:#14b8a6,color:#064e3b,font-weight:bold;
    classDef output fill:#dcfce7,stroke:#22c55e,color:#14532d;
