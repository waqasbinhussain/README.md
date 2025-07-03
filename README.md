## 🤖 AI Model Architectures (Top-to-Bottom Flow)

```mermaid
flowchart TB

%% ML Flow
subgraph ML["🟦 Machine Learning (ML): Decision Tree"]
    A1(["📥 Input: Structured Data (CSV)"]):::input
    B1(["🧹 Preprocessing"]):::process
    C1(["🛠️ Feature Engineering"]):::process
    D1(["🌳 Decision Tree Model"]):::mlmodel
    E1(["🧪 Training & Validation"]):::process
    F1(["🎯 Prediction"]):::output
    G1(["📊 Output: Report or Decision"]):::output
    A1 --> B1 --> C1 --> D1 --> E1 --> F1 --> G1
end

%% DL: CNN / RNN Flow
subgraph DL1["🟩 Deep Learning (DL): CNN / RNN"]
    A2(["🖼️/📝 Input: Image / Text / Audio"]):::input
    B2(["🔧 Preprocessing"]):::process
    C2(["🧠 Model: CNN or RNN"]):::dlmodel
    D2(["📡 Forward Pass"]):::process
    E2(["🔁 Backpropagation"]):::process
    F2(["🎯 Prediction (Label/Score)"]):::output
    G2(["🧾 Output: Human-Readable Format"]):::output
    A2 --> B2 --> C2 --> D2 --> E2 --> F2 --> G2
end

%% Transformer Flow
subgraph DL2["🟪 Transformer (DL): Encoder–Decoder"]
    A3(["📝 Input: Text Sequence"]):::input
    B3(["🔤 Tokenization + Embedding"]):::process
    C3(["📥 Encoder (Context Understanding)"]):::dlmodel
    D3(["📤 Decoder (Text Generation)"]):::dlmodel
    E3(["🎯 Attention + Feedforward Layers"]):::process
    F3(["🧾 Output Tokens"]):::output
    G3(["📄 Output: Text / Translation / Answer"]):::output
    A3 --> B3 --> C3 --> D3 --> E3 --> F3 --> G3
end

%% LSTM Flow
subgraph DL3["🟫 DL: LSTM (Long Short-Term Memory)"]
    A4(["📈 Input: Time Series / Text"]):::input
    B4(["🔠 Tokenization / Sequence Prep"]):::process
    C4(["⏳ Model: LSTM Layers"]):::dlmodel
    D4(["📡 Forward Pass"]):::process
    E4(["🔁 Backprop Through Time"]):::process
    F4(["🔮 Prediction: Sequence Output"]):::output
    G4(["📉 Output: Forecast, Text"]):::output
    A4 --> B4 --> C4 --> D4 --> E4 --> F4 --> G4
end

%% GAN Flow
subgraph DL4["🟥 DL: GAN (Generative Adversarial Network)"]
    A5(["🎲 Input: Random Noise"]):::input
    B5(["🧪 Generator: Create Fake Data"]):::dlmodel
    C5(["🕵️ Discriminator: Real vs Fake"]):::dlmodel
    D5(["🤼 Adversarial Training Loop"]):::process
    E5(["🔄 Improved Generator"]):::process
    F5(["🖼️ Output: Fake Image/Text/Audio"]):::output
    A5 --> B5 --> C5 --> D5 --> E5 --> F5
end

%% RL Flow
subgraph RL["🟨 Reinforcement Learning (RL)"]
    A6(["🌍 Input: Environment State"]):::input
    B6(["🧠 Agent (Policy + Exploration)"]):::rlmodel
    C6(["⚙️ Action Taken"]):::process
    D6(["🏆 Reward / Feedback"]):::process
    E6(["📈 Policy Update"]):::process
    F6(["🧠 Smarter Agent"]):::process
    G6(["🚀 Output: Strategy / Plan"]):::output
    A6 --> B6 --> C6 --> D6 --> E6 --> F6 --> G6
end

%% Style Classes
classDef input fill:#d4e4ff,stroke:#3b82f6,color:#111;
classDef process fill:#fff4e5,stroke:#f59e0b,color:#111;
classDef output fill:#dcfce7,stroke:#22c55e,color:#111;
classDef mlmodel fill:#e0f2fe,stroke:#0284c7,color:#111,font-weight:bold;
classDef dlmodel fill:#ede9fe,stroke:#7c3aed,color:#111,font-weight:bold;
classDef rlmodel fill:#fef9c3,stroke:#eab308,color:#111,font-weight:bold;
