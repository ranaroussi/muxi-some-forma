# some-forma

A new MUXI formation

Created with MUXI CLI.

## Structure

- `formation.yaml` - Formation configuration
- `agents/` - Agent definitions
- `mcps/` - MCP server configurations
- `a2a/` - Agent-to-Agent communication configs
- `sops/` - Standard Operating Procedures
- `triggers/` - Event triggers
- `knowledge/` - Knowledge base documents
- `secrets.enc` - Encrypted secrets
- `.key` - Encryption key (**never commit!**)

## Getting Started

1. Configure secrets (if not done during init):
   ```bash
   muxi secrets setup
   ```


2. Validate formation:
   ```bash
   muxi validate
   ```


3. Deploy:
   ```bash
   muxi deploy --profile production
   ```


## Adding Components

```bash
muxi new agent my-agent
muxi new mcp my-mcp
muxi new sop my-procedure
muxi new trigger my-trigger
muxi new a2a external-api
```


## Development

Edit `formation.yaml` and component files, then:

```bash
muxi validate          # Check configuration
muxi deploy --profile localhost  # Test locally
```

