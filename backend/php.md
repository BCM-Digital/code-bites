# PHP challenge
Your objective is to create a publicly accessible guestbook that anyone can sign.

## Framework requirements
- [Laravel 5.4](https://laravel.com/docs/5.4)
 - You may use any dependencies that are available via Composer ([packagist](https://packagist.org/)).

## App requirements
- The home page `/` should only have a form with two fields (`message` and `name`) and a submit button.
- A user should not be able to submit a new entry without filling in both the `name` and `message` fields.
  - The minimum character count for both fields is **2** characters.
  - The maximum character count for `name` is **50** characters.
  - The maximum character count for `message` is **140** characters.
- All guestbook entries should be viewable at `/entries` and paginated (10 per page).
- Individual entries should be viewable at `/entries/{entries}` where `{entries}` is the entry record's ID.
- The application doesn't require any front-end styling.

## Bonus points
- An api endpoint `/api/entries` that returns a list of all entries in JSON format.
- An api endpoint `/api/entries/special` that returns a list of all entries in JSON format with the following modifications:
  - Each message should be reversed, e.g. "What a cool app!" becomes "!ppa looc a tahW"
  - Each name should be capitalized, e.g. "John" becomes "JOHN".
