Project-Other-Turing
This project implements the "Other Turing" paradigm, focusing on measuring AI system consistency, sensitivity, and responsibility rather than human mimicry.

Features

AST Parser: Extracts symbolic summaries from Python code
Resonance Index: Measures text/code resonance with RSA/cosine fallback
CI Resonance Check

The project includes an automated CI system that monitors code resonance to ensure consistency and quality.

How it Works

Resonance Calculation: The system calculates a resonance score for code changes.
Threshold Check: If resonance scores fall below a default threshold (currently 0.6), the CI fails.
CLI Usage

The resonance metric can be run directly:

# Analyze a single file
PYTHONPATH=. python -m metrics.resonance_metric --input file.py --output-json results.json

# Enable verbose output and deterministic haiku echo
PYTHONPATH=. python -m metrics.resonance_metric --input file.py --verbose --seed 42

# Validate the output schema
PYTHONPATH=. python -m metrics.resonance_metric --validate-schema-only
Documentation

Schema Notes v1.1: Details on the output schema for Resonance Guard.
Resonance Philosophy: Explains the concepts of spectral_trace and resonance_echo.
Haiku Table: The fixed set of haikus used for deterministic resonance echoes.
Installation

pip install pytest jsonschema
Testing

PYTHONPATH=. pytest
Anonymization Module (C9.3) • Docs: docs/ANONYMIZATION_MODULE.md • CLI: scripts/anonymize_heart_event.py (requires HEART_PROTOCOL_SALT) • Batch: scripts/run_anonymization.sh → heart_ledger_anonymized.jsonl • Tests: pytest -q, plus scripts/validate_anonymizer.py smoke test

Anonymization Module (C9.3) • Docs: docs/ANONYMIZATION_MODULE.md • CLI: scripts/anonymize_heart_event.py (requires HEART_PROTOCOL_SALT) • Batch: scripts/run_anonymization.sh → heart_ledger_anonymized.jsonl • Tests: pytest -q, plus scripts/validate_anonymizer.py smoke test 
