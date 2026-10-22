# Self Hosted Transcripts — Pipeline

The archive is built by 4 scripts run in numeric order. `main.py` is a thin runner that calls each one in turn with the arguments you gave it, so running a stage by hand and letting `main.py` do it are equivalent.

| Stage | Script | What it does | Resume log |
|---|---|---|---|
| 1 | `1_download.py` | This script uses yt-dlp to download audio, by year, from the Self Hosted podcast website playlist. | — |
| 2 | `2_transcriber.py` | This script transcribes audio files from the Self Hosted podcast episodes using OpenAI's Whisper model. | `transcribed.log` |
| 3 | `3_summarizer.py` | This script summarizes a transcript file by splitting it into manageable chunks, summarizing each chunk using the Ollama API, and then combining the summaries into a final summary. | `summarized.log` |
| 4 | `4_cleanup.py` | This script processes all .txt and .md files in the current directory, correcting their grammar and spelling using LanguageTool. | `cleaned.log` |

## Running a single stage

Every stage takes the same arguments as `main.py`, so any one of them can be re-run on its own without repeating the stages before it:

```bash
python 1_download.py <year>
```

## Re-running and resume logs

The expensive stages append to a log file as they finish each item, and skip anything already listed there on a later run. That is what makes the pipeline resumable after an interruption.

| Log | Written by |
|---|---|
| `transcribed.log` | `2_transcriber.py` |
| `summarized.log` | `3_summarizer.py` |
| `cleaned.log` | `4_cleanup.py` |

Delete a log to force its stage to redo everything.

## A note on accuracy

Transcription and summarisation are both lossy. Neither the transcripts nor the summaries in this repository are an authoritative record — check the original recording where it matters. See [`CONTENT_LICENSE.md`](../CONTENT_LICENSE.md).
