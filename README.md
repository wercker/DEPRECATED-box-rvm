# RVM box

This box provides the RVM runtime with a couple of Rubies installed.

Currently installed Rubies:

- `ruby-2.0.0-p645` (deprecated)
- `ruby-2.0.0-p647`
- `ruby-2.0.0-p648`
- `ruby-2.1.6` (deprecated)
- `ruby-2.1.7`
- `ruby-2.1.8`
- `ruby-2.2.2` (deprecated)
- `ruby-2.2.3`
- `ruby-2.2.4` (default)

At least _three_ patch level versions will be kept of every version. If you want
to keep using a old version you can lock the version on a box, but we
__strongly__ recommend upgrading to a newer version.

If a Ruby version has `deprecated` next to it, than that version will be removed
next time a new Ruby version gets released.

To switch the Ruby version specify a Ruby version accoring to the following
[rules](https://rvm.io/workflow/projects):

> Listed in order of precedence:
>
> - `.rvmrc` - shell script allowing full customization of the environment,
> - `.versions.conf` - `key=value` configuration file
> - `.ruby-version` - single line `ruby-version` only
> - `Gemfile` - comment: `#ruby=1.9.3` and directive: `ruby "1.9.3"`

You can also manually change the version by using the `wercker/rvm-use` step.

Every installed Ruby version comes installed with `bundler ~> 1.5.1`.

# License

The MIT License (MIT)

# Changelog

## master

- Added `ruby-2.2.4`
- Added `ruby-2.1.8`
- Added `ruby-2.0.0-p648`

## 4.0.0

- Added `ruby-2.2.3`
- Added `ruby-2.1.7`
- Added `ruby-2.0.0-p647`
- Removed `ruby-2.2.0`
- Removed `ruby-2.1.4`
- Removed `ruby-2.0.0-p598`
- Removed `1.9.3-p551`
- Removed `1.9.3-p550`
- Removed `1.9.3-p547`
- Set `ruby-2.2.3` as default

## 3.0.0

- Added `ruby-2.2.2`
- Added `ruby-2.1.6`
- Added `ruby-2.0.0-p645`
- Removed `ruby-2.1.4`
- Removed `ruby-2.0.0-p594`
- Set `ruby-2.2.2` as default
- Update installed bundler gem to `1.9.0`

## 2.5.0

- Added `ruby-2.2.1`
- Added `ruby-2.0.0-p643`
- Removed `ruby-2.0.0-p576`
- Set `ruby-2.2.1` as default

## 2.4.0

- Added `ruby-2.2-0`
- Set `ruby-2.2.0` as default

## 2.3.0

- Added `ruby-1.9.3-p551`
- Added `ruby-2.0.0-p598`
- Added `ruby-2.1.5`
- Removed `ruby-1.9.3-p545`
- Removed `ruby-2.0.0-p481`
- Removed `ruby-2.1.2`
- Set `ruby-2.1.5` as default

## 2.2.0

- Added `ruby-1.9.3-p550`
- Added `ruby-2.0.0-p594`
- Added `ruby-2.1.4`
- Removed `ruby-1.9.3-p484`
- Removed `ruby-2.0.0-p451`
- Removed `ruby-2.1.1`
- Set `ruby-2.0.0-p594` as default

## 2.1.0

- Add `ruby-1.9.3-p547`
- Add `ruby-2.0.0-p576`
- Remove `ruby-2.0.0-p353`
- Remove `ruby-2.1.0`
- Set `ruby-2.0.0-p576` as default

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
