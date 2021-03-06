# LabWise Knowledge Objects
[![GitHub release](https://img.shields.io/github/release/kgrid-objects/labwise.svg)](https://github.com/kgrid-objects/labwise/releases/)


This is a collection of objects that focus on test guidelines as provided by [Chossing Wisely](http://www.choosingwisely.org).


## Status
The current release of LabWise collection of knowledge objects is [![GitHub release](https://img.shields.io/github/release/kgrid-objects/labwise.svg)](https://github.com/kgrid-objects/labwise/releases/)

This release contains 3 KOs, as listed.

1. [ANA sub-serologies Testing](https://library.kgrid.org/#/object/99999%2Ffk4b85k02x%2Fv0.0.2)

1. [Thyroid Testing](https://library.kgrid.org/#/object/99999%2Ffk4g168s5p%2Fv0.0.2)

1. [Thrombophilia Testing](https://library.kgrid.org/#/object/99999%2Ffk4fj2rv22%2Fv0.0.2)

## LabWise KO Description

  Endpoint:       ` /getrecommendation`

  Input Example:
  ```json
  {
    "labtest":"vte",
    "testresult": true
  }
  ```

  Output Example (Only the `result` of the response is shown):
  ```json
  {
    "labtest":"vte",
    "testresult":true,
    "status":"Major transient risk factors are present for the patient",
    "recs":[
      {
        "text":"DO NOT order Thrombophilia Level Test."
      }],
    "source":"American Society of Hematology",
    "link":"http://www.choosingwisely.org/clinician-lists/american-society-hematology-testing-for-thrombophilia-in-adults/"
  }
  ```
