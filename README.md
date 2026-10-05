# AutonBDA / Agentic Autom-BDA

An extension of the published **Autom-BDA** automatic service composition framework
(AutoBDA, *IEEE Transactions on Services Computing*, 2025) in which AI agents replace
some services of the analysis pipeline.

## Live demonstration

**https://agentic-autobda-617217495376.asia-northeast1.run.app**

Sign up, upload a CSV file naming its target column, and describe the analysis goal in
words: an agent drafts the analysis settings, with a reason for each. Approve them, and the
pipeline runs with three registry services performed by AI agents (Google Gemini), beside a
conventional twin run for comparison. AutoBDA's own screens for the same runs are at
`/autobda` on the same site.

Agent calls are rate-limited. The service sleeps after about 15 minutes without visitors and
then starts clean: accounts and runs are kept only while it is awake, and the first visit
after a quiet spell takes a few seconds longer.

![Agentic AutoBDA demonstration](demo/agentic-autobda-demo.gif)

[Full-quality video (MP4)](demo/agentic-autobda-demo.mp4)

## Status - 2026-10-06

| | |
|---|---|
| Prototype | live, on Google Cloud Run (Tokyo) |
| Source code | maintained in a private repository |

## License

Apache-2.0.
