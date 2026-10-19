# hello-world

i'm new to github
hoping to learn a lot through all of this
my name is folarin oluwatodimu adedotun

## Full stack web development projects

Three independent local portfolio projects, each with a responsive JavaScript frontend, a Python JSON API and a persistent SQLite database.

| Project | Features | Start command from repository root |
| --- | --- | --- |
| [Taskflow](projects/taskflow) | Task CRUD, priorities, due dates, status filters and progress | `python projects/taskflow/server.py` |
| [Pocket Ledger](projects/pocketledger) | Income/expense CRUD, categories and NGN totals | `python projects/pocketledger/server.py` |
| [Stockroom](projects/stockroom) | Product CRUD, unique SKUs, stock levels and inventory valuation | `python projects/stockroom/server.py` |

### Getting started

1. Install Python 3.10 or newer.
2. Clone or download this repository.
3. Run a command from the table above (`py` can replace `python` on Windows).
4. Open the localhost URL printed in the terminal: ports 8001, 8002 and 8003 respectively.

No external dependencies, API keys, build tools or pip installation are required. Each project creates its own database automatically. Records survive restarting the server. All apps can run together on their separate ports.

### Repository layout

Each project contains `server.py` (backend and SQL schema), `project.json` (field definitions), `public/index.html`, `public/styles.css`, `public/app.js` and a README with its API documentation.

### Validation

```sh
python -m unittest discover -s tests -v
```

The HTTP integration tests use temporary databases and cover creation, reads, updates, deletion, persistence across schema initialization, invalid input, SKU uniqueness and static file access restrictions.

### Project scope

These are single-user learning projects that run locally, with no login or user isolation. Public deployment needs authentication, a production server and database hosting. Uploading the source to GitHub does not create a running website; GitHub Pages cannot execute the Python APIs.
