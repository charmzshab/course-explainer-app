# Videos Tab — Implementation Checklist

- [x] Add `PLAYLIST_ID` / `PLAYLIST_EMBED_URL` constants to `src/models.py`
- [x] Add `videos()` view function to `src/views.py`
- [x] Register `/videos` route in `src/app.py`
- [x] Create `src/templates/videos.html` with responsive iframe embed
- [x] Add "Videos" nav link to `src/templates/layout.html`
- [x] Add `.videos-section` / `.video-embed-wrapper` CSS rules to `src/static/css/styles.css`
- [x] Extend existing 768px and 480px media queries for the videos section
- [x] Add `test_videos_page_loads` and `test_nav_includes_videos_link` to `tests/test_app.py`
- [x] Run `python -m unittest discover -s tests` — all 14 tests pass except a pre-existing, unrelated `test_index` failure (already broken on `main` before this change)
- [x] Start Flask app and verify `/`, `/videos`, `/contact` all return 200, nav link present, no `BuildError` (verified via curl)
- [ ] Playwright MCP visual screenshot verification — **skipped**, Playwright MCP tool not available in this environment. Manual visual check still recommended.
