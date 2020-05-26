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