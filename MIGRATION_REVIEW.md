# Hyde-inspired Jekyll academic migration, draft review branch

Prepared 3 November 2026. **Not approved for production deployment.**

This branch develops a custom dark sidebar on top of an existing Academic Pages Jekyll repository. It replaces sample homepage/CV/publication/teaching/talk material, adds independently maintained publication and talk records, introduces a DevSecLogs project collection, and keeps the public PDF outside Git history.

## Content and architecture
- Research-led home, About, Research, Projects, Publications, Teaching, Talks & News, Service, CV & Contact
- `_data/hybrid_*.yml`: profile, research, navigation, teaching and news content
- `_publications/`: twelve selected papers with metadata
- `_talks/`: five presentations, including three scheduled CASCON 2026 posters
- `_projects/devseclogs.md`: prototype capabilities, limitations and external link
- `_layouts/hybrid*` and `assets/{css,js}/hybrid.*`: independent responsive sidebar

## Build and production gates
1. Build with the repository's supported Ruby, Jekyll and plugin versions. Confirm layout compilation and all routes, including collection permalinks.
2. Inspect the generated output at desktop, tablet and mobile sizes. Check keyboard and screen-reader behaviour.
3. Audit paper metadata, course appointments, the status of the public DevSecLogs prototype and any future conference events.
4. Upload a privacy-reviewed PDF separately to `files/Sabbir_M_Saleh_Public_Academic_CV.pdf`. Do not commit telephone numbers, private addresses or referee contact details.
5. **Do not merge or deploy** until build and review succeed. Keep `sbrmsaleh.com` on its existing cPanel deployment until the new generated output is tested.
6. The historical Academic Pages sample theme and assets remain in the repository for now, but sample publication/talk/teaching/portfolio records have been removed from this branch.

No GitHub Pages or cPanel publishing workflow is enabled by this change. The independent local staging package is available separately in the ChatGPT conversation.
