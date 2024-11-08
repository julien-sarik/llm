# llm
Start the Ollama app within a container:
```
podman run --rm -p 11434:11434 --name ollama -v "$PWD/.ollama":/root/.ollama ollama/ollama:0.4.0
```

Download and run a Llama model within the Ollama app:
```
podman exec -it ollama ollama run llama3.2:1b
```