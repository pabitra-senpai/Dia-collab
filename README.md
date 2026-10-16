# Dia on Google Colab

Run [nari-labs/dia](https://github.com/nari-labs/dia) (1.6B text-to-dialogue TTS) in a free Colab T4 GPU.

## Quick start
1. Upload this repo to GitHub (or just upload `dia_colab.ipynb` to [colab.research.google.com](https://colab.research.google.com) via File → Upload notebook).
2. Runtime → Change runtime type → **T4 GPU**.
3. Run the cells top to bottom.

### Open from GitHub
After pushing to your GitHub, use this link (replace `YOUR_USER`):

```
https://colab.research.google.com/github/YOUR_USER/dia-colab/blob/main/dia_colab.ipynb
```

## Script format
```
[S1] Hello there. [S2] Hi! How are you? (laughs) [S1] Great, thanks.
```
- Start with `[S1]`, alternate speakers.
- ~5–20 seconds of speech per generation.
- English only. Use non-verbal tags sparingly.

## Notes
- Same `seed` → same voices. Voice cloning needs a 5–10 s clip + its transcript.
- Model and code belong to Nari Labs (Apache-2.0). Do not use for impersonation or deceptive content.

## Web UI
Section 6 of the notebook launches a Gradio UI (public link) with: script editor, non-verbal tag buttons,
voice cloning, seed/CFG/temperature/top-p/top-k/max-tokens controls and automatic chunking for long scripts.
