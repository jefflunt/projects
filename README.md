- `projects` (the repo, and the general framework)
    - `build` (`.build/` folder)
    - `agent_docs/`
    - `scripts/` folder (built, test, install, build-test-install, curl-install,
      release)
    - `.github/workflows` actions for build + release (see `breakdown`)

AI orchestration
- build: the orchestrator itself
    - integrate `agent`
    - extract current hardcoded workflow into a yaml workflow, then make
      workflows configurable (a planning workflow, a simple building workflow, a
      complex building workflow)
    - start supporting a `planning` state where I can iterate on a design until
      I'm ready to hand it off for implementation
        - agent: cli interface to multiple cli agent harnesses (gemini, opencode,
          claude, etc.
    - seems to work, need to finish integrating it into various tools
    - breakdown: take a plan file and make a project tree out of it
        - integrate `agent`
    - contextual: fetch context for agents
        - not all content from Jira pulled in; test against:
        - tables
        - code blocks
        - attachments

games:
- infinimaze: infinite online mazes
  - review where we're at
  - publish, start creating content for it
- keys: 10-key competitive game
  - review where we're at
  - publish, start creating content for it
- taipan / plunder and profit

tools:
- stat: the fast real-time stat aggregator
- remark: promote this
- markdown-viewer: promote this
- money: do I still want to do anything with this?
- txnal apps
    - mail: gmail client, spam blocker, data extractor
        - build the spam blocker first
    - mailer: sent email
