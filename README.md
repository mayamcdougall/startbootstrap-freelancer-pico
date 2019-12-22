# [Start Bootstrap][] - [Freelancer][] - [Pico Version][PicoCMS]

This is a [PicoCMS][] port of for the [Freelancer][] portfolio theme based on [Bootstrap][], created by [Start Bootstrap][].

Live preview of [Freelancer][] available [here][Preview].

## Getting Started

To use this theme:

1. Download the [Latest Release][] on GitHub.
1. Extract `themes/freelancer` to your Pico `themes` folder.
1. Extract `index.md.sample` and `content/feed.md` (optional*) to your `content` folder.
1. Copy or rename `index.md.sample` to `index.md`
1. Copy or reanme `modalitem.md.sample` to `abitraryname.md`
1. Configure your website using the YAML options in `index.md`

\* Provides an RSS feed of your pages at `/feed`

## Contact Form Setup

While out of the scope of this port, in order for the contact form to work, you'll need the php file [`mail/contact_me.php`][MailSupport] from the original HTML version of [Freelancer][].

You'll need to place the `mail` folder in the root of your Pico install.  From there, you'll need to edit `contact_me.php` to specify your email address.  There are additional options you can configure in this file as well.

Support for this feature will ultimately depend on the configuration of your server, but is again, out of scope of this port.

You can easily disable the contact form from within `index.md` if you do not wish to use it.

## No Remote Libraries

If you want to host all libraries locally, you must download the respective libraries and make them available to the theme somehow.
One option is to put the libraries globally into the pico root directory(`<nextcloud_dir>/apps/cms_pico/`). Here you can keep libraries updated for multiple themes relatively easy.

However, if you want to keep libraries available only to a specific theme, you must put such libraries into the theme folder, such as the `includes` directory.
For example, download the the distribution of [Freelancer][]. Copy all subdirectories (`css`, `js`, `mail`, `vendor`, `scss`) into the the `includes` directory.
Then change the files `javascript.twig` and `head.twig` to use the theme's libraries. 
The placeholder `{{ theme_url }}` will return the location in the pico cms.
`javascript.twig` will contain lines such as:
```
  <!-- Custom scripts for this template -->
  <script src="{{ theme_url }}/includes/js/freelancer.js"></script>
```
## Bugs and Issues

Have a bug or an issue with this template? You can open a new [Issue][] here on GitHub.

## Creator

Start Bootstrap was created by and is maintained by **[David Miller][]**, Owner of [Blackrock Digital][].

* https://twitter.com/davidmillerskt
* https://github.com/davidtmiller

Start Bootstrap is based on the [Bootstrap][] framework created by [Mark Otto][] and [Jacob Thorton][].

## Copyright and License

Copyright 2013-2016 Blackrock Digital LLC. Code released under the [MIT][] license.

[Start Bootstrap]: http://startbootstrap.com/
[Freelancer]: http://startbootstrap.com/template-overviews/freelancer/
[Bootstrap]: http://getbootstrap.com/
[PicoCMS]: http://picocms.org
[Latest Release]: https://github.com/smcdougall/startbootstrap-freelancer-pico/releases/
[Preview]: https://blackrockdigital.github.io/startbootstrap-freelancer/
[MailSupport]: https://github.com/BlackrockDigital/startbootstrap-freelancer/blob/master/mail/contact_me.php
[Issue]: https://github.com/smcdougall/startbootstrap-freelancer-pico/issues
[David Miller]: http://davidmiller.io/
[Blackrock Digital]: http://blackrockdigital.io/
[Mark Otto]: https://twitter.com/mdo
[Jacob Thorton]: https://twitter.com/fat
[MIT]: https://github.com/smcdougall/startbootstrap-freelancer-pico/blob/master/LICENSE
