# nodejs-project


  866  oc project nexus-
  
  867  oc project nexus
  
  868  oc get is
  
  869  oc whoami --show-console
  
  870  podman images
  
  871  podman tag localhost/nodejs-image default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  872  podman images
  
  873  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  879  podman login https://default-route-openshift-image-registry.apps.ocp4.imss.co.in
  
  880  podman login https://default-route-openshift-image-registry.apps.ocp4.imss.co.in --tls-verify=false
  
  881  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  882  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest --tls-verify=false
  
  883  oc new-app --name nodejs-app --port 8080:8080 default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  884  oc new-app --name nodejs-app --port 8080:8080 --image=default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  885  oc new-app --name nodejs-app --port 8080:8080 --image-stream=default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  886  oc new-app --name nodejs-app --port 8080:8080 --image-stream default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  887  oc new-app --help
  
  888  oc new-app --help | grep image-steram
  
  889  oc new-app --help | grep image
  
  891  oc new-app --name nodejs-app --port 8080:8080 --image-stream default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  892  oc new-app --name nodejs-app --image-stream default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  
  893  oc new-app default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest --name=nodejs-app
  
  894  oc get deployment
  
  895  oc get events
  
  896  ll

  
  897  cat Dockerfile
  
  898  vim Dockerfile
  899  ll
  900  rm -rf nexus-1.0.0.tgz
  901  ll
  902  podman build -t nodejs-image .
  903  podman tag localhost/nodejs-image:lates default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  904  podman tag localhost/nodejs-image:latest default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  905  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest
  906  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest --tls-verify=false
  907  oc get deplo
  908  oc get deploy
  909  oc delete deployment nodejs-app
  910  oc get deploy
  911  oc new-app default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest --name=nodejs-app
  912  oc get deploy
  913  oc delete deployment nodejs-app
  914  oc new-app default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest --name=nodejs-image:latest
  915  oc new-app default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-image:latest --name=nodejs-image
  916  oc get deploy
  917  oc get pods
  918  oc logs nodejs-image-78b76b4966-pbpdf
  919  ls
  920  ll
  921  cat package.json
  922  cat nodejs-service.yaml
  923  rm -rf nodejs-service.yaml
  924  ls
  925  ll
  926  cat nodejs-rc.yaml
  927  ls
  928  ll
  929  rm -rf nodejs-rc.yaml
  930  ll
  931  cat nexus-ca.crt
  932  ll
  933  vi server.js
  934  ll
  935  vi Dockerfile
  936  podman images
  937  podman rmi localhost/nodejs-image
  938  podman rmi localhost/my-app
  939  podman rmi localhost/my_app
  940  ll
  941  cat package.json
  942  cat package-lock.json
  943  cat Dockerfile
  944  vi Dockerfile
  945  podman build -t nodejs-app .
  946  podman tag localhost/nodejs-app:latest default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-app:latest
  947  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-app:latest
  948  podman push default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-app:latest --tls-verify=false
  949  oc get deployment
  950  oc delete deployment nodejs-image
  951  oc get deployment
  952  oc new-app default-route-openshift-image-registry.apps.ocp4.imss.co.in/nexus/nodejs-app:latest --name=nodejs-app
  953  oc get deployment
  954  oc get pod
  955  oc get pods
  956  oc logs nodejs-app-76b69c9544-xrgv9
  957  oc get svc
  958  oc delete svc nodeja-image
  959  oc delete svc nodejs-image
  960  oc get svc
  961  oc get route
  962  oc expose svc nodejs-app
  963  oc get route
  964  ll
  965  cat package.json
  966  npm pack
  967  ll
  968  vi package.json
  969  npm publish my-nodejs-app-1.0.0.tgz
  970  npm adduser
  971  npm set registry http://nexus.apps.ocp4.imss.co.in/repository/npm-hosted/
  972  npm adduser --registry=http://nexus.apps.ocp4.imss.co.in/repository/npm-hosted/
  973  npm publish
  974  ls
  975  ll
  976  cat ~/.npmrc
  977  npm publish
  978  cat /home/core/.npm/_logs/2025-06-18T07_45_42_763Z-debug-0.log
  979  npm publish
  980  npm pack
  981  npm publish
  982  npm pack
  983  npm publish
  984  export NODE_EXTRA_CA_CERTS=./nexus-ca.crt
  985  npm publish
  986  vi package.json
  987  npm publish
  988  rm -f ~/.npmrc
  989  echo -n 'admin:admin' | base64
  990  vi ~/.npmrc
  991  curl -u admin:admin http://nexus.apps.ocp4.imss.co.in/service/rest/v1/status
  992  curl -u admin:your-password http://nexus.apps.ocp4.imss.co.in/service/rest/v1/status
  993  npm publish --registry=http://nexus.apps.ocp4.imss.co.in/repository/npm-hosted/
  994  curl -u admin:admin https://nexus.apps.ocp4.imss.co.in/service/rest/v1/status
  995  curl --cacert ./nexus-ca.crt -u admin:admin https://nexus.apps.ocp4.imss.co.in/service/rest/v1/status
  996  export NODE_EXTRA_CA_CERTS=./nexus-ca.crt
  997  npm publish --registry=https://nexus.apps.ocp4.imss.co.in/repository/npm-hosted/
  998  vi ~/.npmrc
  999  npm publish --registry=https://nexus.apps.ocp4.imss.co.in/repository/npm-hosted/ --tls-verify=false
  
  
  
  ============================================
  oc project -q — Get the current project name.

oc project nexus — Switch to the nexus project.

oc get is — List image streams in the current project.

oc whoami --show-console — Show the OpenShift web console URL.

podman images — List local container images.

podman tag ... — Tag a local image with a new name (usually for pushing to a registry).

podman push ... — Push a tagged image to the specified container registry.

podman login ... — Log in to a container registry.

oc new-app ... — Create a new app (deployment, svc, route) from an image.

oc get deployment — Show all deployments in the current project.

oc get events — Display recent cluster events.

oc get deplo / oc get deploy — Shortcuts to show deployments.

oc delete deployment ... — Delete a specific deployment.

oc get pods / oc get pod — Show all pods in the project.

oc logs <pod> — Show logs for the given pod.

oc get svc — List services.

oc delete svc ... — Delete a specific service.

oc get route — Show OpenShift routes (external URLs).

oc expose svc ... — Create a route from a service.

Node.js/NPM Build & Publish:

ls / ll — List files in the directory.

cat <file> — Display file content.

vim / vi <file> — Open file in the editor.

rm -rf <file> — Delete the specified file.

podman build -t ... — Build a container image from Dockerfile.

npm pack — Create a .tgz tarball package from package.json.

npm publish — Publish the package to the NPM registry.

npm adduser — Authenticate with an NPM registry.

npm set registry ... — Set custom NPM registry URL.

cat ~/.npmrc — View npm config file (credentials, registry).

export NODE_EXTRA_CA_CERTS=... — Add custom CA cert for HTTPS registry.

echo -n 'admin:admin' | base64 — Encode credentials for HTTP auth.

curl -u admin:admin ... — Check Nexus status with API call.
