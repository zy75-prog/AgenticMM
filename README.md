# AgenticMM

AgenticMM is a material-centered multi-agent architecture for scalable first-principles materials modeling. One persistent agent owns each material's workflow and scientific state, and one coordinator manages shared computing resources, communication, and campaign progress. Externally supplied MatterSkills define the scientific workflows.

![AgenticMM architecture](figures/figure_1.png)

This repository accompanies *AgenticMM: A Material-Centered Multi-Agent Architecture for Scalable First-Principles Materials Modeling* by Zhenkun Yuan and Geoffroy Hautier.

## Repository contents

- [AgenticMM.pdf](AgenticMM.pdf) contains an introduction and the architecture and execution protocol (Sections II and III).
- [AgenticMM.tex](AgenticMM.tex) is the LaTeX source.
- [figures/](figures/) contains the architecture diagram.

## How to use

1. Open a new Codex chat.
2. Attach [AgenticMM.pdf](AgenticMM.pdf) and the MatterSkills for your workflow, such as [DefectSkills.pdf](https://github.com/zy75-prog/DefectSkills/blob/main/DefectSkills.pdf) for VASP-based point-defect calculations.
3. Send a request like this, replacing the bracketed text.

   > I want to study [property or scientific question] for [list of materials], using the AgenticMM architecture to implement the supplied MatterSkills. Set up one coordinator agent and one distinct material agent per material.

4. Answer the coordinator’s setup questions to specify the authorized computing environment, working directory, and any material-specific requirements.
5. Follow the readiness checks in Section III. Approve the campaign setup and verify the recorded agent assignments before authorizing calculations.

## License

The documentation and architecture figure in this repository are licensed under CC BY 4.0. See [LICENSE.md](LICENSE.md) for the scope and attribution.
