#
# Copyright 2020 IBM Corporation
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
FROM quay.io/operator-framework/helm-operator:v0.15.1

LABEL org.label-schema.vendor="IBM" \
    org.label-schema.name="ibm-elastic-stack-operator" \
    org.label-schema.description="IBM Elastic Stack Operator" \
    org.label-schema.vcs-ref=$VCS_REF \
    org.label-schema.vcs-url=$VCS_URL \
    org.label-schema.license="Apache License 2.0" \
    org.label-schema.schema-version="1.0" \
    name="ibm-elastic-stack-operator" \
    vendor="IBM" \
    description="Operator that installs and manages Elastic Stack logging service instances" \
    summary="IBM Elastic Stack Operator"

COPY watches.yaml ${HOME}/watches.yaml
COPY helm-charts/ ${HOME}/helm-charts/
COPY LICENSE /licenses/
