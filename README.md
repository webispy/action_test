# GitHub Actions

* GitHub Actions product - https://github.com/features/actions
* Marketplace - https://github.com/marketplace?type=actions

## Basic syntax

* [YAML basic syntax](https://en.wikipedia.org/wiki/YAML#Basic_components)
* [Workflow syntax](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions)

## Reference

* [Events that trigger workflows](https://docs.github.com/en/actions/reference/events-that-trigger-workflows)
* [Environment variables](https://docs.github.com/en/actions/reference/environment-variables)

## Examples

* [Hello world](https://github.com/webispy/action_test/tree/step0)
* [Multiple jobs](https://github.com/webispy/action_test/tree/step1)
  * Step들 간에 값 공유 ([`steps` context](https://docs.github.com/en/actions/reference/context-and-expression-syntax-for-github-actions#steps-context))
  * Job들 간에 값 공유 ([`needs` context](https://docs.github.com/en/actions/reference/context-and-expression-syntax-for-github-actions#needs-context))
* [Annotation](https://github.com/webispy/action_test/tree/step2)
  * 코드의 특정 라인에 코멘트 남기기
  * [error message](https://docs.github.com/en/actions/reference/workflow-commands-for-github-actions#setting-an-error-message)

## Events

|Event|설명|
|---|---|
|[pull_request](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#pull_request)|PR이 생성되었을 때|
|[push](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#push)|커밋이 push되었을 때(PR이 머지 되었을 때)|
|[schedule](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#schedule)|특정 시간마다 action을 수행하고 싶을 경우(cron)|
|[release](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#release)|Release가 생성되었을 때|
|[workflow_dispatch](https://docs.github.com/en/actions/reference/events-that-trigger-workflows#workflow_dispatch)|수동으로 GUI를 통해 Action 수행|
