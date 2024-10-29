## OpenLineage Provider 1.12.2 for Airflow 2.7

This repository contains the wheels for the OpenLineage Provider 1.12.2 and Common Compat Provider 1.2.1 for Airflow 2.7.

## How to use

Add the provider wheel to your Airflow Dockerfile:

```bash
RUN pip install https://github.com/astronomer/custom-ol-provider-for-2.7/raw/refs/heads/main/apache_airflow_providers_openlineage-1.12.2-py3-none-any.whl https://github.com/astronomer/custom-ol-provider-for-2.7/raw/refs/heads/main/apache_airflow_providers_common_compat-1.2.1-py3-none-any.whl
```

Full example of Dockerfile for Astro Runtime 9.19.4:

```dockerfile
FROM quay.io/astronomer/astro-runtime:9.19.4

USER root
RUN pip install https://github.com/astronomer/custom-ol-provider-for-2.7/raw/refs/heads/main/apache_airflow_providers_openlineage-1.12.2-py3-none-any.whl https://github.com/astronomer/custom-ol-provider-for-2.7/raw/refs/heads/main/apache_airflow_providers_common_compat-1.2.1-py3-none-any.whl
USER astro```
