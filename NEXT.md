# Next

Updated: 2026-11-25

## Where it stands

ELIZA, a recreation of Joseph Weizenbaum's 1960s ELIZA running the DOCTOR script. Built 2 to 6 March 2025 as the sample agent for the Union College course History and Future of Technology Innovation in the Bay Area (Winter 2025). The chat page still publishes at eliza.aroughidea.com, but it does not answer: `pages/api/proxy.js` sends every message to a ZeroWidth agent, and ZeroWidth is gone. The agent's system instructions and knowledge base lived in ZeroWidth, not here. The owner decided on 2026-11-25 to rebuild it.

What survives of the agent:
- `config/config.js`: the opening line ("HOW DO YOU DO. PLEASE STATE YOUR PROBLEM.") and the suggested prompts.
- The Google Doc "Embedding an Agent in a website" (March 2025): the request and reply shape. Each reply was JSON with `response` (in capitals), `reasoning` and `references`; the recorded reply cited Weizenbaum 1976, Turkle 2011 and Carr 2010.
- Photos of the ELIZA exhibit, 21 February 2025, in Drive: the 1966 transcript, Norbert Landsteiner's 2005 implementation, and a Weizenbaum quote.

## Next step

Rebuild the agent without ZeroWidth: replace the ZeroWidth call in `pages/api/proxy.js` with one this repository controls, keep its instructions and knowledge in the repository, and keep the reply shape above, so eliza.aroughidea.com answers again. Use the owner's notes if he finds them.

## After that

- Remove ZeroWidth from the README, `.env` names and comments.
- Rename the repository (the owner asked on 2026-11-25), then update the register to the new name.

## Blocked or waiting

- The owner is looking for his notes: the original system instructions and knowledge base.

## Open questions

- Should the rebuild be a language model playing ELIZA, as the ZeroWidth agent was, or Weizenbaum's own DOCTOR script as he published it in 1966 (keywords, decomposition and reassembly rules), or both side by side?
- The new name for the repository.
