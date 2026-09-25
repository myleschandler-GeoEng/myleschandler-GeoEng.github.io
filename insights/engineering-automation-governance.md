
Title: Engineering and Automation Governance
Published: September 2026

# Engineering and Automation Governance
Automation can significantly improve the efficiency and consistency of engineering workflows, particularly where repetitive processing tasks can be standardised. However, automation does not remove the need for engineering judgement. Effective workflows explicitly define the interfaces where automated processes end and where human interpretation, challenge, and decision-making begin.

The objective of engineering governance is to ensure that technical responsibility remains with suitably qualified individuals. A workflow should make clear which stages are automated, which require review, and who is responsible for making key decisions.

## Defining Human Judgement in a Workflow
Not all engineering tasks are well-suited to automation. Data preparation, processing, quality checks, and report generation can often be scripted effectively, depending on the data formats; interpretation of results, assessment of uncertainty, and selection of design parameters typically require professional judgement. Automation can support these activities, for example, by quantifying statistical uncertainty and plotting trends, but the overall assessment of uncertainty remains an engineering decision.

Problems arise when the outputs of an automated process are treated as conclusions rather than inputs to a wider engineering assessment. This is recognised where the engineers view scripts and automation _like magic..._ A well-governed workflow identifies the points at which an engineer must review the outputs, challenge assumptions, and determine whether the results are suitable for their intended purpose.

These decision points should be defined during workflow development, rather than be introduced reactively after issues are identified during implementation on a project.

## Review Gates
Review gates provide a structured mechanism for exercising engineering judgement within an automated workflow. They are pre-defined stages where automated outputs are assessed before further processing or decision-making can occur. In my experience, implementing review gates significantly reduces engineering report revisions issued and increases the technical understanding of junior team members.

Scripts are often developed, reviewed, and used by individuals with different technical backgrounds. In some cases, the script author may have strong programming capability but may not be the most experienced subject matter expert. Review gates allow technical specialists, reviewers, and project stakeholders to assess whether the outputs are reasonable and whether the workflow should proceed.

Typical review gate decisions may include:

- Proceeding with the current workflow.
- Re-running the analysis using revised parameters.
- Acquiring additional data.
- Modifying assumptions.
- Escalating technical concerns for further review.

By defining these decisions explicitly, responsibility remains with the engineering team rather than with the automated process itself.

## Selecting Review Gate Locations
Review gates should be placed where engineering judgement materially influences the outcome of the workflow. Their location depends on the nature of the process, the uncertainty associated with the data, and the consequences of an incorrect decision.

Common locations include:

- Following data acquisition and quality assurance.
- After automated processing stages.
- Prior to design parameter selection.
- Before issuing deliverables to the client.

The aim is to focus effort where expert interpretation adds value, rather than review every part of the script. Effective review gates occur at points where reasonable engineers could reach different conclusions from the same information. 

## Documentation and Traceability
Automation can only be governed effectively if users understand how a workflow operates and what assumptions it contains. Documentation should clearly describe:

- The purpose of the workflow.
- Input requirements and limitations.
- Key assumptions and parameters.
- Validation methods.
- Defined review gate locations.
- Responsible roles and reviewers.

Good documentation improves traceability, supports quality assurance, and reduces reliance on the knowledge of individual script authors. It also provides a framework for future validation, maintenance, and improvement.

## Practical Implementation
Too few review points can result in a workflow appearing as a _black box_, where users accept outputs without understanding how they were produced or whether they are appropriate. This increases the risk of incorrect assumptions propagating through a project and makes design choices difficult to explain to a client.

Conversely, excessive review can reduce the benefits of automation by requiring constant intervention and duplicate checking. The objective is to achieve a balance where routine tasks are automated while engineering effort is concentrated on interpretation, decision-making, and risk management.

Successful automation provides a structured framework that allows engineers to apply that judgement where it has the greatest value.

## Alternatives to Review Gates
Alternative engineering governance mechanisms are available, and combinations can be implemented for further quality assurance. Mature and well-validated workflows may instead rely on:

- Automated validation and quality-control checks.
- Independent verification of scripts and algorithms.
- Benchmarking against known datasets.
- Standardised procedures and design criteria.
- Formal peer review of workflow updates.
- Controlled change-management processes.

The most effective governance framework is defined by how clearly it identifies where human judgement is required and how that judgement is exercised.
