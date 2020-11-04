### YNAB API
[YNAB API](https://api.youneedabudget.com/)
### Live Demo
[live demo](https://ynab.github.io/ynab-api-starter-kit/)
### Local Usage
* Install [Node.js](https://nodejs.org/).
* In your terminal, run `npx ynab-api-starter-kit my-ynab-app`

This will:
* Create a copy of this project on your computer.
* Install all the dependencies.
* Start up the server ready for development.

### Alternatively

If you're looking for a little less magic:

* Use git to clone it: `git clone https://github.com/ynab/ynab-api-starter-kit`
* From within the folder, run `npm install`
* Then run `npm start`

## Create An OAuth Application

Go to the [YNAB Developer Settings](https://app.youneedabudget.com/settings/developer)
and create a new application.

You'll see your client id, client secret and redirect URI(s).

Copy and paste your client id and redirect URI into the `src/config.json` file.

### `npm start`
Runs the development server (defaults to `localhost:8080`) and watches for changes.

### `npm run build`
Builds the production assets for deployment. This will build to `dist/build.js`
which the `index.html` will load.

### [`src/App.vue`](https://github.com/ajmarroquin/ynab-api-starter-kit/blob/gh-pages/src/App.vue)

In the script portion of this page, you can see how to build an OAuth URI to
obtain an access token for the API.

It also has some examples on retrieving budgets and transactions.

### [`src/Transactions.vue`](https://github.com/ajmarroquin/ynab-api-starter-kit/blob/gh-pages/src/components/Transactions.vue)

This displays all the transactions when you've got them. It also has an example
of using `utils.convertMilliUnitsToCurrencyAmount` to convert the milliunits that
YNAB uses into the currency format of the budget.

### GitHub Pages
If you have a GitHub account, fork this repo. You can now modify your fork, run
`npm run build`, commit and push the code. Your app will be live on `https://[yourgithubacccount].github.io/ynab-api-starter-kit/`.
