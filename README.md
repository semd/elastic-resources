# Elastic resources

Technical references and interactive diagrams, published with GitHub Pages.

- [AlertZero worker reference](https://semd.github.io/elastic-resources/alertzero/)

## Files

- `docs/index.html`: resources landing page.
- `docs/alertzero/index.html`: worker reference, table, and behavior notes.
- `docs/alertzero/workers.html`: interactive worker relationships.
- `docs/alertzero/data_flow.html`: interactive data flow and rule feedback.
- `docs/alertzero/*.architecture.json`: editable Archify diagram specifications.

The diagrams are standalone HTML files; readers do not need Archify installed.

## Preview locally

Run `python3 -m http.server 8000 --directory docs` and open
<http://localhost:8000/alertzero/>.

## Update and publish

Edit the reference page directly. For diagram changes, edit the corresponding
JSON specification and regenerate the HTML using the Archify skill. Keep the
source revision and verification date current when rechecking the implementation.

GitHub Pages publishes `docs/` from `main`. Push changes to `main` to update the
site, then check the Pages deployment in the repository's Actions tab.
`docs/.nojekyll` makes this a plain static site.
