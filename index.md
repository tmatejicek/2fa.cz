---
layout: default
services: [
    {
        "name":"Apple ID",
        "title":"Dvoufaktorové ověřování Apple ID",
        "href":"https://support.apple.com/cs-cz/HT204915"
    },
    {
        "name":"Centrum Mail",
        "title":"Dvoufaktorové ověřování",
        "href":"https://freemail.help.economia.cz/articles/95769-prvotni-nastaveni-2fa",
    },
    {
        "name":"Facebook",
        "title":"Jak zapnout nebo nastavovat dvoufázové ověření",
        "href":"https://www.facebook.com/help/148233965247823",
    },
    {
        "name":"Google",
        "title":"Zapnutí dvoufázového ověření",
        "href":"https://support.google.com/accounts/answer/185839?hl=cs&co=GENIE.Platform%3DAndroid",
    },
    {
        "name":"Instagram",
        "title":"Zabezpečení instagramového účtu dvoufázovým ověřením",
        "href":"https://help.instagram.com/566810106808145",
    },
    {
        "name":"Microsoft (osobní)",
        "title":"Jak používat dvoustupňové ověřování s účtem Microsoft",
        "href":"https://support.microsoft.com/cs-cz/account-billing/jak-pou%C5%BE%C3%ADvat-dvoustup%C5%88ov%C3%A9-ov%C4%9B%C5%99ov%C3%A1n%C3%AD-s-%C3%BA%C4%8Dtem-microsoft-c7910146-672f-01e9-50a0-93b4585e7eb4",
    },
    {
        "name":"Seznam",
        "title":"Zapnutí dvoufázového ověření",
        "href":"https://napoveda.seznam.cz/cz/login/zapnuti-dvoufazoveho-overeni/",
        "note":"Pro zapnutí dvoufázového ověření je zapotřebí mít nainstalovaný Seznam.cz prohlížeč",
    },
    {
        "name":"X (Twitter)",
        "title":"How to use two-factor authentication",
        "href":"https://help.twitter.com/en/managing-your-account/two-factor-authentication",
    },
]
---

<table>
  <thead>
    <tr>
      <th style="text-align: left">Web/Služba</th>
      <th style="text-align: left">Odkaz na postup zapnutí dvoufaktorového ověřování</th>
    </tr>
  </thead>
  <tbody>
  {% for row in page.services %}
    <tr>
      <td style="text-align: left">
        {{ row.name }}
      </td>
      <td style="text-align: left">
        <a href="{{ row.href }}" target="_blank">{{ row.title }}</a>
        {% if row.note %}
        <br/><small>({{ row.note }})</small>
        {% endif %}
      </td>
    </tr>
  {% endfor %}
  </tbody>
</table>