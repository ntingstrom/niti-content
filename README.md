# Niti Content

This repository contains content used by Framer code components. The data files
are fetched from the raw GitHub URLs and rendered inside Framer.

## Code Components

The `src/NitiContent.tsx` file exposes a set of React components:

- `About` – renders the `about.md` file using Markdown
- `Projects` – shows projects from `projects.json` as cards
- `Articles` – lists articles from `articles.json`
- `YouTubeVideos` – embeds videos defined in `youtube.json`
- `NitiContent` – convenience component showing everything together

These components fetch the latest version of each file from GitHub and display a
loading state and error state by default.

### Usage in Framer

1. Install the `marked` package in your Framer project for Markdown support.
2. Copy the `src/NitiContent.tsx` file into your Framer code section.
3. Import and place any of the exported components on your canvas.

```tsx
import { NitiContent } from "./NitiContent";
```

Feel free to style the components further to match the Rescale theme.
