# Hive Quiz — Learn. Play. Share.

A buildless, browser-only Hive knowledge quiz. 60 original beginner questions, 25/50 question rounds, shuffled questions and answers, immediate or end-of-quiz feedback, source-linked review, topic breakdown, missed-question practice, and downloadable square/wide PNG scorecards. Official Hive assets from https://hive.io/brand/.

## GitHub Pages

1. Create a public repository named `hive-quiz`.
2. The application files are already at the repository root.
3. In Settings → Pages, select Deploy from a branch, `main`, `/ (root)`.
4. Set `publicUrl` in `config.js` to the final public Pages URL.
5. Update `og:image` in `index.html` to `https://YOURNAME.github.io/hive-quiz/assets/social-preview.png`.

No installation, build, API credentials, or Hive wallet is needed. Serve files over HTTP; opening index.html with file:// cannot fetch the JSON bank.

## Challenge configuration

In `config.js`, set `challengeUrl` to the Hive announcement and `challengeEndsAt` to its payout deadline as an ISO timestamp including timezone. Both must be set before the challenge is shown as active. Example format: `2026-11-12T18:00:00+02:00`. The page automatically switches to a closed message at the deadline. Add `hiveProfileUrl` for the feedback link. Discord contact: `katerinaramm`.

The quiz does not post, validate identities, verify scores, or cast upvotes. Results are self-reported and publicly inspectable. Missed-question practice is labeled on its result card. Run the challenge manually under your post rules. A 100% upvote does not promise any fixed payout.

## GoatCounter

GoatCounter is configured with `https://hive-quiz.goatcounter.com/count` using the async script at `//gc.zgo.at/count.js`. The footer discloses visit analytics. The optional name, quiz answers, and scores are not included in the analytics configuration.

## Question bank

Edit `questions.json`. Each question needs a unique id, topic, difficulty, type, question, four distinct options, answer index (0-based), explanation, and HTTPS source URL. At least 50 questions are required. Do not remove source links. Review source material for protocol changes; some glossary and FAQ details can be historical. This initial bank avoids rates, reward percentages, and protocol parameters likely to change.

Keep at least 50 questions with unique IDs and valid answer indexes.

## Limits

Browser sharing support varies. Download PNG and copy text are fallbacks. Desktop X posts require attaching the downloaded image manually. Link previews are fixed; scorecards are not remotely hosted. Preferences use local storage. Names and answers are held in memory and are sent only when the user explicitly shares. Reloading loses an in-progress quiz. No accounts, timer, leaderboard, or verified score database.

## Files

The repository root contains the complete publishable application.
