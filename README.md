# tf-operator-helm-hook
This repository is introduced, to cater helm chart based installation
requirements for tungsten fabric controller (for Airship based deployments),
leveraging the existing lifecycle management functionality available in tungsten
fabric operator.

Though we recommend induction of operator life-cycle manager into Airship, this
helm-hook is provided as a interim solution for integration of tungsten fabric
with airship and openstack-helm.

## Background
With introduction of operator-sdk, and a shift to support life-cycle management
of various applications using operator lifecycle manager, in a kubernetes native
way. It was identified that operator framework caters to tungsten fabric
lifecycle management requirements more comprehensively by providing a custom
runtime controller.

tf-operator-helm-hook allows unification of dependency management under single
umberalla of tf-operator, but still allows a helm chart based installation when
required.
