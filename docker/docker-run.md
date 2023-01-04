### options

- -e
The operator can set any environment variables in their container by using one or more `-e` flags, even overriding default value or already defined by the developer with a Dockerfile `ENV`.
If the operator names an environment variable without specifying a value, then the current value of the named variable is propagated into the container's environment.

- -v
-v, --volume=[host-src:]container-dest[:<options>]: Bind mount a volume.

host-src can use current path of host machine like below.

example:
-v $(pwd):/dir_name

- -w
-w="", --workdir="": Working directory inside the container.

- -it

- --entrypoint
Overwrite the default entrypoint set by the image.
The `ENTRYPOINT` of an image is similar to a `COMMAND` because it specifies what executable to run when the container starts, but it is (purposely) more difficult to override.
