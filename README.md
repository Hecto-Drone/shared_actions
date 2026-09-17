<h1>Shared Actions Repository - README</h1>
<b>NB This is a public repository, so avoid putting sensitive logic or information in composite actions here. The repo is public to allow easy access for other repos. </b>

This repository holds composite actions intended to be used together with reusable workflow or directly in application repositories. Composite action are intented to simplify logic of the workflows and to enable the same actions/logic to be reused over different workflows. 

When setting up a new composite action please use the following naming and folder structure. The action name (ex.: your-composite-action-name) must be a subfolder in the .github folder, and in that folder the .yaml file is placed and named action.yaml 
```
.github
└───your-composite-action-name
    └───action.yaml
```

Using an action requires the reference to a tag on the action. To bring the tag of the must recent commit up-to-date run
```
git tag -f v1 <new-commit-sha>
git push origin v1 --force
```