# php-helm-chart
## How to build
helm package php

helm repo index . --url https://nicolas2lee.github.io/php-helm-chart/
## How to use
    helm repo add nicolas2lee https://nicolas2lee.github.io/php-helm-chart/
    helm repo update 
    helm search repo 
    helm install php-demo nicolas2lee/php
   
   
    
    helm repo index --url "https://nicolas2lee.github.io/helm-charts/" --merge index.yaml ./laravel-nginx 
    
## Helm standard labels
https://helm.sh/docs/chart_best_practices/labels/

common labels:

|Key                         |Description                                                                           |Example           |Generated Value                |Mapping Custom |
|----------------------------|--------------------------------------------------------------------------------------|------------------|-------------------------------|---------------|
|selector labels             |======================================================================================|==================|===============================|===============|
|app.kubernetes.io/name	     |The name of the application	                                                        |laravel nginx     |{{ include "app.name" . }}     |app            |
|app.kubernetes.io/instance  |A unique name identifying the instance of an application                              |php-laravel-nginx |{{ .Release.Name }}            |release        |
|Common labels               |======================================================================================|==================|===============================|===============|
|app.kubernetes.io/version   |The current version of the application (e.g., a semantic version, revision hash, etc.)|0.1               |{{ .Chart.AppVersion | quote }}|version	       |
|app.kubernetes.io/component |The component within the architecture                                                 |back-end          |                               |tier           |
|app.kubernetes.io/part-of   |The name of a higher level application this one is part of                            |demo              |                               |               |
|app.kubernetes.io/managed-by|The tool being used to manage the operation of an application                         |helm              |{{ .Release.Service }}         |heritage       |
code-app
chart {{ .Chart.Name }}-{{ .Chart.Version }}
function

			
			git tag -a v0.1.0 -m "version 0.1.0, simple version without ssl, ingress/egress, hpa, istio"
			
			docker run -d \
              -it \
              --name devtest \
              -v "$(pwd)"/docker/rpm-package:/app \
              centos/httpd-24-centos7
          
yum install http://rpms.remirepo.net/enterprise/remi-release-7.rpm

#yum install yum-utils


yum-config-manager --enable remi-php72
yum update


yum search php72 | more

yum install php72 php72-php-fpm php72-php-gd php72-php-json php72-php-mbstring php72-php-xml php72-php-xmlrpc php72-php-opcache php-cli

yum install --downloadonly --downloaddir=/app php72 php72-php-fpm php72-php-gd php72-php-json php72-php-mbstring php72-php-xml php72-php-xmlrpc php72-php-opcache php-cli


 docker build -t nicolas2lee/php:72 .
 
 
 audit-libs-python
 checkpolicy
 libcgroup
 libselinux-python
 libselinux-utils
 libsemanage-python
 libxslt
 policycoreutils
 policycoreutils-python
 python-IPy
 scl-utils
 setools-libs
 
 
 yum install --downloadonly --downloaddir=/app  audit-libs-python \
                                                checkpolicy \
                                                libcgroup \
                                                libselinux-python \
                                                libselinux-utils \
                                                libsemanage-python \
                                                libxslt \
                                                policycoreutils \
                                                policycoreutils-python \
                                                python-IPy \
                                                scl-utils \
                                                setools-libs
                                                
                                                
 docker cp 1630895c7275:/app /Users/xinrui/tao/apps/github/php-helm-chart/docker
 
 
 
 yum install --downloadonly --downloaddir=/app php70 php70-php-fpm php70-php-gd php70-php-json php70-php-mbstring php70-php-xml php70-php-xmlrpc php70-php-opcache php-cli


Default package:
libselinux
libselinux-python
libselinux-utils

yum install --downloadonly --downloaddir=/app  rh-php70 rh-php70-php-fpm


                                                
 docker cp 6a80e7fdcccc:/app /Users/xinrui/tao/apps/github/php-helm-chart/docker/repo/php7
 
 https://download-ib01.fedoraproject.org/pub/epel/7/aarch64/Packages/e/epel-release-7-12.noarch.rpm
 
 
  environment-modules
  libargon2
  scl-utils
  
  policycoreutils-python
  libselinux-utils
  libedit
  libX11
  
  libtcl
  
  yum install --downloadonly --downloaddir=/app php php-cli php-mbstring php-fpm
  