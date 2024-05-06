# Tiny GenAI Stack

This 🐳 Compose GenAI Stack is an example of the usage of the [Parakeet](https://github.com/parakeet-nest/parakeet) 🦜🪺 GoLang library, made to simplify the development of small generative AI applications.

## Start the stack

If you want to use the stack with your local install of Ollama:

```bash
HTTP_PORT=9999 LLM=tinydolphin OLLAMA_BASE_URL=http://host.docker.internal:11434 docker compose --profile webapp up
```
> Make sure that Ollama is started

If you want to use the stack with Ollama running in a container:
```bash
HTTP_PORT=8888 LLM=gemma:2b OLLAMA_BASE_URL=http://ollama:11434 docker compose --profile container up
```

> ✋ Compose will start the pull of the LLM, so be patient (my advice would be to use "small LLM" as tinyllama, tinydolphin or gemma:2b)

## Remarks

If you have a GPU on your workstation, you can turn on GPU access with Docker Compose: https://docs.docker.com/compose/gpu-support. With Mac M1, M2 and M3 use the local install of Ollama.
