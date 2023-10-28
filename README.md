# Postgres + WAL-G

Bare bones container combining default [Postgres](https://www.postgresql.org/) and [WAL-G](https://wal-g.readthedocs.io/).

## Tag

Tag name comes from : \<Postgres image\>_\<WAL-G binary\>.

## Missing a release?

Since this contains a random runnable binary file (WAL-G), I'm a bit hesitant of pulling other branches directly (**AND YOU SHOULD TOO AND IF YOU DON'T TRUST ME, USE THE GUIDE BELOW**)

For private use/paranoia: 
- Fork.
- Add WAL-G binary to files.
- Change build-and-public-images.yml file to suit Your needs (usually change jobs.build.strategy.matrix.include to point to the new tag, binary and Postgres image combination).
- Commit/run Github actions.

If You wish for me to publish Your new release, use Github issue template for new release and I will add the release to build pipeline as soon as I can.
