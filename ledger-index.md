# Ledger Index (Human View)

This page lists entries from the machine-readable [`ledger-index.json`](ledger-index.json).
It’s generated at view-time so tools can keep using the JSON, and humans get a friendly table.

<div id="ledger-target">Loading ledger entries…</div>

<script>
(function () {
  const mount = document.getElementById('ledger-target');

  function renderTable(entries) {
    if (!Array.isArray(entries) || entries.length === 0) {
      mount.textContent = 'No entries yet.';
      return;
    }
    const table = document.createElement('table');
    table.style.width = '100%';
    table.style.borderCollapse = 'collapse';
    const thead = document.createElement('thead');
    const headerRow = document.createElement('tr');
    ['Date','Title','File'].forEach(h => {
      const th = document.createElement('th');
      th.textContent = h;
      th.style.textAlign = 'left';
      th.style.padding = '8px 6px';
      th.style.borderBottom = '1px solid #ddd';
      headerRow.appendChild(th);
    });
    thead.appendChild(headerRow);
    table.appendChild(thead);

    const tbody = document.createElement('tbody');
    entries.forEach(e => {
      const tr = document.createElement('tr');

      function td(textOrNode) {
        const td = document.createElement('td');
        td.style.padding = '8px 6px';
        if (typeof textOrNode === 'string') td.textContent = textOrNode;
        else td.appendChild(textOrNode);
        return td;
      }

      const date = e.date || '';
      const title = e.title || e.id || '(untitled)';
      const file = e.file || '';

      const link = document.createElement('a');
      link.href = file;              // keep relative path, works in Pages
      link.textContent = file || '(missing)';

      tr.appendChild(td(date));
      tr.appendChild(td(title));
      tr.appendChild(td(link));
      tbody.appendChild(tr);
    });

    table.appendChild(tbody);
    mount.innerHTML = '';
    mount.appendChild(table);
  }

  fetch('ledger-index.json')
    .then(r => r.json())
    .then(json => renderTable(json.entries || []))
    .catch(err => {
      console.error(err);
      mount.textContent = 'Could not load ledger-index.json';
    });
})();
</script>
