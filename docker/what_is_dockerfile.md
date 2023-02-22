# Dockerfile
Docker can build images automatically by reading the instructions from a Dockerfile. A Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image.

## Format
Here is the format of the Dockerfile.
```dockerfile
# Comment
INSTRUCTION arguments

# example
FROM golang:1.15.7-alpine
```
