# Two-Player Word Game

A local two-player word-building game delivered as a Streamlit web app.

## Rules

- Two players enter their names before the game starts.
- There is a shared pool of 100 points.
- On each turn, roll the dice and select up to that many letters, spaces, or punctuation marks.
- Each selected character uses one point from the shared pool.
- `Repeat` removes the most recent selection made during the current turn.
- `Done` ends the current turn.
- Selecting `SPACE` displays `_` until another character is selected.
- When all 100 points have been used, valid English text and the higher score determine the winner.

## Run locally

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
streamlit run app.py
```

On Windows PowerShell, activate the environment with:

```powershell
.venv\Scripts\Activate.ps1
```

## GitHub and Streamlit Community Cloud

1. Put all repository files in one folder.
2. Create a private GitHub repository and push the folder.
3. In Streamlit Community Cloud, choose **Create app**.
4. Select the private repository, branch, and `app.py` as the entry point.
5. Deploy.

The Streamlit account must have permission to access the private GitHub repository.
