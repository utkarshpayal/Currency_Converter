# Currency Converter

A simple browser-based currency converter. Enter an amount, choose a base currency (Indian Rupee, US Dollar or Euro), and the page shows a table of the converted value in every currency returned by the [currencyapi.com](https://currencyapi.com/) `v3/latest` endpoint (currency name, code and rounded converted value).

## Technology used:
- Html
- CSS
- JavaScript

## How it works

- `index.html` – form with an amount input (1–10) and a base-currency dropdown (`INR`, `USD`, `EUR`), plus a results table.
- `main.js` – on submit, fetches `https://api.currencyapi.com/v3/latest?apikey=...&base_currency=<currency>` and fills the table with `rate × amount` (rounded to a whole number).
- `style.css` – styles.

## Running locally

No build step or dependencies are needed.

```sh
git clone https://github.com/utkarshpayal/Currency_Converter.git
cd Currency_Converter
# open index.html in your browser
```

## Configuration

The app needs a currencyapi.com API key. There are no environment variables; the key is part of the request URL in `main.js` (the `apikey` query parameter). To use your own key, create one at currencyapi.com and replace the value in that URL.

## License

MIT – see [LICENSE](LICENSE).

## By CodeWithHarry
