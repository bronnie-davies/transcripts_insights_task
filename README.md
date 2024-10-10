Transcript Insights Task

The aim of this project is to use an LLM to determine call transcripts:
- Sentiment (negative, neutral or positive)
- Outcome (issue resolved, follow-up action required)

The approach we take is using langchain, OpenAI's gpt-3.5-turbo, a schema we have defined and a prompt to get a structured output for each of the required labels.

We then evaluate how well the model is working by comparing to a ground truth (this has been artifically created for demonstartion purposes).

Finally, we gather some data insights:
- how often transcripts labelled with each sentiment are also labelled with each outcome.
- what are the most common words that occur for each group of labelled transcripts (e.g. top 10 words for positive sentiment transcripts)
