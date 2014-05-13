# RVM box

This box provides the RVM runtime with a couple of Rubies installed.

Currently installed Rubies:

- `ruby-1.9.3-p484`
- `ruby-1.9.3-p545`
- `ruby-2.0.0-p353` (deprecated)
- `ruby-2.0.0-p451`
- `ruby-2.0.0-p481` (default)
- `ruby-2.1.0` (deprecated)
- `ruby-2.1.1`
- `ruby-2.1.2`

At least _three_ patch level versions will be kept of every version. If you want to keep using a old version you can lock the version on a box, but we __strongly__ recommend upgrading to a newer version.

If a Ruby version has "deprecated" next to it, than that version will be removed next time a new Ruby version gets released.

To switch the Ruby version specify a Ruby version accoring to the following [rules](https://rvm.io/workflow/projects):

> Listed in order of precedence:
>
> - `.rvmrc` - shell script allowing full customization of the environment,
> - `.versions.conf` - `key=value` configuration file
> - `.ruby-version` - single line `ruby-version` only
> - `Gemfile` - comment: `#ruby=1.9.3` and directive: `ruby "1.9.3"`

You can also manually change the version by using the `wercker/rvm-use` step.

Every installed Ruby version comes installed with `bundler ~> 1.5.1`.

# What's new

- Add `ruby-2.0.0-p481`
- Add `ruby-2.1.2`
- Remove `ruby-2.0.0-p247`

# License

The MIT License (MIT)

# Changelog

## 2.0.1
 
- use of updated wercker-essentials box (fix for missing phantomjs)

## 2.0.0

- Add `ruby-2.0.0-p481`
- Add `ruby-2.1.2`
- Remove `ruby-2.0.0-p247`

## 1.0.6

- Use wercker-essentials 1.0.2

## 1.0.5

- Add `ruby-1.9.3-p545`
- Add `ruby-2.0.0-p451`
- Add `ruby-2.1.1`

## 1.0.2

- Add `box-detect` and `default-build`

## 1.0.1

- Use bundler version ~> 1.5.1

## 1.0.0

- Initial release
