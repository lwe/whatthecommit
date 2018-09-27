whatthecommit
=============

An unoffical command client to fetch a random and silly commit message from
[whatthecommit.com][wtc].

> For the sources of [whatthecommit.com][wtc] see
> https://github.com/ngerakines/commitment

FAQ
---

#### Is it useful?

Yeah, sure, I mean it's perfect for those cases where you
haven't committed a change in ages and feel too important to use
`git add -i`, so `git commit -am "$(whatthecommit)"` to the rescue :wink:

#### How do I install it?

To get up and running as fast as possbile run

```bash
# installs to /usr/local/bin/whatthecommit
curl -L https://github.com/lwe/whatthecommit/raw/master/whatthecommit >/usr/local/bin/whatthecommit
chmod 0755 /usr/local/bin/whatthecommit
```

#### Are there any options?

Sure, check `whatthecommit -h` for usage and options.

#### Do I need this? / Alternatives

No, [whatthecommit.com][wtc] provides since some time a
plain text interface at https://whatthecommit.com/index.txt - so a good
alternative would be to create something like:

```bash
# .bashrc / .zshrc or whatever
function whatthecommit() {
  curl --silent --fail https://whatthecommit.com/index.txt
}
```

...or how about a git alias?

```bash
# From https://github.com/ngerakines/commitment/issues/69#issuecomment-91053061
git config --global alias.yolo '!git add -A && git commit -m "$(curl --silent --fail https://whatthecommit.com/index.txt)"'
```

Thanks to [m13253](https://github.com/m13253) for the index.txt trick.

[wtc]: https://whatthecommit.com/
