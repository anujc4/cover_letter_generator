# COVER LETTER GENERATOR

Generates a word document from a predefined template and replaces the defined
template variables.

## Prerequisites

Ruby

## Usage

> Keep a variable name called `CANDIDATE_NAME` which is your name and `JOB_COMPANY` which is the name of the
> company you are applying to. This makes it easier for the app to spit out a proper file name. 

Edit the `varibles.yml` file. Add any variable name you want. Just make sure that the variable name is present in the
document in the format {{variable_name}}.

```(yaml)
# Your name
CANDIDATE_NAME: Anuj Chandra

# Name of the person addressing the letter to
JOB_CONTACT_PERSON: HR Manager

# Source where job was posted eg. LinkedIn
JOB_SOURCE: the company's website

# Position applying to
JOB_DEVELOPER: developer

# Name of the role applying to
JOB_TITLE: Engineer

# Name of the company applying to
JOB_COMPANY: FooBar
```

Once this is done, install gems and execute the `lt` binary to generate the file. The file is created in the root directory of this project and should be opened automatically.

```(shell)
gme install os docx yaml 
./lt
```
