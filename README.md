# plushu-buildstep-buildpacks

Installs the default set of buildpacks used by Buildstep.

## Usage

```bash
# if you haven't already installed the buildpacks plugin
plushu install buildpacks

plushu install buildstep-buildpacks
```

## How is this different from plushu-heroku-buildpacks?

This installs a very similar set of buildpacks to the Heroku buildpack plugin.
There are two significant differences:

- This reads the configuration defined for buildstep, which is locked to
  specific, vetted versions. The heroku-buildpacks plugin always installs the
  current master. (If this plugin cannot read the current configuration, it
  will fall back to installing the current master revision as well.)
- buildstep includes the [ddollar/heroku-buildpack-multi][] buildpack, which
  is not technically an official Heroku buildpack.

[ddollar/heroku-buildpack-multi]: https://github.com/ddollar/heroku-buildpack-multi

## See also

[plushu/plushu-buildstep-custom-buildpacks][] - adds the custom buildpacks that
used to be included with buildstep.

[plushu/plushu-buildstep-custom-buildpacks]: https://github.com/plushu/plushu-buildstep-custom-buildpacks
