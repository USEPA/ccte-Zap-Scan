# ZAP GitHub Action

This GitHub Action performs application security scans using OWASP ZAP (Zed Attack Proxy).

## Inputs
- `zap_token`: ZAP API token for authentication (required).
- `zap_target`: Target URL for the ZAP scan (required).
- `zap_format`: Format for the ZAP scan (default: `openapi`).
- `zap_cmd_options`: Additional command options for ZAP (optional, default: `-a`).

## Example Usage
```yaml
uses: your-username/zap-github-action@v1
with:
  zap_token: ${{ secrets.GITHUB_TOKEN }}
  zap_target: 'https://your-target-url.com'
  zap_format: 'openapi'
  zap_cmd_options: '-a'
