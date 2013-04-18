whatthecommit
=============

An unoffical command client to fetch a commit message from http://whatthecommit.com/

FAQ
---

**Is it useful?** Yeah, sure, I mean it's perfect for those cases where you haven't committed a
change in ages and feel too important to use `git add -i`, so `git commit -am "$(whatthecommit)"`
to the rescue :wink:

**How do I install it?** To get up and running as fast as possbile run

    curl -L https://raw.github.com/dbldots/whatthecommit/master/whatthecommit > /usr/local/bin/whatthecommit
    chmod 0755 /usr/local/bin/whatthecommit

**Are there any options?** Sure, check `whatthecommit -h` for usage and options.

