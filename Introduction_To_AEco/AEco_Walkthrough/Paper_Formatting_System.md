# Paper Formatting System

From: AEco_Walkthrough / Introduction_To_AEco

Date: March 26, 2026

Author: AEco

---------------------------------

This is the Paper Formatting System Explanation for AEco. Everything from how papers are written to how hierarchies are utilized is explained down below:


# Axiomatic Files

These are the building blocks of AEco files; papers that contain definitions, models and epistemics for its respective folder to implement. Any paper that uses a term or model defined in an Axiomatic File must declare that dependency explicitly in its header under the Axiomatics field, citing the Axiomatic File number and the specific definitions or models it draws from.


# Hierarchies/Link-Trees

Every file follows a link-tree relationship; each inheriting a set number of axiomatics/concepts which gets passed onto the next file. A child file cannot introduce a term or model that has not been established or derivable from its parent. This means the conceptual surface area of any given file is strictly bounded by what was passed down to it; no file is self-grounding.

The tree is 100% directional: inheritance flows downward from Axiomatic Files through successive modulars, and no file may cite a descendant as a dependency. The root of any branch is always an Axiomatic File.
When a file extends or redefines an inherited concept, it must note the divergence explicitly; either as a refinement (narrowing the definition) or a derivation (building a new model from it). Silent overrides are not permitted.


# Paper Template

Because this is a repository that spans every paradigm, every modular that exists in their paradigm would be built on an inherited tree of concepts, depending on the axiomatics of the previous modular (SEE AEco_Modularization_System.md for info).

The kind of protocol would vary between tiers and their respective modular. However the protocol follows a consistent template that lists the author's name, date, paper title, tree dependance and axiomatics.


TEMPLATE:

- Hashtag {TITLE}
- From {PARENT FOLDER} + {Nth FOLDER/FILE}
- Date: MM DD, YYYY
- Author: {AUTHOR'S HANDLE}

- Axiomatics {AXIOMATICS FILE NUMBER}**

[DASH LINE GOES HERE] - - - - [DASH LINE GOES HERE]

- AXIOMS

    - DEFINITION / MODEL 1
    - DEFINITION / MODEL ...
    - DEFINITION / MODEL N

- [MODEL IS BUILT FROM AXIOMS HERE]

- MODEL'S THESIS
- MODEL'S EXPLANATION
- MODEL'S CONCLUSION



**For files that depend on definitions/models specified outside of it, it should include the title of the axiomatics file & the respective items pulled from it. Axiomatic files sit on the top layer of the respective folder for files below to build concepts on top of it and must be referenced. 