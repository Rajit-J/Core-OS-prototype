# Core-OS Dashboard

A local Flask dashboard prototype backed by SQLite. It brings task, habit, budget, wellness, and related dashboard views into one browser interface.

## Technology

- Python and Flask
- SQLite
- HTML, CSS, and JavaScript

## Run locally on Windows

From the repository root in PowerShell:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install Flask
$env:PORT = "5102"
python dashboard_app\app.py
```

Open [http://127.0.0.1:5102](http://127.0.0.1:5102). Stop the server with **Ctrl+C**, then run `deactivate`.

The app creates and uses a local `dashboard.db` in the current working directory. Start it from the repository root. This database is local application data and should not be committed.

## Configuration and limitations

This is a local prototype, not a hardened multi-user service. Configure a secure session secret outside the repository before any deployment, and do not use real personal or financial information in the demo.

## Before publishing

Exclude SQLite databases, virtual environments, caches, and logs. Review configuration and sample data for personal or environment-specific information. No license is included; confirm ownership and license terms before adding one.
