# 🛡️ Guard Panel

A customized black & white themed subscription management panel (based on SulgX Panel v1.1.0).

**Changes from original:**
- Renamed to **Guard Panel**
- Theme changed from green to elegant **black & white** with enhanced glassmorphism buttons
- All "free / رایگان" references removed and replaced with "Your Subscription"
- Fully compatible with **Railway**, Render, and other platforms

## Deploy on Railway (Recommended)

1. Create a new project on [Railway](https://railway.app)
2. Deploy from this folder (or connect Git repo)
3. Add a **Volume** mounted at `/data`
4. Set environment variables:
   - `ADMIN_PASSWORD` = your strong password (min 8 chars, upper+lower+digit)
   - `SECRET_KEY` = any long random string
   - `DOMAIN` = your Railway public domain (e.g. `xxx.up.railway.app`)
   - `DB_PATH` = `/data/panel.db`
5. Open `https://your-domain/panel` and login

The included `Dockerfile` + `railway.toml` ensure zero-config build.

## Local Run

```bash
pip install -r requirements.txt
export ADMIN_PASSWORD=YourPass123
python main.py
```

Then open http://localhost:8000/panel
