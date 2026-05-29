# Helmfile template

## Folder structure

- charts/ -> Helm charts
    - upstream/ -> Third-party charts not managed by us
    - example-chart/
        - templates/ -> Custom YAML files
        - Chart.yaml
        - values.yaml -> Default values
- kustomizations/
    - example-kustomization/
        - patches/
        - resources/ -> Custom YAML files
        - upstream/ -> Dependency YAML files from upstream sources
        - kustomization.yaml
- secrets -> Placeholder secrets used when manually deploying (No actual secrets should ever be uploaded to source control)
- values
