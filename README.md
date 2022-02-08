# paas-the-parser

From [ongoing discussions](https://github.com/MADICES/MADICES-2022/discussions/33#discussioncomment-2134909):

> We discussed how parsing unstructured logs/output files is still very common. Everyone's writes their own parser that maps to their own data models. Usually these are bundled as part of larger packages that do the analysis (e.g. pymatgen, Ase, aiida in comp. mat. sci), and rewritten in multiple languages (e.g. the modular cheminfo parsers in JS).

> Do we think a simple registry/framework for code objects that operate on files and return structured data would be a useful investment? e.g., a docker image per parser with a unified interface that also spits out a schema for the parsed data? Do such things already exist? Does this go any way to tackling the scalability of our current ecosystem, or is this just creating more laborious work? This could then motivate the development by the original raw file creators, like instrument manufacturers and code authors.

>These could then be employed across multiple ELN/repository services and used for ETL in perhaps a more scalable way than is currently available. Given the wealth of existing parsers it would be easy to test this out quite quickly, and there is potential for nice integration with many existing services present at the workshop.

## Prior art

- @kjappelbaum's work within the cheminfo ecosystem on a registry of chemical files: [kjappelbaum/chemical-files-registry](https://github.com/kjappelbaum/chemical-files-registry) which was supposed to feed the [app registry](https://fervent-banach-4255bd.netlify.app/)
