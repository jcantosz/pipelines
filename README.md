This repository is an example of how-to on starting with Codefresh pipelines configured with code from this repository.

In the root of this repository is `codefresh-spec.yaml` file which is the pipeline-creator that will create/update the pipelines coded in this repository.

There is an example ci pipeline `common` which is a single pipeline `ci/common/codefresh-spec.yaml` shared by multiple projects defined in the `projects` folder of `ci/common` directory.

If any new projects are added in the projects folder they will reuse the common CI pipeline.

There is also a cd pipelines `argo-sync` which is called upon from `common` when the timing is right to run ArgoCD Sync for a project.

For more in-depth explanation please talk to Solutions Architect or Customer Success teams.