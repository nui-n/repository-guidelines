# Branch

## Quick Legend

<table>
  <thead>
    <tr>
      <th>Branch</th>
      <th>Role</th>
      <th>Description</th>
      <th>Lifespan</th>
      <th>Source</th>
      <th>Merge Target</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>main</code></td>
      <td>Integration</td>
      <td>Central integration branch</td>
      <td>Permanet</td>
      <td>—</td>
      <td><code>stable</code></td>
    </tr>
    <tr>
      <td><code>work/*</code></td>
      <td>Work</td>
      <td>Short-lived work branch for a single task (feature, doc, investigation) — tied to one issue/PR</td>
      <td>Temporary</td>
      <td><code>main</code></td>
      <td><code>main</code></td>
    </tr>
    <tr>
      <td><code>hotfix/*</code></td>
      <td>Hotfix</td>
      <td>Urgent fixes for current release</td>
      <td>Temporary</td>
      <td><code>stable</code></td>
      <td><code>stable</code>, <code>main</code></td>
    </tr>
    <tr>
      <td><code>stable</code></td>
      <td>Stable</td>
      <td>Holds current and past tagged snapshots of releases — canonical stable state for downstream use</td>
      <td>Permanet</td>
      <td><code>main</code></td>
      <td>—</td>
    </tr>
  </tbody>
</table>

## Main Branches

Long-lived foundational branches that always exist in the repository

### `main`

- Branch for integation
- Essentially the collection of commits made in historical `work/*` branches; you can trace nearly all commits by looking here
- Accepts merges from `work/*` and `hotfix/*` only; direct commits that bypass those are not accepted

### `stable`

- Branch for archival storage
- A collection of snapshots indexed by tags; commits (count) = releases (count)
- Accepts merges from `main` and `hotfix/*` only; direct commits and merges from `work/*` are not accepted

## Supporting Branches

Short-lived branches created for work

### `work/*`

- Branches for general work
- Created for general work (features, docs, workflows, etc.); temporary and deleted after merging.
- Commit directly to add changes and merge into `main`

### `hotfix/*`

- Branches for emergency fixes
- Created to address issues discovered after release; temporary and deleted after merging
- Commit directly for fix releases and merge into both `stable` and `main`
