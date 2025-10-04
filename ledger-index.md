# Ledger Index (Human View)

This page lists entries from the machine-readable [`ledger-index.json`](ledger-index.json).

<div id="ledger-list">Loading ledger entries…</div>

<script>
(function () {
  const target = document.getElementById('ledger-list');
  function link(href, text) { const a = document.createElement('a'); a.href = href; a.textContent = text; return a; }
  function li(child) { const el = document.createElement('li'); el.appendChild(child); return el; }

  fetch('ledger-index.json')
    .then(r => r.json())
    .then(data => {
      const ul = document.createElement('ul');
      (data.entries || []).forEach(e => {
        const fileHref = e.file || '';
        const title = e.title || e.id || fileHref;
        const date = e.date ? ` — ${e.date}` : '';
        const item = document.createElement('span');
        item.appendChild(link(fileHref, title));
        item.appendChild(document.createTextNode(date));
        ul.appendChild(li(item));
      });
      target.innerHTML = '';
      target.appendChild(ul);
    })
    .catch(err => {
      target.textContent = 'Could not load ledger-index.json';
      console.error(err);
    });
})();
</script>
