# Small Wins

A small Flask task list. Tasks are saved in the current browser's local storage; the server does not use a database or store task data. Browser storage does not sync between devices or browsers.

## Run locally

```powershell
python -m pip install -r requirements.txt
python app.py
```

Open <http://localhost:5000>.

## Run with Docker

```powershell
docker build -t small-wins .
docker run --rm -p 5000:5000 small-wins
```

Open <http://localhost:5000>. A container host can set `PORT`; the app binds to that port automatically. The `/health` endpoint returns the app's health status.
