# GenomicX

GenomicX develops open-source bioinformatics tools that run in your browser. Sequence analysis runs locally on your device, using WebAssembly and JavaScript. Applications download software and reference databases as needed.

Browse the [tool catalogue](https://genomicx.org/#tools) or open an application below.

## Genomics applications

| Application | What it does | Open |
|-------------|--------------|------|
| [BRIGX](https://github.com/genomicx/brigx) | BLAST-based circular genome comparisons | [Launch](https://brigx.genomicx.org) |
| [MLSTX](https://github.com/genomicx/mlstx) | MLST allele calling with BLAST; scheme detection with minimap2 | [Launch](https://mlstx.genomicx.org) |
| [MashtreeWebX](https://github.com/genomicx/mashtreewebx) | Mash distances and neighbour-joining trees from genome assemblies | [Launch](https://mashtreex.genomicx.org) |
| [RonaQC](https://github.com/genomicx/ronaQC) | SARS-CoV-2 sequencing quality control from mapped reads | [Launch](https://ronaqc.genomicx.org) |
| [SocruX](https://github.com/genomicx/socrux) | Genome structural typing using rRNA operon arrangements | [Launch](https://socrux.genomicx.org) |
| [BarrnapX](https://github.com/genomicx/barrnapx) | rRNA, tRNA and ncRNA annotation | [Launch](https://barrnapx.genomicx.org) |
| [assembly-statsx](https://github.com/genomicx/assembly-statsx) | Assembly statistics, including N50 and GC content | [Launch](https://assembly-statsx.genomicx.org) |
| [snp-distsx](https://github.com/genomicx/snp-distsx) | Pairwise SNP distance matrices from alignments | [Launch](https://snp-distsx.genomicx.org) |
| [SNP-SitesX](https://github.com/genomicx/snp-sitesx) | SNP site extraction and VCF/Phylip export | [Launch](https://snp-sitesx.genomicx.org) |
| [ScagaireX](https://github.com/genomicx/scagairex) | Species-specific AMR gene filtering | [Launch](https://scagairex.genomicx.org) |
| [MadansiX](https://github.com/genomicx/madansix) | Contig scaffolding using pan-genome gene synteny | [Launch](https://madansix.genomicx.org) |
| [MashX](https://github.com/genomicx/mashx) | Mash-based species identification and metagenomic screening | [Launch](https://mashx.genomicx.org) |
| [GeneTrax](https://github.com/genomicx/genetrax) | BLAST-based screening for AMR, virulence and plasmid markers | [Launch](https://genetrax.genomicx.org) |
| [ConsensusX](https://github.com/genomicx/consensusx) | Read mapping, reference consensus and assembly of unmapped reads | [Launch](https://consensusx.genomicx.org) |
| [TipToftX](https://github.com/genomicx/tiptoftx) | Plasmid replicon detection from long reads | [Launch](https://tiptoftx.genomicx.org) |
| [GrapeTree](https://github.com/achtman-lab/GrapeTree) | Allele-profile tree construction and interactive tree/metadata visualisation | [Launch browser/WASM app](https://grapetree.genomicx.org/browser-wasm/) |

These links identify deployed applications. Benchmark coverage and known limitations vary by tool; consult each repository before interpreting results. Deployment is separate from scientific validation.

## Lab and conference utilities

| Application | What it does | Open |
|-------------|--------------|------|
| [BarcodeX](https://github.com/genomicx/barcodex) | Barcode generation and printable labels | [Launch](https://barcodex.genomicx.org) |
| [Conference Bingo](https://github.com/genomicx/conferencebingo) | Conference bingo card generation | [Launch](https://conferencebingo.genomicx.org) |

## Planned tools

SpecX (species identification and assembly QC), pMLSTX (plasmid MLST typing) and ImpressX (EMBOSS sequence utilities) remain planned projects without public application links.

## Development

Many tools compile established command-line software to WebAssembly; others reimplement workflows in JavaScript or TypeScript. Compatibility must be tested for each implementation rather than assumed from the original program.

[`@genomicx/ui`](https://github.com/genomicx/ui) provides shared components and light/dark styling for GenomicX applications. GrapeTree retains its own interface. Applications are hosted on Cloudflare under `*.genomicx.org`.

Bug reports and contributions are welcome in the relevant repository. For catalogue changes or suggestions for new tools, [open a website issue](https://github.com/genomicx/genomicx.github.io/issues).

Website: [genomicx.org](https://genomicx.org)

Built by [Nabil-Fareed Alikhan](https://www.happykhan.com/) and contributors, using software and databases credited in each project.
