# nlp

NLP

## Reproducibility of POC

Assuming there is local ollama and garak installations:

```bash
ollama pull qwen3:0.6b
ollama serve
```

```bash
garak --config safety_3areas.yml
```

## Reproducibility of safety bench: cultural, disinformative, offensive

```bash
cd safety-bench
uv run score_prompts.py --input nlp.xlsx --output scored_prompts.xlsx --subset disinformation
```
