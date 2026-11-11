# hermes-rg

Comment `/rg <commit-sha> [base=<sha>] [tests=<path>,...]` on the Red/green requests issue. The workflow fetches the commit from kvnloo/hermes-agent or NousResearch/hermes-agent, runs its changed tests at the commit (GREEN) and with its source changes reverted to `base` (RED; default = the commit parent), and replies with the verdict. Post an add-on upstream only when the verdict is **DISCRIMINATES**.
