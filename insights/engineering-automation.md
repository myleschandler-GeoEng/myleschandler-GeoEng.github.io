---
Title: Automation Does Not Remove Engineering Judgement
Published: incomplete - September 2026
---

# Automation Does Not Remove Engineering Judgement

Engineering automation is most effective where repetitive tasks
are separated from interpretation and decision-making. Introducing review gates 
to scripted processes assists defining this interface; these are stages 
at which the engineer must step back and ensure the script is conducting
the analysis properly, usually with a reviewer separate from the author.

## Review Gates 

Scripts can be used by, reviewed, and built with technical and non-technical 
staff. A collaboratively-produced script involving multiple parties is 
more likely to satisfy key stakeholders. However, this creates difficulty 
where the script author (or coder) is not the person with the most technical
expertise. A review gate is vital at key stages to bring stakeholders together
to discuss the outputs and whether to re-run or proceed. This prevents an
end product being submitted and rejected due to variables not being considered.

## Selecting Review Gate Locations

Selecting a location for a review gate requires understanding the full
extent of the workflow. Review gate styles differ per workflow type and 
typically involve interrogating outputs from the script with stakeholders. 
The objective is to understand the uncertainty and validity of the results,
leading to a final decision to continue or re-run with different parameters.

## Practical Implementation

Few or no review gates result in the script appearing _magical_ and 
risk lacking engineering judgement, too many and the projected
time saved using the script is minimal compared to a manual procedure.

Automation fails where a user poorly or incorrectly understands 
the software's considerations, limitations, or method. Well-written 
documentation is vital to understand and convey concepts used in scripts,
it also helps track method validation and identify areas of further development.
