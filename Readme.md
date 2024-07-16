
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
