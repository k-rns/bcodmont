# Run templates

### Biology
## Run physiology.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template biology/robot_templates/physiology.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_"  --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/biology/robot_templates/physiology.owl" -o biology/robot_templates/physiology.owl


OLD
```
## Run qualifiers.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template qualifiers/robot_templates/qualifiers.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --prefix "SIO:http://semanticscience.org/resource/SIO_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/qualifiers/robot_templates/qualifiers.owl" -o qualifiers/robot_templates/qualifiers.owl
```

### quantifiers
## Run quantifiers.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template quantifiers/robot_templates/quantifiers.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --prefix "SIO:http://semanticscience.org/resource/SIO_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/quantifiers/robot_templates/quantifiers.owl" -o quantifiers/robot_templates/quantifiers.owl





### Chemistry
## Run element.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template chemistry/robot_templates/element.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/chemistry/robot_templates/element.owl" -o chemistry/robot_templates/element.owl

## Run compound.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template chemistry/robot_templates/compound.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/chemistry/robot_templates/compound.owl" -o chemistry/robot_templates/compound.owl


### Physics
## Run characteristic.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template physics/robot_templates/characteristic.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/physics/robot_templates/characteristic.owl" -o physics/robot_templates/characteristic.owl

## Run phenomenon.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template physics/robot_templates/phenomenon.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --prefix "SIO:http://semanticscience.org/resource/SIO_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/physics/robot_templates/phenomenon.owl" -o physics/robot_templates/phenomenon.owl


### Matrix
## Run material.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template matrix/robot_templates/material.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/robot_templates/material.owl" -o matrix/robot_templates/material.owl

## Run context.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template matrix/robot_templates/context.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/robot_templates/context.owl" -o matrix/robot_templates/context.owl

## Run biome.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template matrix/robot_templates/biome.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/robot_templates/biome.owl" -o matrix/robot_templates/biome.owl

## Run region.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template matrix/robot_templates/region.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/robot_templates/region.owl" -o matrix/robot_templates/region.owl

### Operational
## Run operational.tsv run from bcodmont/src/ontology/BCODMO_SM/
robot template --template operational/robot_templates/operational.tsv -i ../bcodmont-edit.owl --prefix "RO:http://purl.obolibrary.org/obo/RO_" --prefix "BSM:http://purl.obolibrary.org/obo/BSM_" --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/operational/robot_templates/operational.owl" -o operational/robot_templates/operational.owl



# Merge templates

## Merge imports and preliminary robot templates, run from bcodmont/src/ontology/BCODMO_SM/
## for modules other than chemistry (not removing CHEBIs axioms)
robot merge --input ../imports/envo_import.owl --input ../imports/pato_import.owl --input ../imports/uberon_import.owl --input ../imports/go_import.owl --input ../imports/iao_import.owl --input ../imports/obi_import.owl --input ../imports/uo_import.owl --input ../imports/chebi_import.owl --input ../imports/stato_import.owl --input ../imports/ms_import.owl --input biology/robot_templates/physiology.owl --input physics/robot_templates/characteristic.owl --input physics/robot_templates/phenomenon.owl --input quantifiers/robot_templates/quantifiers.owl --input operational/robot_templates/operational.owl annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/merge_products/BCODMO_SM_merged.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/merge_products/BCODMO_SM_merged.owl" --output merge_products/BCODMO_SM_merged.owl

## Make object property free version of CHEBI (could add others here in future) Only run after adding to CHEBI import
robot remove --input ../imports/chebi_import.owl --axioms logical annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/intermediate/chebi_import_axioms_removed.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/intermediate/chebi_import_axioms_removed.owl" --output intermediate/chebi_import_axioms_removed.owl

## Make object property free version of ENVO Only run after adding to ENVO import
robot remove --input ../imports/envo_import.owl --axioms logical annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/intermediate/envo_import_axioms_removed.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/intermediate/envo_import_axioms_removed.owl" --output intermediate/envo_import_axioms_removed.owl


## Merge chemistry and matrix modules with axiom removed CHEBI and ENVO
robot merge --input intermediate/chebi_import_axioms_removed.owl --input intermediate/envo_import_axioms_removed.owl --input chemistry/robot_templates/element.owl --input chemistry/robot_templates/compound.owl --input matrix/robot_templates/material.owl --input matrix/robot_templates/context.owl --input matrix/robot_templates/biome.owl --input matrix/robot_templates/region.owl annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/merge_products/BCODMO_SM_axioms_removed_merged.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/merge_products/BCODMO_SM_axioms_removed_merged.owl" --output merge_products/BCODMO_SM_axioms_removed_merged.owl




# Filter to create export products

### Biology
## Filter physiology from merged ontology
robot filter --input merge_products/BCODMO_SM_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:physiology" --select annotations --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/biology/physiology.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/biology/physiology.owl" --output biology/physiology.owl

OLD
```
### Qualifiers
## Filter qualifiers from merged ontology
robot filter --input merge_products/BCODMO_SM_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:qualifiers" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/qualifiers/qualifiers.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/qualifiers/qualifiers.owl" --output qualifiers/qualifiers.owl
```

### Quantifiers
## Filter quantifiers from merged ontology
robot filter --input merge_products/BCODMO_SM_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:quantifiers" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/quantifiers/quantifiers.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/quantifiers/quantifiers.owl" --output quantifiers/quantifiers.owl




### Chemistry
## Filter element from axiom-free merged ontology
robot filter --input merge_products/BCODMO_SM_axioms_removed_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:element" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/chemistry/element.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/chemistry/element.owl" --output chemistry/element.owl

## Filter compound from axiom-free merged ontology
robot filter --input merge_products/BCODMO_SM_axioms_removed_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:compound" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/chemistry/compound.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/chemistry/compound.owl" --output chemistry/compound.owl


### Physics
## Filter characteristic from merged ontology
robot filter --input merge_products/BCODMO_SM_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:characteristic" --select annotations --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/physics/characteristic.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/physics/characteristic.owl" --output physics/characteristic.owl

## Filter phenomenon from merged ontology
robot filter --input merge_products/BCODMO_SM_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:phenomenon" --select annotations --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/physics/phenomenon.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/physics/phenomenon.owl" --output physics/phenomenon.owl


### Matrix
## Filter material from merged ontology
robot filter --input merge_products/BCODMO_SM_axioms_removed_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:material" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/material.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/material.owl" --output matrix/material.owl

## Filter context from merged ontology
robot filter --input merge_products/BCODMO_SM_axioms_removed_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:context" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/context.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/context.owl" --output matrix/context.owl

## Filter biome from merged ontology
robot filter --input merge_products/BCODMO_SM_axioms_removed_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:biome" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/biome.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/matrix/biome.owl" --output matrix/biome.owl


### Operational
## Filter operational from merged ontology
robot filter --input merge_products/BCODMO_SM_merged.owl --prefix "bsm:http://bcodmo/sm#" --select "oboInOwl:inSubset=bsm:operational" --select annotations  --signature true annotate --ontology-iri "http://purl.obolibrary.org/BCODMO_SM/operational/operational.owl" --version-iri "http://purl.obolibrary.org/BCODMO_SM/operational/operational.owl" --output operational/operational.owl





# Export formats:

## Robot
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.json
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.obo
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.ofn
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.omn
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.owl
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.owx
robot convert --input qualifiers/qualifiers.owl --output exports/qualifiers_robot.ttl

## owl2vowl module to get to json
java -jar exports/util/owl2vowl.jar -file qualifiers/qualifiers.owl && mv qualifiers.json exports/qualifiers_owl2vowl.json
