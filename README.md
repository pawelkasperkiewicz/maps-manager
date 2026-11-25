# Maps Manager — website

Website and privacy policy of the Maps Manager Android app, published with GitHub Pages:

- https://pawelkasperkiewicz.github.io/maps-manager/
- https://pawelkasperkiewicz.github.io/maps-manager/privacy/

Contact: beta.developer007@gmail.com

## Paid uploads switch (`config.json`)

The app reads `config.json` (at most once an hour) to know whether uploading maps to the watch is paid:

```json
{ "paidUploadsFrom": null }
```

- `null` — uploading is free for everyone (early access).
- `"2027-03-01"` (midnight UTC) or `"2027-03-01T10:00:00Z"` — from that moment uploading needs the
  yearly subscription, except for everyone who installed the app before that moment (they stay free).
