## Pod de Wordpress amb dos contenidors MySQL i servidor web amb Wordpress
### Procediment:
- Crear el directori on posarem els fitxers de Wordpress.
- Editar el fitxer "wordpress-pod.yml" per posar el directori anterior `path: /home/job/Pods/wordpress/html`.
- Podem editar el fitxer "wordpress-configmap.yml" per si volem modificar les dades de la base de dades.
- Executar la comanda de creació del pod.

```bash
$ podman play kube --configmap ./wordpress-configmap.yml ./wordpress-pod.yml
```


