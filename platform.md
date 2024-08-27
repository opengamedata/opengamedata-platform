# OpenGameData Software Reference Platform

Below is a list of standard software libraries that make up the **OpenGameData Reference Platform**. This **reference platform** is meant as a *convention* for keeping new development coordinated with respect to the development and deployment environments.

## Justification

The bar for updating a package is relatively low, we only require some simple justification,
e.g. "we need a feature from a newer version to make X better,"
or "the current version is old and nobody uses it anymore,"
or "another library needs a newer version."

In general, we avoid allowing projects to become so oddly-specific as to be tied to a specific package/version. The onus is on us to keep OGD projects running on relatively recent library versions, to keep a low barrier for entry to new collaborators who want to start fresh.

However, any OpenGameData project should avoid using a different version of any of these libraries than what is listed. Instead, ask for a version bump and wait for an update to the platform, so we don’t have incompatibilities pop up at random.

We use this list for GitHub Actions, requirements.txt, and .devcontainer files.
Note: for some libraries, we use .* to indicate any patch version may be used (we only specify patch version for mission-critical dependencies, such as database libraries).

## Latest Platform

- Python: 3.12
  - build 1.2.*
  - gitdb 4.0.*
  - GitPython 3.1.*
  - google-cloud-bigquery 3.19.0
  - ipywidgets 8.0.*
  - matplotlib 3.9.*
  - mysql-connector-python 8.0.25
  - numpy 2.1.*
  - flask 2.3.3
  - flask-cors 4.0.1
  - flask-restful 0.3.10
  - pandas 2.2.*
  - scikit-learn 1.5.*
  - seaborn 0.13.*
  - sshtunnel 0.4.0
  - statsmodels 0.13.*
  - tensorflow 2.17.*
  - twine 4.0.*
- PHP v.8.1.17
- MariaDB 10.5.18 (compatible with MySQL 15.1)

Last updated August 2024.