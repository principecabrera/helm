an add instruction in the README.md for charts installation like this (replace princecharts, principecabrera, and main-py-api):

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add princecharts https://principecabrera.github.io/helm-charts

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
princecharts` to see the charts.

To install the main-py-api chart:

    helm install main-py-api princecharts/main-py-api

To uninstall the chart:

    helm delete main-py-api
