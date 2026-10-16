# Pursor for Claude

Read a client's finance work from Pursor inside Claude Code, Cowork or
claude.ai: what needs a person today, where the month-end close stands,
every account the close reconciles, one account's view for a month, the
open cashflow sheet, and a question put to the ledger through Pursor's
Ask.

It reads. Nothing here posts, drafts, codes, signs or moves a card.
Every verb stays on the card in Pursor, with its trail and its Undo, and
every answer ends with the link to the page that holds it.

## Getting Pursor

Pursor is set up for your company by your accounting firm or by us; to
start, talk to us at https://pursor.com/contact. The plugin reads an
account you already have.

## Install

```
claude plugin marketplace add pursorapp/claude-plugin
claude plugin install pursor@pursor
```

The first call opens pursor.com: sign in, approve, and from then on
Claude reads Pursor as you. In claude.ai or Cowork, add
`https://pursor.com/api/mcp` as a custom connector instead.

## What it reads

Exactly what you can see in Pursor, as you. A person at the client reads
their own company; a person at the servicing firm reads the clients the
firm lets them see. Payroll's cards and its page are never read from here.

## What it records

Every tool call is recorded under your name: which tool, which client,
how long. A question through Ask is recorded as Pursor's Ask records
every question. Nothing is shared with anyone else.

## Disconnect

On your Team page in Pursor, your row reads "Connected to Claude ·
Disconnect". Signing out everywhere ends it too. In Claude Code,
`claude mcp logout pursor`.

## Tools

| Tool | What it returns |
| --- | --- |
| `clients` | The clients you can see, with what each needs today |
| `today` | What needs a person at a client today, one line per card |
| `card` | One card whole, with its reason, its cause where Pursor investigated, and the verb it carries |
| `close` | The month's close: which day of five, the five steps, the rows of one |
| `reconcile` | Every account the close reconciles, one line each, with one of five words |
| `account` | One account's view for a month: the books against the bank or the rail |
| `cashflow` | The open sheet: the week, the low point, week one, what moved since last week |
| `ask` | A question to the ledger through Pursor's Ask, read-only, recorded |

Documentation: https://pursor.com/plugin
