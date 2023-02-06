# Doitsu
Simple and generic web framework, mostly only routing and templating.

## Requirements

- Make sure PHP is available on your system. We recommend PHP 8 or above.
- Make sure Composer is available on your system.

## How to run

- Clone this repository
- Go to the project directory (usually using `cd` command)
- Run `composer -vvv install` (this command is to install the dependencies, will create `vendor` directory)
- Run `php -S 0.0.0.0:4000 -t public` (this command is to run the built-in PHP web server for development purpose)
- Open the web on your browser at `http://localhost:4000` (until this point it means we already have `/` route that handle the home page)

## Sample output

![My image](https://github.com/radicalcircle/doitsu/blob/main/doitsu.png?raw=true)

## What next?

It depends on your imagination. For example in our use case, we use this framework with Alpine.js to handle the reactivity, add date-fns to manipulate date, add Tailwind CSS for nice styling flow and sometimes add Flowbite to take the component advantage of nice visual UI. The limit is your creativity.

## Quick FAQs

- **Want to add new route such as /about or anything?** Just go to `src/_routes.php` and add there. Observe the current code. After you create new route usually you will create a method on `Application` class (located at `src/Application.php`) to execute some code (a.k.a controller) before you render some visual page (a.k.a view).
- **Can I deploy to shared hosting?** Yes, but you should point the website to the `public` folder, since that folder is the entry point or commonly said as web root directory. There is `index.php` file there and everything starts from that script.
- **Can I deploy using Docker?** Yes, we will give the docker-compose sample later.
- **Why another framework? Is Laravel or Symfony not enough?** Hmmmm, you know my motivation create this framework is just for fun and learn. So nothing can stop me to create something haha.

## License

MIT

Copyright (c) 2023-present, Sony Arianto Kurniawan and contributors
