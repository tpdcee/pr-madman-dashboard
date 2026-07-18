# PR & Influence Dashboard

A lightweight GitHub Pages dashboard for viewing the Madman PR & Influence team's Google Calendar schedules in one place.

## Live dashboard

The site is published through GitHub Pages from the repository's `main` branch.

## Calendar owners

| Color | Team member |
| --- | --- |
| `#0B8043` | JB Suarez |
| `#D81B60` | Ally Martinez |
| `#EF6C00` | Celine Balbuena |

## Updating team members

1. Add or remove the relevant `src` calendar parameter in the iframe URL inside `index.html`.
2. Add or remove the corresponding `color` parameter in the same order.
3. Update the legend markup and CSS color variable.
4. Confirm that the calendar color and legend color match exactly.
5. Test the dashboard on both desktop and mobile.

## Font

The dashboard uses Mofugu Sans from:

`assets/fonts/Mofugu-Regular.woff2`

Keep the filename and path unchanged unless the `@font-face` URL in `index.html` is updated as well.

## Calendar privacy

- Do not make private team calendars publicly accessible.
- Share calendars only with authorized Madman Workspace users or the appropriate Google Group.
- Use **See only free/busy** when event details are unnecessary.
- Use **See all event details** only for teammates who require that visibility.
- Do not place confidential client information, embargoed announcements, passwords, private meeting links, or personal contact details in broadly visible event titles.
- Authorized viewers should be signed in to their Madman Google Workspace account when opening the dashboard.

## Project structure

- `index.html` — dashboard structure and styling
- `assets/fonts/Mofugu-Regular.woff2` — locally hosted font
- `_config.yml` — retained for GitHub Pages/Jekyll configuration and possible future templating

## Maintenance

Use descriptive commit messages such as:

- `Add PR team calendar member`
- `Update calendar colors and legend`
- `Improve mobile calendar layout`

After every update, verify that the GitHub Pages deployment completes and that the embedded calendars load for an authorized account.
