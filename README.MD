delay - ES Module for Deno, Node and Web
=

Usage
-

```js
import delay from './delay.js';

await delay( 100 );
console.log( 'after 100ms' )
```

delay.frame
-

`delay.frame()` awaits [requestAnimationFrame](https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame)

```js
btn.addEventListener( 'click', async () => {
    // Moves btn diagonally every frame
    for ( let i1 = 0; i1 < 1024; i1++ ) {
        await delay.frame();
        btn.style.left = i1.toString();
        btn.style.top = i1.toString();
    }
});
```

Issues
-
For any bug reports or feature requests please
[post an issue on GitHub][issues-url].

Author
-
[**Vincent**](https://www.vincentvictoria.com/)
<br/>
[![Follow on GitHub][github-follow-img]][github-follow-url]
[![Follow on Twitter][twitter-follow-img]][twitter-follow-url]
<br/>
[![Follow on Stack Exchange][stackexchange-img]][stackoverflow-url]

License
-
MIT License. See [LICENSE.md](LICENSE.md) for details.

[github-url]: https://github.com/vincentvictoria/delay
[readme-url]: https://github.com/vincentvictoria/delay#readme
[issues-url]: https://github.com/vincentvictoria/delay/issues
[license-url]: https://github.com/vincentvictoria/delay/blob/master/LICENSE.md
[actions-url]: https://github.com/vincentvictoria/delay/actions
[actions-img]: https://github.com/vincentvictoria/delay/workflows/ci/badge.svg?branch=master&event=push
[travis-url]: https://travis-ci.org/vincentvictoria/delay
[travis-img]: https://travis-ci.org/vincentvictoria/delay.svg?branch=master
[install-img]: https://nodei.co/npm/ende.png?compact=true
[downloads-img]: https://img.shields.io/npm/dt/ende.svg
[license-img]: https://img.shields.io/npm/l/ende.svg
[github-follow-url]: https://github.com/vincentvictoria
[github-follow-img]: https://img.shields.io/github/followers/vincentvictoria.svg?style=social&logo=github&label=Follow
[twitter-follow-url]: https://twitter.com/intent/follow?screen_name=vincentvictoria
[twitter-follow-img]: https://img.shields.io/twitter/follow/vincentvictoria.svg?style=social&logo=twitter&label=Follow
[stackoverflow-url]: https://stackoverflow.com/users/121240
[stackexchange-url]: https://stackexchange.com/users/41681
[stackexchange-img]: https://stackexchange.com/users/flair/41681.png