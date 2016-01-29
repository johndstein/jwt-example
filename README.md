# JWT Examples

```
./build.sh
npm test
```

So to use public private key you generate a keypair as normal.

```
$ ssh-keygen -t rsa -b 4096 -C "junk@id.rsa"
```

This second bit is the KEY!!! You MUST turn your .pub file into a .pem
or jsonwebtoken no like it! You will get nasty errors like:
JsonWebTokenError: invalid algorithm

```
$ ssh-keygen -f junk_id_rsa.pub -e -m pem > junk_id_rsa.pem
```


