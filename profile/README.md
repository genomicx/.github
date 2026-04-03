# GenomicX

**Can bioinformatics run in the browser?**

GenomicX is an open-source experiment in compiling established bioinformatics tools to WebAssembly and running them entirely client-side. No servers, no uploads — just the browser.

Each tool is a proof of concept testing a different class of genomic analysis: pairwise alignment, sequence typing, distance estimation, scaffolding, and more. The goal is to understand where browser-based execution works well and where it falls short.

---

### Tools

| Tool | What it tests | Demo |
|------|--------------|------|
| **[BRIGx](https://github.com/genomicx/brigx)** | Pairwise genome alignment (LASTZ) with Web Workers | [Try it](https://brigx.genomicx.org) |
| **[MLSTx](https://github.com/genomicx/mlstx)** | minimap2 in-browser for MLST sequence typing | [Try it](https://mlstx.vercel.app) |
| **[MashtreeWebx](https://github.com/genomicx/mashtreewebx)** | Mash sketch distances compiled to WASM | [Try it](https://mashtreewebx.vercel.app) |
| **[RonaQC](https://github.com/genomicx/ronaQC)** | Full QC pipeline (samtools + ivar) client-side on BAMs | [Try it](https://rona-qc.vercel.app) |
| **[Socrux](https://github.com/genomicx/socrux)** | Genome structural typing via rRNA operon mapping | [Try it](https://socrux.vercel.app) |
| **[Barrnapx](https://github.com/genomicx/barrnapx)** | rRNA/tRNA/ncRNA annotation in-browser | [Try it](https://barrnapx.vercel.app) |
| **[assembly-statsx](https://github.com/happykhan/assembly-statsx)** | N50, GC content, and assembly QC metrics | [Try it](https://assembly-statsx.vercel.app) |
| **[snp-distsx](https://github.com/happykhan/snp-distsx)** | Pairwise SNP distance matrices from alignments | [Try it](https://snp-distsx.vercel.app) |
| **[SNP-Sitesx](https://github.com/happykhan/snp-sitesx)** | SNP site extraction with VCF/Phylip export | [Try it](https://snp-sitesx.vercel.app) |
| **[ScagaireX](https://github.com/happykhan/scagairex)** | Species-specific AMR gene filtering | [Try it](https://scagairex.vercel.app) |
| **[madansix](https://github.com/happykhan/madansix)** | Pan-genome guided contig scaffolding | [Try it](https://madansix.vercel.app) |
| **[MashX](https://github.com/genomicx/mashx)** | Mash distance species ID and metagenomics screening | [Try it](https://mashx.genomicx.org) |
| **Specx** | Species identification and assembly QC | *In progress* |
| **[Genetrax](https://github.com/genomicx/genetrax)** | AMR and virulence gene detection | *In development* |
| **pMLSTx** | Plasmid replicon typing via pMLST | *In progress* |
| **Impressx** | EMBOSS sequence analysis utilities | *In progress* |
| **Consensusx** | Consensus sequence generation from reads | *In progress* |

---

### Design decisions

- **Client-side only.** All data stays on your machine. Nothing is uploaded or transmitted.
- **Open source.** All code is public. Reproducibility requires openness.
- **Reuse established tools.** We cross-compile proven C/C++ tools to WebAssembly — the science is unchanged, only the delivery is new.

---

### Contributing

Bug reports, pull requests, and suggestions for tools to port are welcome. If you have a favourite command-line bioinformatics tool you would like to see in the browser, [open an issue](https://github.com/genomicx/genomicx.github.io/issues).

---

**Website:** [genomicx.github.io](https://genomicx.github.io)

Built by [Nabil-Fareed Alikhan](https://www.happykhan.com/) and contributors.
