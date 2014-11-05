# cram-docker

Docker image of cram

Homepage: https://bitheap.org/cram/
BitBucket: https://bitbucket.org/brodie/cram/overview

Build:

```
docker build -t zeisss/cram-docker .
```


Usage: 

```
alias cram='docker run -it -v $(pwd):$(pwd) -w $(pwd) zeisss/cram-docker'
cram -h

cat > simple.t <<EOF
Simple commands:

  $ echo foo
  foo
  $ printf 'bar\nbaz\n' | cat
  bar
  baz
EOF

cram simple.t
```
