# Archived: math tutoring page (taken down 2026-10-15)

Spencer stopped tutoring, so the page and every link to it came off the site. This folder keeps
them for reference. Jekyll does not build it: its name starts with an underscore and it is not in
the `include:` list of `_config.yml`, so nothing here is published.

## To bring it back

1. Move `tutoring.md` back to `_pages/tutoring.md`. Its permalink is `/tutoring/`.
2. Add the menu entry back to `_data/navigation.yml`, between "Research" and "CV":

   ```yaml
     - title: "Tutoring"
       url: /tutoring/
   ```

3. Put this sentence back into the Bio in `_pages/research.md`, after the first sentence:

   ```html
   I also offer math tutoring services, online and in-person in the New York City area (<a href="/tutoring/">see here</a>).
   ```

4. Update the dated wording on the page ("Slots open for Summer 2026!", "Summer slots available!").
5. Build with `bundle exec jekyll build`, check `_site/tutoring/`, then commit and push.
