# Daily pipeline

Goal: collect new AI work every day so writing never starts with hunting for examples. Collect and organize only.

## Archive tabs
- **Sessions:** date | platform(s) | project | what happened | decision / outcome | link
- **Her Words:** verbatim line | date | project | lane | starred (starred is left blank for the human)
- **Media:** image link | what it shows | what capability it proves | project | used/unused | source | date
- **Lanes:** lane name | status (seed / developing / drafted / published) | evidence so far | what is missing | supporting projects
- **Dashboard:** Metric | Number | Status | Explanation
- **Run Log:** date | platform | chats found | chats archived | prompts counted | status | notes

## Steps
1. Read saved state (last successful run per platform). A platform with no prior run, or a failed one, looks back 14 days.
2. Read existing Session links so the same chat is never added twice.
3. For each platform, independently: list conversations updated since the last run, keep project-related ones, skip personal ones, record decisions, artifacts, failures and discoveries, and copy the human's own opinions verbatim. A failure on one platform is logged and does not stop the others.
4. Merge duplicate episodes across platforms into one Sessions row; note which models were used and why the switch happened.
5. Sort episodes into lanes, reusing existing lanes before creating new ones. Update "evidence so far" and "what is missing" using only facts in the rows.
6. Update dashboard counts (prompts counted, conversations, platforms) in the fixed four-column format. A platform that failed shows Unavailable instead of a guess.
7. Append one Run Log row per platform and advance a platform's timestamp only if it was actually read.
8. Finish with a five-line summary: what was added, new lanes, what failed.

## Status vocabulary
- `no new activity`: nothing changed since last run, or everything changed was personal and skipped (count noted). Not a failure.
- `failed`: the platform could not be read (logged out, would not load). A suspiciously empty list on a platform used recently is double-checked once before being called quiet.

## Data access
Each platform is read through my own logged-in session or its official data export. Account tokens, internal endpoints and identifiers are not part of this repository. Prefer official exports where a platform offers them.
