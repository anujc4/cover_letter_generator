# COVER LETTER GENERATOR

Generates a word document from a predefined template and replaces the defined
template variables.

## Prerequisites

Ruby

## Usage

Edit the `varibles.yml` file.

```(yaml)
# OPTIONAL: Name of the person addressing the letter to
# Default: "HR Manager"
JOB_CONTACT_PERSON:

# OPTIONAL: Source where job was posted eg. LinkedIn
# Default: "the company's website"
JOB_SOURCE:

# OPTIONAL: Position applying to
# Default: "developer"
JOB_DEVELOPER: Data Engineer

# MANDATORY: Name of the role applying to
JOB_TITLE: Graduate level Data Engineer (8211)

# MANDATORY: Name of the company applying to
JOB_COMPANY: Allianz
```

Once this is done, install gems and execute the `lt` binary to generate the file. The file is created in the root directory of this project and should be opened automatically.

```(shell)
gme install os docx yaml 
./lt
```
