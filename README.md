# Getting Started

Clone this project

```bash
$ git clone https://github.com/benoitduval/zend_expressive.git
```

Run composer install

```bash
$ composer install
```

Create symlink between vendor and public files

```bash
$ cd public
$ ln -s ../vendor/components/font-awesome .
$ ln -s ../vendor/components/jquery .
$ ln -s ../vendor/twbs/bootstrap .
```

Test your instance

```bash
$ cd ..
$ composer serve
```

You can then browse to http://localhost:8080.

> ### Setting a timeout
>
> Composer commands time out after 300 seconds (5 minutes). On Linux-based
> systems, the `php -S` command that `composer server` spawns continues running
> as a background process, but on other systems halts when the timeout occurs.
>
> If you want the server to live longer, you can use the
> `COMPOSER_PROCESS_TIMEOUT` environment variable when executing `composer
> serve` to extend the timeout. As an example, the following will extend it
> to a full day:
>
> ```bash
> $ COMPOSER_PROCESS_TIMEOUT=86400 composer serve
> ```
