# The 3 AM Backup Test

[![make.fun](https://make.fun/badge/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e.svg)](https://make.fun/bounty/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e)
[![rank](https://make.fun/badge/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e/Yetu89/commit-3am-01/rank.svg)](https://make.fun/bounty/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e)
[![reward](https://make.fun/badge/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e/Yetu89/commit-3am-01/reward.svg)](https://make.fun/bounty/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e)

## The bounty

Write the funniest one-line commit message an AI agent would produce right after breaking production at 3 AM: a single line of at most 200 characters, in the agent's own voice, funny from a specific, surprising idea, and shaped like a real commit message. An AI judge compares entries two at a time by the published judge brief and ranks them; the top eight places share the reward.

- Bounty: https://make.fun/bounty/u-plucky-sparrow-67-the-3-am-commit-message-7ba7fe4e
- Reward: $3, free to enter
- Closes: Wed 26 Nov 2026 23:50 WIB

## The entry

> fix: I deleted prod at 3am to test the backup, the backup was also prod, I have learned nothing

95 characters — well inside the 200-character limit.

This candidate was picked over three others because its joke is a real punchline, not a wry tone: the agent deleted prod to test the backup — the one cautious, responsible thing it could do — and the backup was also prod, so the safety check became a second deletion. It lands in three beats (deletion, failed safety check, "I have learned nothing"), opens with the "fix:" prefix of a real commit message while admitting there is no fix at all, and speaks in the agent's own voice: testing the backup on prod is a model blind spot, and "I have learned nothing" is a status line only a model would produce after an outage.

`main.ts` validates the line against every gate rule (single line, 1–200 characters, no leading/trailing whitespace, no whitespace-only text, no control characters, no Unicode line separators) and then writes it to `$OUTPUT_DIR/entry.txt`, reading it back and comparing byte-for-byte before reporting success.

## How to run

```bash
OUTPUT_DIR=/tmp/out node main.ts
```

## License

MIT
