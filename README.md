# STPi Video Repository (`stpi-cloud/stpi-videos`)

This is the dedicated video sub-repository for the **STPi Social & Press Autopilot (`press/auto.py`)**.

## How Video Posting Works
1. **Upload any `.mp4` (or `.mov` / `.webm`) file into this repository** (via the GitHub web interface **Add file → Upload files** or `git push`):
   - `shorts/` — vertical or short-form videos (ideal for **YouTube Shorts, TikTok, Instagram Reels, Facebook Reels, Threads**)
   - `long/` — full-length horizontal videos (ideal for **YouTube, Facebook Page, LinkedIn, X**)
   - `company/` — videos restricted to Company Buffer accounts only
   - `seller-a/` or `seller-b/` — videos restricted to Seller A or Seller B Buffer accounts only
   - Or simply drop `.mp4` files directly in the root `/` — the engine discovers every `.mp4` automatically!
2. **Optional Custom Caption / Title:**
   - Upload a matching `.txt` or `.md` file with the same name (e.g., `shorts/my-clip.txt` alongside `shorts/my-clip.mp4`), OR add an entry to `manifest.json`.
   - If you only upload the `.mp4` file with no `.txt` file, `press/auto.py` automatically generates a platform-tailored title and caption from the filename + topic pool and validates it through our hard copy gates.
3. **3-Buffer-Account Routing (Identical for Company & Every Seller):**
   - **Buffer Account A (`STPI_BUFFER_TOKEN_A_CO` / `STPI_BUFFER_TOKEN_<S>_A`):** X (`x`), LinkedIn (`linkedin`), Pinterest (`pinterest`)
   - **Buffer Account B (`STPI_BUFFER_TOKEN_B_CO` / `STPI_BUFFER_TOKEN_<S>_B`):** Facebook Page (`facebook`), Instagram (`instagram`), Threads (`threads`)
   - **Buffer Account C (`STPI_BUFFER_TOKEN_C_CO` / `STPI_BUFFER_TOKEN_<S>_C`):** YouTube (`youtube`), TikTok (`tiktok`), Google Business Profile (`gbp`)
