

|:----------------------------------------|:------------------------------------------------:|
| Fitness is Subjective                   |                                                  |
|                                         | <strong class="new-price">Be Better than you were the day before </strong>|
| Fitness is more than a gym and weights  |                                                  |
|                                         | <strong class="new-price">Its a state of mind and making constant decision </strong>|
| Fitness can be anywhere                 |                                                  |
|                                         | <strong class="new-price">As long and you're motivated and put in the work </strong> |
| __Price__                     | __Free__            | <span class="price"><del>$99</del> <strong class="new-price">$69</strong> <small>One-Time Payment</small></span> [^22] |
|===============================+=====================+=====================|
data-gumroad-single-product="true"} |
{:.stretch-table.dl-table}

<script type="module">
  document.querySelectorAll('a[href="#_search-input"]').forEach(el => {
    if (!el.dataset.done) {
      el.addEventListener('click', () => document.getElementById('_search-input').focus());
      el.dataset.done = '';
    }
  });

  document.querySelectorAll('.ppi').forEach(async el => {
    if (!el.dataset.done) {
      const { name, emoji, code, discount } = await window._ppiData;
      if (!code) return;
      el.querySelectorAll('.name').forEach(el => { el.innerText = name });
      el.querySelectorAll('.emoji').forEach(el => { el.innerText = emoji; el.title = name });
      el.querySelectorAll('.code').forEach(el => { el.innerText = code.toUpperCase() });
      el.querySelectorAll('.discount').forEach(el => { el.innerText = `${discount * 100}%` });
      el.dataset.done = '';
    }
  });

  document.querySelectorAll('.price').forEach(async el => {
    if (!el.dataset.done) {
      const { name, emoji, code, discount } = await window._ppiData;
      if (!code) return;
      el.querySelectorAll('.name').forEach(el => { el.innerText = name });
      el.querySelectorAll('.emoji').forEach(el => { el.innerText = emoji; el.title = name });
      el.querySelectorAll('.code').forEach(el => { el.innerText = code.toUpperCase() });
      el.querySelectorAll('.new-price').forEach(el => { el.innerText = `$${99 - discount * 100}` });
      el.dataset.done = '';
    }
  });
</script>
