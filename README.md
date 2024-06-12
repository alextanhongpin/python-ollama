# Getting Started


```bash
$ ollama run phi3
$ ollama
$ ollama list
$ ollama show phi3 --template
{{ if .System }}<|system|>
{{ .System }}<|end|>
{{ end }}{{ if .Prompt }}<|user|>
{{ .Prompt }}<|end|>
{{ end }}<|assistant|>
{{ .Response }}<|end|>
```

To kill `ollama serve`:

```bash
# https://github.com/ollama/ollama/issues/690
$ ollama ps
# or pgrep ollama
$ lsof -i :11434 # Get the PID
$ kill -9 <PID>
```
