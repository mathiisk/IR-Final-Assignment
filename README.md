

## Dependencies

```bash
pip install -r requirements.txt
```

Code was developed on a local computer with a GPU with ~16 GB VRAM.

## Data

Place TREC DL'19 files in `Data/`:

```
Data/
  queries.tsv
  candidates.tsv
  qrels.txt
```

MS MARCO training data is downloaded automatically into `msmarco-data/` on first run.

## Running

Run cells top to bottom. Fine-tuned cross-encoders are saved to `finetuned_models/<name>-<timestamp>/` and reloaded by path in later cells. The Zephyr LLM is pulled from HuggingFace and cached in `~/.cache/huggingface/`.
