# action-repo
This repository is used only for testing GitHub Webhook events such as:

- `push`
- `pull_request`
- (Optional) `merge`

These events are sent to a separate backend (`webhook-repo`) using a GitHub webhook.

---

## Purpose

The goal of this repository is to generate webhook payloads by:

- Making commits and pushing to branches
- Opening pull requests from one branch to another
- Merging pull requests (optional, for extra credit)

All events are sent to a webhook URL configured in the repo settings.

---

## Usage

You can perform the following actions to trigger webhooks:

### 1. Push

```bash
git add .
git commit -m "your commit message"
git push origin branch-name
