# fiesta_llm


# 1. Instalacion de OLLAMA
curl -fsSL https://ollama.com/install.sh | sh

## 2. Instalación 

ollama serve

ollama pull tinyllama


## 3. Hablar con OLLAMA
ollama run tinyllama ___

## 4.tokens despacio
curl http://127.0.0.1:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt":"por que el cielo es azul?"
  
}'
## 5.tokens instantanios
curl http://127.0.0.1:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt":"por que el cielo es azul?",
  "stream": false
}'
