# AGENTS.md for my ticketing system

## Ticket description

- Read the `./TICKET.md` file for an example of how a ticket should look
- The only required sections of a ticket are:
  - `Key` - the issue key and a summary
  - `Description` - a longer description of the issue/task
- All other fields are optional. These include:
  - `PRD` - A formal PRD describing the solution. See `./PRD.md` for an example of how a PRD should look.
  - `Plan` - The implementation plan created by an AI agent which details the work required to fulfill the PRD.
    - `Relevant files` - a required sub-field of `Plan` which lists all the files to edit or create to fulfill the PRD.
    - `Notes` - an optional sub-field of `Plan`, with important reminders or teting commands
    - `Subtasks` - A list of subtasks, if any.
  - `Comments` - Comments with date/time stamps describing work done or other relevant information.
  - `PRs` - a list of branches and PR urls

## Instructions
- When appropriate, or when asked, move a Ticket file from `todo` to `in-progress` or `done`. New tickets always land in `todo`.
- Never run read/write `git` commands; run _only_ readonly `git` commands if needed. It will probably not be needed.
- *Never* delete or alter the `Key` or `Description` sections. Consider those readonly.
- Always re-read the `Description` field of a ticket, in case it has changed.
- *Do* add/alter `PRD` and `Subtasks` fields
- *Always* alter the `PRD` field according to the `./PRD.md` template.
