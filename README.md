# RVM box

This box provides the RVM runtime with a couple of Rubies installed.

Currently installed Rubies:

- `ruby-1.9.3-p484`
- `ruby-2.0.0-p247`
- `ruby-2.0.0-p353`
- `ruby-2.1.0`

At least _three_ patch level versions will be kept of every version. If you want to keep using a old version you can lock the version on a box, but we __strongly__ recommend upgrading to a newer version. 

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

- Add `box-detect` and `default-build`

# License

The MIT License (MIT)

# Changelog

## 1.0.2

- Add `box-detect` and `default-build`

## 1.0.1

- Use bundler version ~> 1.5.1

## 1.0.0

- Initial release
