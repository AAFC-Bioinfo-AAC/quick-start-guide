# Guidance: Disclosure of AI-Assisted Development

When generative artificial intelligence (AI) tools are used in the development of a bioinformatics workflow intended for public release, their use should be disclosed when they make a substantive contribution to the workflow, source code, documentation, testing, or other released material.

## What should be disclosed

The disclosure should identify, where applicable:

- the AI tool or service used;
- the general purpose for which it was used, such as code generation, code refinement, debugging, documentation, test development, or code review;
- the extent of AI involvement when it materially contributed to the released product; and
- the human review, testing, and validation applied to AI-assisted outputs.

Routine use for minor spelling, grammar, formatting, or similar editorial assistance generally does not require detailed disclosure unless organizational or publication requirements specify otherwise.

## Human responsibility

AI-generated content should not be incorporated into a publicly released workflow without appropriate human review.

The workflow developer or maintainer remains responsible for:

- scientific and technical accuracy;
- validation of code and analytical outputs;
- reproducibility of the workflow;
- protection of sensitive, confidential, or protected information;
- security and privacy considerations;
- appropriate attribution and licensing;
- compliance with applicable organizational policies and publication requirements; and
- determining whether the workflow is appropriate for public release.

AI-generated code should be treated as unreviewed code until it has been inspected and tested by a qualified person.

## Recommended repository documentation

For substantive AI use, include a short **AI Use and Responsibility Statement** in the repository, preferably in the `README.md` or another clearly identified documentation file. If AI use was extensive, a dedicated section such as `AI-assisted development` may be appropriate.

A suggested statement is:

> Generative artificial intelligence (AI) tools were used during the development of this workflow to assist with selected tasks such as code development and refinement, troubleshooting, documentation, and/or code review. All AI-generated or AI-assisted content incorporated into the released workflow was reviewed, tested, and validated by the workflow authors.
>
> AI tools were used as development aids and did not replace scientific judgment, quality control, or human oversight. The authors remain responsible for the accuracy, reproducibility, security, licensing compliance, and scientific appropriateness of the published workflow and its documentation.

## Good practice for AI-assisted code

Where AI contributes substantially to source code, developers should retain sufficient development history to demonstrate human oversight. Depending on the project, this may include Git commit history, code review records, automated tests, validation datasets, workflow execution logs, or issue/merge-request discussions.

Do not enter unpublished research data, personal information, credentials, protected information, confidential material, or other information that is not authorized for disclosure into an external AI service.

## Suggested publication-checklist item

### AI-assisted development

- [ ] Determine whether generative AI materially contributed to the workflow or documentation.
- [ ] Review and validate all AI-assisted code and scientific content.
- [ ] Confirm that no protected, sensitive, confidential, or unauthorized information was provided to the AI service.
- [ ] Review AI-assisted code for security, attribution, dependency, and licensing concerns.
- [ ] Include an AI Use and Responsibility Statement when substantive AI assistance was used.
- [ ] Ensure that a named human developer or maintainer accepts responsibility for the released workflow.
