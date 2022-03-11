# gritn
It's grit, except array lengths are passed to GAS output and can be used in code as `extern const unsigned long` variables.

## why?
Relying on grit to create a header file at build-time creates issues when multitasking gets involved. It also makes an IDE throw errors when the project is unbuilt. It's nicer to create a C macro that can point to extern variables.