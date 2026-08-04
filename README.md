# Adding a project

The portfolio is data-driven: add a project to `projects.json` and it appears automatically on the Work page and receives its own shareable detail URL.

1. Add any new images to `assets/engassets/<project-name>/`.
2. Duplicate an object in `projects.json` and update its values. The `id` must be unique and URL-safe (for example, `solar-tracker`).
3. Use paths beginning with `../../assets/` because the data is loaded from `pages/projects/`.
4. Add the strongest image to `image` and `heroImage`, then include supporting images in `gallery`.

The resulting project URL is:

```
project.html?project=solar-tracker
```

You do not need to create another HTML page for each project. The shared `project.html` template uses the project data to render a consistent case study.
