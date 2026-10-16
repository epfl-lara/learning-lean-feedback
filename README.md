# Learning Lean Feedback

Learned evaluators that predict Lean 4 verdicts and compiler feedback (goal states and error messages) for candidate proofs, and hybrid GRPO rewards that combine their predictions with Lean.

**Status:** code coming soon. The training, evaluation, and GRPO code will be added to this repository.

## Models and datasets

Available in the Hugging Face collection [EPFL-LARA/learning-lean-feedback](https://huggingface.co/collections/EPFL-LARA/learning-lean-feedback):

- [`lean-encoder-modernbert-large`](https://huggingface.co/EPFL-LARA/lean-encoder-modernbert-large): ModernBERT-large validity classifier
- [`lean-one-token-qwen3-8b`](https://huggingface.co/EPFL-LARA/lean-one-token-qwen3-8b): Qwen3-8B one-token validity classifier
- [`lean-feedback-qwen3-4b`](https://huggingface.co/EPFL-LARA/lean-feedback-qwen3-4b): Qwen3-4B feedback model
- [`lean-compiler-training-corpus`](https://huggingface.co/datasets/EPFL-LARA/lean-compiler-training-corpus): 4.84M compiler-labelled Lean programs (Lean v4.15.0)
- [`lean-evaluation-benchmark`](https://huggingface.co/datasets/EPFL-LARA/lean-evaluation-benchmark): 68,932 candidate programs from three public provers on miniF2F and ProofNet

## Paper

Lazar Milikic, Etienne Bamas, Emmanuel Abbe, Viktor Kunčak. *Learning Lean Feedback for Efficient Proof-Candidate Evaluation on GPUs.* NeurIPS 2026 Workshop on AI for Verifiable Coding (VeriCodeGen).

## Citation

If you use this work, please cite:

```bibtex
@misc{milikic2026learningleanfeedbackefficient,
  title={Learning Lean Feedback for Efficient Proof-Candidate Evaluation on GPUs},
  author={Lazar Milikic and Etienne Bamas and Emmanuel Abbe and Viktor Kunčak},
  year={2026},
  eprint={2610.21881},
  archivePrefix={arXiv},
  primaryClass={cs.LG},
  url={https://arxiv.org/abs/2610.21881},
}
```

## License

The code in this repository is released under the Apache License 2.0 (see [LICENSE](LICENSE)).
