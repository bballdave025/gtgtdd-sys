# Gather Capture Protocol

## Purpose

Make raw GTD capture available from any ChatGPT conversation without turning
capture into planning.

The governing distinction is:

> **Gather first. Clarify later.**

A gathered item is not yet a project, next action, or durable reference item.

## Trigger language

Treat any clear request using language such as the following as a raw GTD
capture request:

- `gather`
- `capture`
- `inbox`
- `GTD this`
- equivalent language that clearly means “catch this now; process it later”

Do not require Dave to invoke a special command syntax.

## Canonical raw-capture location

Google Drive:

`My Drive / __General_Reference / _INBOX_SCANS`

Folder:
https://drive.google.com/drive/folders/17f5O5kCc0QuT03Eqwcs9CGVm6Qfm8OaE

## Default behavior

For each atomic gathered thought, create one plain UTF-8 text file in
`_INBOX_SCANS`.

Filename convention:

`GATHER_YYYY-MM-DD_-_<short-readable-slug>.txt`

Keep the file intentionally small:

```text
GTD GATHER
Captured: YYYY-MM-DD
Status: UNPROCESSED

<captured thought>
```

Preserve Dave's meaning and useful wording. Minimal cleanup is fine. Do not
research, decompose, prioritize, schedule, or otherwise clarify the item merely
because it was captured.

## One file per item

Default to one file for each atomic gather item. The visible accumulation of
small files is intentional light pressure to process the inbox daily or weekly.

Do **not** combine new captures into a growing master file by default.

If the inbox becomes noisy, combine a batch during review only when Dave asks
or when doing so clearly helps processing. Do not redesign the capture system
merely because several files exist.

## Asana boundary

Asana is canonical **actionable** state after clarification.

A raw gather does not need a duplicate Asana task by default.

Create or update Asana immediately only when:

1. Dave explicitly asks for the item in Asana as well; or
2. inbox processing has clarified the capture into a Next Action, Project,
   Waiting For, Calendar item, or other actionable state.

This prevents two competing raw inboxes while preserving Asana as the trusted
system for actions.

## Processing / clearing

During daily or weekly inbox processing, each gather file should resolve to one
of the normal GTD outcomes:

- Next Action
- Project
- Waiting For
- Calendar
- Someday/Maybe
- Reference
- Trash

After the clarified outcome is recorded in its canonical home, remove or move
the raw capture file so `_INBOX_SCANS` visibly shrinks.

## Cross-chat rule

Any chat working under the uGTgtdD system should honor this protocol when Dave
uses gather/capture/inbox language. Domain chats do not need to own the later
clarification; their job at gather time is simply to preserve the thought in
the raw inbox and return to the domain trunk.

If a chat cannot write to Google Drive, it should state that limitation and
capture the text in the current conversation for later transfer rather than
silently pretending the Drive file exists.

## Anti-cathedral rule

Do not add tags, hashes, IDs, manifests, schemas, or elaborate metadata unless
a real retrieval problem appears.

The success criterion is simple:

> Dave can say a thought once, trust that it was caught, and process it later.
