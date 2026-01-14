# Chatbot-with-Transformer
Chatbot with transformer

## Models Overview

This project contains three different chatbot implementations using transformer models:

### Model Comparison

| Feature | **Model_1** (BlenderBot) | **Model_2** (FLAN-T5-base) | **Model_3** (FLAN-T5-small) |
|---------|--------------------------|----------------------------|----------------------------|
| **Model Name** | facebook/blenderbot-400M-distill | google/flan-t5-base | google/flan-t5-small |
| **Model Size** | ~730MB | ~990MB | ~308MB |
| **Type** | Conversational AI | Instruction-following | Instruction-following |
| **Best For** | Open-ended chat, friendly conversations | Complex Q&A, detailed tasks | Quick Q&A, faster responses |
| **Speed** | Medium | Slower (larger model) | **Fastest** (smaller model) |
| **Accuracy** | Good for dialogue | High accuracy | Lower accuracy than base |
| **Memory Usage** | Medium | High | **Low** (best for limited resources) |

### Key Differences

**Model_1 (BlenderBot):**
- 🎭 Personality-driven, conversational chatbot
- Designed for open-ended dialogue and maintaining context
- Best for: Casual conversations, friendly chat, building rapport
- Example: "How was your day?", "Tell me about your hobbies"

**Model_2 (FLAN-T5-base):**
- 🎯 Most accurate instruction-following model
- Handles complex questions and detailed explanations
- Best for: Question-answering, reasoning tasks, translations
- ⚠️ Slower and requires more memory
- Example: "Explain quantum physics", "Translate this to French"

**Model_3 (FLAN-T5-small):**
- ⚡ Fastest and lightest model
- Quick responses with lower resource requirements
- Best for: Simple Q&A, quick facts, basic tasks
- ⚠️ Less accurate than Model_2 but much faster
- Example: "What is the capital of France?", "Define photosynthesis"

### When to Use Each Model

- Use **Model_1** when you want natural, conversational dialogue
- Use **Model_2** when you need accurate, detailed, and comprehensive answers
- Use **Model_3** when you need quick responses or have limited computational resources

## How to Run

1. Install dependencies:
```bash
pip install torch torchvision torchaudio transformers tensorflow sentencepiece numpy
```

2. Run any model:
```bash
python Model_1.py  # BlenderBot
python Model_2.py  # FLAN-T5-base
python Model_3.py  # FLAN-T5-small
```

3. Chat with the bot - type your messages and press Enter
4. Exit by typing: `quit`, `exit`, or `bye`
