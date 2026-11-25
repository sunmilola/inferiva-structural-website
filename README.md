# INFERIVA customer website

Open `index.html` for the customer homepage or preview the site locally:

```bash
python3 -m http.server 8000
```

The archive includes the generated HTML, all eight original films and their
caption tracks, and the Python generator. Edit page content in `pages.py`
and shared layout in `build.py`, then run `python3 build.py` to regenerate.

The homepage opens with INFERIVA’s platform proposition, followed by a
customer workflow, sector routes and engagement options. Detailed product
pages and the assurance specimen are available from their respective sections.

## Enquiry delivery

The supplied HTML opens a prefilled email draft addressed to
`enquiries@inferivastructural.com`. The visitor reviews and sends it in their
email app.

To enable web submission, rebuild the site with an HTTPS form endpoint that
you control and that accepts multipart POST requests from the deployed origin.
The endpoint should return an HTTP 2xx response only when it has accepted the
enquiry. Set the recipient and spam protection with your form provider.

```bash
INFERIVA_ENQUIRY_ENDPOINT='https://your-configured-endpoint' python3 build.py
```

Deploy the regenerated HTML and media together. Submit a test enquiry from
the deployed site and confirm that it reaches the intended inbox.

## Website photography

The photos illustrate ordinary work and payment settings.

| Asset | Photographer and source |
| --- | --- |
| Homepage | [Edmond Dantès](https://www.pexels.com/photo/people-brainstorming-at-the-office-8550845/) |
| Commercial banking | [Edmond Dantès](https://www.pexels.com/photo/photograph-of-a-group-of-people-talking-4345107/) |
| Payments and mobile money | [Pavel Danilyuk](https://www.pexels.com/photo/a-person-tapping-the-phone-on-a-payment-terminal-6612717/) |
| Microfinance | [Mikhail Nilov](https://www.pexels.com/photo/a-woman-holding-laptop-8872695/) |
| Development finance | [Mikhail Nilov](https://www.pexels.com/photo/woman-working-on-her-laptop-8938355/) |

Source terms are available under the [Pexels License](https://www.pexels.com/license/).
