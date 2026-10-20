# nurwork-sharh

Data for NURWORK (nurwork.one): the classical commentaries (shurūḥ) on the ḥadīth collections, in
their Arabic, cut at each ḥadīth's number so the app can show a commentator's words under any ḥadīth.

- `<work>/<n div 100>.json`: `{"<n>": {"b": chapter, "on": [first, last], "p": [paragraphs], "pg": page} | {"see": "<n>", "on": [...]}}`.
  A chapter explained once for several aḥādīth is kept on the first and pointed to from the rest.
  A last paragraph of "…" means it was cut short (the rest is at al-Shāmila, page `pg`).
- `index.json`: the numbers each work speaks on.

Works: Fatḥ al-Bārī (Ibn Ḥajar), Sharḥ Ibn Baṭṭāl, Irshād al-Sārī (al-Qasṭallānī) on al-Bukhārī;
al-Minhāj (al-Nawawī) on Muslim; Tuḥfat al-Aḥwadhī on al-Tirmidhī; ʿAwn al-Maʿbūd on Abū Dāwūd;
al-Sindī's notes on al-Nasāʾī and Ibn Mājah; Ibn Daqīq al-ʿĪd on al-Nawawī's Forty.

Source: al-Maktaba al-Shāmila (shamela.ws), as turath.io serves it; the printed editions'
footnotes are left out. Built by `scripts/build-sharh.py` in the NURWORK app.
