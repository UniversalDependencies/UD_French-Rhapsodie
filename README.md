# Summary

A Universal Dependencies corpus for spoken French.

# Introduction

The corpus was converted automatically from the [Rhapsodie treebank](https://rhapsodie.modyco.fr/) with manual corrections.
The treebank in maintained in the repository [SUD_French-Rhapsodie](https://github.com/surfacesyntacticud/SUD_French-Rhapsodie) in the [SUD](https://surfacesyntacticud.github.io/) annotation schema.

The SUD version is also available with prosodic annotation (see [SUD README.md](https://github.com/surfacesyntacticud/SUD_French-Rhapsodie/blob/master/README.md)).

# Structure

+ fr_rhapsodie-ud-train.conllu 1,288 sentences and 19,138 tokens
+ fr_rhapsodie-ud-dev.conllu 1,081 sentences 12,906 tokens
+ fr_rhapsodie-ud-test.conllu  840 sentences 12,187 tokens
+ total 3,209 sentences 44,231 tokens

# Acknowledgement
The final discussions on the guidelines for spoken treebanks were supported by the COST Action CA21167 —Universality, diversity and idiosyncrasy in language technology ([UniDive](https://unidive.lisn.upsaclay.fr/)).
Resource maintenance has been supported by [Autogramm](https://autogramm.github.io/en/), ANR (Agence Nationale de la Recherche), Projet-ANR-21-CE38-0017 (2021-2026).


# Changelog

* 2026-11-15 v2.19
  * Implement Co-construction as described in the [proposal](https://grew.fr/spoken-language-guidelines/workgroups/spoken-data/).
  * Restore basic (non-layered) `Tense` morphosyntactic features on `VERB` with `VerbForm=Part`. Feature status is now recorded in the MISC column with  `Status[Tense]=Denom`.
* 2026-05-15 v2.18
  * Restore basic (non-layered) `Gender` and `Number` morphosyntactic features on `NOUN` and `ADJ`. Feature status is now recorded in the MISC column with  `Exponence[Gender]` and `Exponence[Number]` (see [#985](https://github.com/UniversalDependencies/docs/issues/985)).
* 2025-11-15 v2.17
  * Introduction of layered morphosyntactic features `Gender[lex]` on `NOUN` and `Tense[denom]` on `VERB` with `VerbForm=Part` 
  * More metadata
  * Sound alignement
* 2024-05-15 v2.14
  * Introduction of layered morphosyntactic features `Gender[ctxt]` and `Number[ctxt]` on `ADJ`.
  * Fix a few inconsistent annotation of idioms
  * See [SUD commit logs](https://github.com/surfacesyntacticud/SUD_French-Rhapsodie/commits/master/) for more details
* 2021-11-15 v2.9
  * Repository renamed from UD_French-Spoken to UD_French-Rhapsodie.
* 2020-11-15 v2.7
  * Morphology added
* 2018-04-15 v2.2
  * Initial release


=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.2
License: CC BY-SA 4.0
Includes text: yes
Parallel: no
Genre: spoken
Lemmas: converted from manual
UPOS: converted with corrections
XPOS: not available
Features: not available
Relations: converted with corrections
Contributors: Gerdes, Kim; Kahane, Sylvain; Nakhlé, Mariam; Yan, Chunxiao; Etienne, Aline; Courtin, Marine; Guillaume, Bruno
Contributing: here
Contact: kim@gerdes.fr
===============================================================================
