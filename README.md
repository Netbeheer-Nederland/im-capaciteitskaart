# im-capaciteitskaart

Informatiemodel voor de NBNL-capaciteitskaart.

## Website

[https://Netbeheer-Nederland.github.io/im-capaciteitskaart](https://Netbeheer-Nederland.github.io/im-capaciteitskaart)

## Repository Structure

* [examples/](examples/) - example data
* [project/](project/) - project files (do not edit these)
* [src/](src/) - source files (edit these)
  * [im_capaciteitskaart](src/im_capaciteitskaart)
    * [schema](src/im_capaciteitskaart/schema) -- LinkML schema
      (edit this)

## Schema Generation

Run the following commands before committing new versions:

```
$ make site
$ gen-linkml-profile pydantic src/im_capaciteitskaart/schema/im_capaciteitskaart-full.yaml --out src/im_capaciteitskaart/schema/im_capaciteitskaart.yaml -a demand99Percentile demand_99_percentile -a demand75Percentile demand_75_percentile -a demand50Percentile demand_50_percentile -a demand25Percentile demand_25_percentile
```

## Developer Documentation

<details>
Use the `make` command to generate project artefacts:

* `make all`: make everything
* `make deploy`: deploys site
</details>

## Credits

This project was made with
[linkml-project-cookiecutter](https://github.com/linkml/linkml-project-cookiecutter).
