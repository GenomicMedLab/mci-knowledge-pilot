# Molecular Characterization Initiative (MCI) Knowledge Pilot

[![Actions status](https://github.com/genomicmedlab/mci_knowledge_pilot/actions/workflows/checks.yaml/badge.svg)](https://github.com/genomicmedlab/mci_knowledge_pilot/actions/checks.yaml)

This repository contains a pilot effort to transform semi-structured somatic cancer variant classification knowledge into computable clinical assertions using [GA4GH Genomic Knowledge Standards (GKS)](https://www.ga4gh.org/work_stream/genomic-knowledge-standards/).

Previously captured clinical significance classifications from spreadsheets were programmatically mapped to the [GA4GH Variant Annotation Specification (VA-Spec)](https://www.ga4gh.org/product/variant-annotation/) to evaluate approaches for reducing knowledge silos and improving interoperability.

---

## Development

Clone the repo and create a virtual environment:

```shell
git clone https://github.com/genomicmedlab/mci_knowledge_pilot
cd mci_knowledge_pilot
python3 -m virtualenv venv
source venv/bin/activate
```

Install development dependencies and `prek`:

```shell
python3 -m pip install -e '.[dev]'
prek install
```

Check style with `ruff`:

```shell
python3 -m ruff format . && python3 -m ruff check --fix .
```
