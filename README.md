# K&U Campus — privacy policy and terms of service

The public copy of the privacy policy and terms of service for **K&U Campus**,
an app for international students at five Korean universities.

Live at **<https://kandu-teamm.github.io/legal/>**, served by GitHub Pages
from `index.html` on `main`.

## Why this repository exists

Both the App Store and Google Play require a privacy policy at a URL that
opens, and it is a listing field neither of them will let you skip. This repo
is public so that URL works; the app's own source stays private.

The domain is not important to either store — they check that the link opens
and that the text describes this app. Both also allow the URL to be changed
later without submitting a new build, so this can move to `kandu.kr` whenever
the website is ready.

## Do not edit `index.html` by hand

It is generated from the app repository, where the same text is also rendered
on the app's own **Settings → Privacy & Terms** screen. One source, because a
policy that says one thing in the app and another on the web is a problem
nobody notices until a reviewer does.

To change the text, edit `app/lib/features/legal/legal_content.dart` in the
app repository, then:

```bash
cd app
flutter test tool/make_legal_page_test.dart   # writes site/index.html
```

and copy the result here.

## Contact

<TeamMillionM@gmail.com>

K&U Campus is an independent, student-run project. It is not affiliated with,
endorsed by, or operated by any of the universities it covers.
