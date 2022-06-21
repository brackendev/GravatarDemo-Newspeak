_My Gravatar demo projects are for developers to get acquainted with languages and platforms with something more than a "Hello World" example. Versions are available for [Clojure](https://github.com/brackendev/GravatarDemo-Clojure), [F#](https://github.com/brackendev/GravatarDemo-FSharp), [Newspeak](https://github.com/brackendev/GravatarDemo-Newspeak), [Pharo](https://github.com/brackendev/GravatarDemo-Pharo), [Racket](https://github.com/brackendev/GravatarDemo-Racket), and [Squeak](https://github.com/brackendev/GravatarDemo-Squeak)._

- - -

GravatarDemo-Newspeak
===================
**[Newspeak](http://www.newspeaklanguage.org/) implementation to interact with the [Gravatar API](https://en.gravatar.com/site/implement/).**

* [Newspeak 2018-05-12](http://www.newspeaklanguage.org/) reference platform.

## TODO

- [ ] Support the latest Newspeak release.

## Installation

1. Download this project.
2. Install and run [Newspeak](http://www.newspeaklanguage.org/).
3. In the **Newspeak Browser**, select _Repositories_. Add a new repository with the local repository path (this project's location).
4. Select the repository then select _revert_ in the _Image_ column.
5. After syncing, the Gravatar namespace will be accessible.

## Example Usage

Evaluate in a Workspace:

```newspeak
(* Retrieve the image for the email address *)
| gravatar |
gravatar:: Gravatar usingPlatform: platform.
gravatar retrieveProfileForEmail: 'email@example.com'.
```

```newspeak
(* Retrieve the image (200 px by 200 px, rated 'G' or 'PG') for the email address *)
| gravatar |
gravatar:: Gravatar usingPlatform: platform.
gravatar retrieveImageForEmail: 'email@example.com' size: 200 rating: 'pg'.
```

```newspeak
(* Retrieve the profile for the email address *)
| gravatar |
gravatar:: Gravatar usingPlatform: platform.
gravatar retrieveImageForEmail: 'email@example.com'.
```

## Author

Bracken Spencer

* [GitHub](https://www.github.com/brackendev)
* [LinkedIn](https://www.linkedin.com/in/brackenspencer/)
* [Twitter](https://twitter.com/brackendev)

## License

GravatarDemo-Newspeak is released under the MIT license. See the LICENSE file for more info.

- - -

## Useful Links

* Gilad Bracha
    * [@Gilad_Bracha](https://twitter.com/Gilad_Bracha) [Twitter]
    * Design of Newspeak Language: [Part 1](https://www.youtube.com/watch?v=UwkROn7OmNQ), [Part 2](https://www.youtube.com/watch?v=FAUUY4VQc8w)
    * [Room 101](https://gbracha.blogspot.com)
    * [bracha.org](http://www.bracha.org/)
* [Newspeak 101: A Guide for the Perplexed](https://medium.com/newspeak-documentation/newspeak-101-1fe7a924d726)
* [Newspeak Google Group](https://groups.google.com/forum/#!forum/newspeaklanguage)
* [newspeaklanguage.org](http://www.newspeaklanguage.org/)
