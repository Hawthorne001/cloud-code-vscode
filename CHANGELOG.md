# Release Notes

This page documents production updates to Cloud Code for Visual Studio Code. You can check this page for announcements about new or updated features, bug fixes, known issues, and deprecated functionality.

## Version 1.0.0

We are pleased to announce that Cloud Code is now GA!

### New Features

* **Cloud Shell Integration** Use the ‘Open with Cloud Code’ feature to quickly get started using Google Cloud Platform. It uses a remote development environment in [Cloud Shell](https://cloud.google.com/shell/docs) which means you’ll get to skip setup and start developing with Cloud Code with the click of a button. 

    With ‘Open with Cloud Code’, you can edit, run, and debug code; as well as utilize all of Cloud Code's features directly from inside Cloud Shell. Visual Studio Code's integrated terminal allows direct interaction with command line utilities running in Cloud Shell, such as the gcloud command-line tool, skaffold, and kubectl.

    ![alt_text](images/cloudshell_1_0_0.gif "image_tooltip")

* **YAML editing** Get started with Cloud Build with Cloud Code’s built-in snippets for Cloud Build and Cloud Build trigger YAML files.

    ![alt_text](images/cloudbuild-yaml_1_0_0.gif "image_tooltip")

### Notable Fixes

* Added ability to view and edit yaml of Ingress resource (#158)

## Version 0.0.13

### New Features

* **Logs Viewer**  Browse through and filter Kubernetes cluster logs easily using the new Logs Viewer. For clusters that do not support Stackdriver logging cluster logs will now be colorized.

    ![alt_text](images/logs_viewer_0_0_13.gif "image_tooltip")

* **Dependency Installer** Cloud Code will manage kubectl and Skaffold CLI dependencies automatically.  This can be controlled using the `cloudcode.auto-install` setting.

    ![alt_text](images/dependency_installer_0_0_13.png "image_tooltip")

* **YAML Editing **Create and modify YAML with Cloud Code’s richer YAML editing experience for these configuration types:
  * Anthos Config Management ([link](https://cloud.google.com/anthos-config-management/docs/how-to/configs))
  * Config Connector ([link](https://cloud.google.com/config-connector/docs/overview))
  * Migrate for Anthos ([link](https://cloud.google.com/migrate/anthos/docs/yaml-reference))

    ![alt_text](images/migrate_for_anthos_0_0_13.gif "image_tooltip")

* **Colorized Streams **Deployment and Continuous Deployment output streams will be colorized to highlight key events.

    ![alt_text](images/colorized_streams_0_0_13.gif "image_tooltip")

### Notable Fixes

* Improved extension activation time by removing dependency on language server activation. ([#140](https://github.com/GoogleCloudPlatform/cloud-code-vscode/issues/140))
* Reduced the memory footprint of Kubernetes Cluster Explorer to allow handling large clusters.
* Included various stability fixes. ([#147](https://github.com/GoogleCloudPlatform/cloud-code-vscode/issues/147)) ([#101](https://github.com/GoogleCloudPlatform/cloud-code-vscode/issues/101))