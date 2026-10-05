# Office File Reader

> Reads text and table contents from Word, Excel, and PowerPoint files by parsing their internal XML structure without requiring Office applications.

The bundle zip (**29.6 MB**) is stored in this repository at **`74991031-7860-42d5-b8fb-de8a1172914d.zip`**.

This repository is part of the **Forjinn-Desk** MCP bundle collection. An MCP bundle is a self-contained server that a host application launches and communicates with over the MCP (Model Context Protocol) protocol.

## Repo metadata

| Field | Value |
| --- | --- |
| Registry ID | `74991031-7860-42d5-b8fb-de8a1172914d` |
| Status in registry | inactive |
| Bundle size | 29.6 MB |
| Distribution | committed to this repo |

## Environment variables

| Variable | Value / note |
| --- | --- |
| _(none)_ | _no required environment variables_ |

## MCP launch configuration

The host replaces `__INSTALL_DIR__` (install dir) and `__PYTHON__` (bundled Python) at runtime.

```json
{
  "command": "__PYTHON__",
  "args": [
    "server.py"
  ]
}
```

## Setup / usage notes

No special setup required. The tool reads .docx, .xlsx, and .pptx files directly by parsing their internal XML structure. Ensure the file paths provided are correct and the files are valid Office Open XML format files.


## Install / usage

1. Get the bundle:
   - download `74991031-7860-42d5-b8fb-de8a1172914d.zip` from this repo (Code → Download ZIP, or `git clone`).
2. Extract to your target installation directory (config paths expect contents at the install-dir root).
3. Set the environment variables listed above.
4. Launch using the MCP config JSON (or let a host client manage it automatically).

> Bundles may include vendored runtimes (bundled Python, Node, or native executables). Builds are Windows x64.
