
<h1>
  Kpush / ktag 
</h1>
<p>
    multi tag and push images for a registry
    <br/>
</p>

## Installation 


```shell
git clone https://github.com/DCx14/kpush-ktag.git
cd kpush-ktag
chmod a+x ktag && chmod a+x kpush
cp ktag /usr/local/bin && cp kpush /usr/local/bin
```


## Utilisation

### ktag

```shell
 ktag  frankenphp registry.private.fr/private-image/image-franken:v1.0:latest
```

Output :

```shell
root@H0st42:/# ktag  frankenphp  registry.private.fr/private-image/image-franken:v1.0:latest
 ---------------------------------------------------------------------------
+ | Image: frankenphp
  | | Repository: registry.private.fr/private-image/image-franken
    | |-- v1.0
    | |-- latest
 ---------------------------------------------------------------------------
```

### Kpush

```shell
 kpush registry.private.fr/private-image/image-franken:v1.0:latest:stable
```

Output :

```shell
root@H0st42:/# kpush  registry.private.fr/private-image/image-franken:v1.0:latest:stable
Pushing registry.private.fr/private-image/image-franken:v1.0...
The push refers to repository [registry.private.fr/private-image/image-franken]
4f60957ad86f: Layer already exists 
...
32148f9f6c5a: Layer already exists 
v1.0: digest: sha256:72e04041b2864ee3458bdd722b92759551a8847bcbdf622d83ee5c1823088afbcc size: 3870
Successfully pushed registry.private.fr/private-image/image-franken:v1.0
Pushing registry.private.fr/private-image/image-franken:latest...
The push refers to repository [registry.private.fr/private-image/image-franken]
4f60957ad86f: Layer already exists 
...
32148f9f6c5a: Layer already exists 
latest: digest: sha256:72e04041b2864ee3458bdd722b92759551a8847bcbdf622d83ee5c1823088afbcc size: 3870
Successfully pushed registry.private.fr/private-image/image-franken:latest
Pushing registry.private.fr/private-image/image-franken:stable...
The push refers to repository [registry.private.fr/private-image/image-franken]
4f60957ad86f: Layer already exists 
...
32148f9f6c5a: Layer already exists 
stable: digest: sha256:72e04041b2864ee3458bdd722b92759551a8847bcbdf622d83ee5c1823088afbcc size: 3870
Successfully pushed registry.private.fr/private-image/image-franken:stable
---------------------------------------------------------------------------
All images pushed:
  | Image: registry.private.fr/private-image/image-franken
  | | Repository: registry.private.fr
    | |-- v1.0
    | |-- latest
    | |-- stable
  | -- 
---------------------------------------------------------------------------
All images pushed successfully.

```
