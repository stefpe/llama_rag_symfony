# LLAMA RAG Symfony

Use LLAMA2 cpp library in a Symfony project and test embeddings.

## Download LLAMA2 model
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF
e.g. https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGUF/blob/main/llama-2-7b-chat.Q2_K.gguf

## Build and run C++ webserver (Faster performance) https://github.com/ggerganov/llama.cpp/tree/master/examples/server
    - git clone https://github.com/ggerganov/llama.cpp.git
    - cd llama.cpp
    - LLAMA_METAL=1 make (Metal for Apple Silicone)
    - ./llama.cpp/server -m models/llama-2-7b-chat.Q2_K.gguf -c 2048 --embedding
