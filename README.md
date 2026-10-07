# ATG Rollout Tracker

Progress dashboard for the Automatic Tank Gauge (ATG) rollout across 1,000 retail outlets in Pakistan:
site surveys, site readiness, ATG installation, tanks and service ports, field teams, and a map.

## Opening the dashboard

Open the GitHub Pages address of this repository and enter the dashboard password.
Ask the administrator for the password. It is never stored in this repository.

## What is in this repository

| File | Contents |
|---|---|
| `index.html` | The dashboard and the Pakistan map. Site data is encrypted with the password (AES-256-GCM). |
| `status.enc` | Survey, readiness and installation status, field teams and the activity log, encrypted with the same password. |
| `robots.txt`, `.nojekyll` | Keep search engines out and serve the files as they are. |

Without the password, both files are unreadable.

## Admin: saving changes

1. On github.com open **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. **Repository access:** *Only select repositories* → this repository.
3. **Permissions → Repository permissions → Contents:** *Read and write*.
4. In the dashboard click **Admin**, paste the token and sign in.

Every change (survey done, site ready, ATG installed, teams, notes) is saved into `status.enc`.
Other viewers see it within about a minute, or when they reload the page.
