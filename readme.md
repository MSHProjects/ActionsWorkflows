# General workflows

```bash
├── .github
│   └── workflows
│       ├── sonar-node.yml
│       ├── sonar-python.yml
│       └── staging-deployment.yml
└── readme.md
```

## How to launch the scanner-node 

```bash
curl -XPOST -u "MohamedSoulaimenHammami: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" \
  -H "Accept: application/vnd.github.everest-preview+json" \
  "https://api.github.com/repos/MSHProjects/ActionsWorkflows/dispatches" \
  -d '{"event_type": "sonar-scan", "client_payload": {"OWNER": "iovision-io","REPOS": "gpt-review","PAT": "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","REF": "bugs","node_version": "16" , "projectKey":"TRIGGER" , "projectBaseDir": "src/"}}'

```