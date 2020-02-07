# Heroku Buildpack for Custom Fonts

Fonts used by [Côté Nature](https://cotenature.com) for printing documents.

__WARNING: DO NOT POINT YOUR BUILDPACK CONFIG TO THIS PROJECT__

This buildpack is very specific to our needs. It can and will change and __YOUR APP WILL BREAK__.
The fonts in `fonts.tar.gz` are *probably not what you want or expect*.

We'd hate to see that happen. But please feel free to fork it or crib ideas to make it your own, though!

## Development

### How to Update Fonts Archive

Move individual TTF files into `fonts_source`

```bash
tar -czvf fonts.tar.gz -C fonts_source .
```

### Original Inspiration

* https://github.com/debitoor/heroku-buildpack-converter-fonts
