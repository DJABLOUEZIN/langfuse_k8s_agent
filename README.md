# AWS and Kubernetes chat assistants

Two chat assistants that answer questions about real infrastructure and never change it.

| Folder | Reads | Through |
|--------|-------|---------|
| [kubernetes-assistant/](./kubernetes-assistant/) | A Kubernetes cluster | A Kubernetes MCP server on your laptop |
| [aws-assistant/](./aws-assistant/) | An AWS account | The AWS MCP Server |

Both folders start empty. You build each app file by file, following its lab guide in
[docs/](./docs/).

## Get started

```bash
git clone https://github.com/utrains/langfuse-aws-k8s-agent.git
cd langfuse-aws-k8s-agent
```

Then open [docs/kubernetes-assistant-lab.pdf](./docs/kubernetes-assistant-lab.pdf) and start at step 0.

## Langfuse lab

The Langfuse observability lab adds tracing, prompt versioning, scores and experiments to the
Kubernetes Assistant. Its guide is online at https://kodelumi.com/w/AVWkaKxQo3zaT28p: start with
`getting-started-with-langfuse.md`, then follow `lab.md`. [langfuse-setup/](./langfuse-setup/) runs
Langfuse on your laptop.

## Settings and credentials

Each folder gets its own `.env` file, because each app reads different settings. You create it
during the lab.

Git ignores every `.env` and every `kubeconfig` in this repository. Never commit either one: they
hold your Anthropic key and your cluster token.
