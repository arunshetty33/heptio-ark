# About Heptio Ark

* Heptio Ark provides customizable degrees of recovery for all Kubernetes objects (Pods, Deployments, Jobs, Custom Resource Definitions, etc.), as well as for persistent volumes. This recovery can be cluster-wide, or fine-tuned according to object type, namespace, or labels.

* Ark is ideal for the disaster recovery use case, as well as for snapshotting your application state, prior to performing system operations on your cluster (e.g. upgrades).

# Heptio-Ark server

* This helm chart installs Heptio-ark version v0.8.1


#To set up Ark on AWS, :

*  Create  S3 bucket,
*  Create an AWS IAM role for Ark,
*  Configure the server,
*  Add kube2iam annotation in deployment
 ```
              annotations:
                      iam.amazonaws.com/role: "{{ template "common.kube2iam-role" . }}"
 ```                     
#More information

* https://heptio.github.io/ark/ provides detailed information about building from source, architecture, extending Ark, and more.



