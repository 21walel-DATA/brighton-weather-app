# Brighton Weather App

A simple weather app built in plain HTML, CSS and JavaScript (no libraries), using the free [Open-Meteo](https://open-meteo.com/) API. No API key is needed.

I built it in five stages as part of week 7 of the TechNative 10-week Software Development Bootcamp. Each stage is its own page, so you can see how the app grew.

| Stage | File | What it adds |
|---|---|---|
| 1 | [brighton-weather.html](brighton-weather.html) | A `CONFIG` object for the town and its location, and a `buildUrl` function that makes the API address. The page shows the town and a link to the address. |
| 2 | [brighton-weather-fetch.html](brighton-weather-fetch.html) | `loadWeather` uses `fetch` with `async`/`await` and shows the raw JSON in a `<pre>` tag. |
| 3 | [brighton-weather-parse.html](brighton-weather-parse.html) | `showWeather` picks out the weather code, temperature and time. `try`/`catch` shows an error message if loading fails. |
| 4 | [brighton-weather-refresh.html](brighton-weather-refresh.html) | A Refresh button. `formatDate` uses `split` to show the date as 28/10/2026 12:45. `describeWeather` turns the weather code into words, and the temperature gets °C. |
| 5 | [brighton-weather-extras.html](brighton-weather-extras.html) | A styled weather card, a big weather emoji, a background colour that matches the weather, and a search box that looks up any town with the Open-Meteo geocoding API. |

## How to run it

Download or clone the repo, then double-click any `.html` file to open it in your browser. It needs an internet connection to fetch the weather.

## What I learned

- Building API URLs from settings
- Using `fetch`, `async` and `await` to get data
- Reading values out of JSON
- Handling errors with `try`/`catch`
- Reusing functions, for example from button clicks with `addEventListener`
- Working with strings using `split`
- Styling a page with CSS: flexbox, rounded corners and shadows

## How it was made

I planned and directed the project stage by stage, following the bootcamp's stage instructions. I used [Claude Code](https://claude.com/claude-code), an AI coding assistant, to write the code from my prompts. I then tested each stage myself and studied how the code works.
