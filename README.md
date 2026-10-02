# Daisy JSON Mappings for Oopsy

This is a repository of parameter definition files for programming
[Daisy](https://daisy.audio/) Seed boards with [oopsy](https://github.com/daisyaudio/oopsy).

Oopsy is a project by Graham Wakefield that allows you to export patches from
the `gen~` patching environment in Max/MSP to the Daisy, instead of programming
the Daisy in C++.

Check out [oopsy](https://github.com/daisyaudio/oopsy) for a lot more
information about how to program a Daisy in `gen~`.

## What this repository is for

Oopsy already includes configurations for many common Daisy hardware platforms
such as the [Daisy Pod](https://daisy.audio/products/pod) or the [Noise
Engineering Versio](https://noiseengineering.us/products/versio/). However,
Daisy's popularity has meant that there are now more hardware devices that work
with the daisy, including [Cleveland Music Co
Hothouse](https://clevelandmusicco.com/products/hothouse-digital-signal-processing-platform-kit)
that are not included in oopsy. This repository provides configuration files
for some of these other platforms.

## Getting started

1. Go to [oopsy](https://github.com/daisyaudio/oopsy) and follow its
   instructions to install the Max package and oopsy toolchain.
2. Clone this repository or download its contents. Save it to some place in
   your Max search path. (e.g. `~/Documents/Max 9/Library`)
3. Create a max patch that includes an `oopsy.maxpat` `bpatcher`, as shown in
   the oopsy examples.
4. Instead of using the small dropdown menu inside the `bpatcher` to select
   your target (e.g. `field`), send a `target` message to the `bpatcher` with
   the name of the mapping file you want to use (e.g. `target seed.hothouse.json`)

## Feedback and configurations

If you think something is broken, please file an issue.

If you would like to contribute a new mapping or modify an existing one, please
make a pull request.

## Resources

When building your own JSON mappings, I recommend these reference materials:

- The README from the [Daisy json2daisy repository](https://github.com/daisyaudio/json2daisy/blob/main/src/json2daisy/resources/component_defs.json)
- Component definitions from [json2daisy](https://github.com/daisyaudio/json2daisy/blob/main/src/json2daisy/resources/component_defs.json)
- Existing mappings from oopsy: <https://github.com/daisyaudio/oopsy/tree/main/source>
- Blog and forum posts from Daisy, including:
  - <https://daisy.audio/blogs/seeds-n-circuits/what-the-mux-a-guided-tutorial-for-using-multiplexers-with-daisy>
  - <https://community.daisy.audio/t/quick-guide-on-setting-up-a-custom-json-file-for-pd2dsy-oopsy/4021>
