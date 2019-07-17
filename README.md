_My Gravatar demo projects are for users to get acquainted with languages and platforms with something more than a "Hello World" example. Versions are available for [Clojure](https://brackendev.github.io/GravatarDemo-Clojure/), [F#](https://brackendev.github.io/GravatarDemo-FSharp/), [Newspeak](https://brackendev.github.io/GravatarDemo-Newspeak/), [Pharo](https://brackendev.github.io/GravatarDemo-Pharo/), and [Squeak](https://brackendev.github.io/GravatarDemo-Squeak/)._

- - -

GravatarDemo-Newspeak
===================
**[Newspeak](http://www.newspeaklanguage.org/) implementation to interact with the [Gravatar API](https://en.gravatar.com/site/implement/).**

* [Newspeak 2018-05-12](http://www.newspeaklanguage.org/) reference platform.

## Installation

1. Install and setup [Newspeak](http://www.newspeaklanguage.org/).
2. Download this project.
3. In the **Newspeak Browser**, select _Repositories_. Add a new repository with the local repository path.
4. Select the repository then select _revert_ in the _Image_ column.
5. After syncing, the Gravatar namespace will be accessible.

## Example Usage

In a Newspeak workspace, evaluate:

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

## Acknowledgements

* The [Automattic](http://www.automattic.com/) team for running and supporting Gravatar's free service.
* [Gilad Bracha](http://www.bracha.org/), [Peter Ahe](https://github.com/peter-ahe-google), [Vassili Bykov](http://blog.3plus4.org/), [Ryan Macnak](https://github.com/rmacnak), Bill Maddox, [Yaron Kashai](https://www.linkedin.com/in/yaronkashai/), the [Ministry of Truth team](https://github.com/orgs/newspeaklanguage/people), and [contributors](https://github.com/newspeaklanguage/newspeak/graphs/contributors) for Newspeak, the new programming language in the tradition of Self and Smalltalk. Newspeak is highly dynamic and reflective - but designed to support modularity and security. It supports both object-oriented and functional programming.
* [Eliot Miranda](http://www.mirandabanda.org/cogblog/microbio/), the [OpenSmalltalk team](https://github.com/orgs/OpenSmalltalk/people), and [contributors](https://github.com/OpenSmalltalk/opensmalltalk-vm/graphs/contributors) for [OpenSmalltalk](https://github.com/OpenSmalltalk/opensmalltalk-vm) ([Cog](http://www.mirandabanda.org/cogblog/about-cog/)), the cross-platform virtual machine for Squeak, Pharo, Cuis, and Newspeak.

## Author

[brackendev](https://www.github.com/brackendev)

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
