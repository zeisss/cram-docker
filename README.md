# cram-docker

Docker image of cram

Homepage: https://bitheap.org/cram/
BitBucket: https://bitbucket.org/brodie/cram/overview

Usage: 

```
alias cram='docker run -it -v $(pwd):$(pwd) -w $(pwd) zeisss/cram'
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
