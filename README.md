Just a test repo for hosting helm charts.

All is needed is the following:
- workflows in .github/workflows
- gh-pages branch must exist
- The permissions under Settings/Actions/General/Workflow permissions needs "Read and write permissions"

After that a Job will be triggered at every push to main and it will create the right links in the index.yaml under gh-pages branch

```sh
$ helm repo add vp-test https://mbaldessari.github.io/vp-helm-charts/
$ helm search repo vp-hello
NAME            	CHART VERSION	APP VERSION	DESCRIPTION
vp-test/vp-hello	0.1.0        	1.16.0     	A Helm chart for Kubernetes for Validated Patte...
``````
