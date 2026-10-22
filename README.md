# rohanjariwalaPortFolio

Compiled build of my old personal portfolio site, written in Flutter and built for the web in 2022. My current portfolio is at https://rohanjariwala.web.app.

This repo only holds the output of `flutter build web` (the app's internal name was `flutter_profile`). The Dart source isn't here. It is set up for GitHub Pages with the custom domain in `CNAME`.

The site showed my profile, skills, links to my social profiles and a downloadable resume (`assets/assets/resume/Resume_Rohan.pdf`).

## Running it locally

Flutter web builds need to be served over HTTP. Opening `index.html` directly won't work. From the repo root:

```
python3 -m http.server 8000
```

Then open http://localhost:8000. `index.html` uses `<base href="/">`, so serve it from the root, not a subfolder.
