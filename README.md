# ALP_CalcHEP
This respository contains CalcHEP model files for a model including a dark matter Dirac fermion ($\chi$) and an axion-like particle ($a$). The ALP couples to electroweak gauge bosons and to dark matter. This model follows the conventions of arXiv:2405.xyzab. Please cite this paper if you use this CalcHEP model.

## Coupling conventions
The couplings are defined according to the following Lagrangian,

$$ -\frac{1}{2f}\partial_\mu a \bar\chi\gamma^\mu\gamma^5\chi - \frac{C_{a\gamma\gamma}}{4}F_{\mu\nu}\tilde{F}^{\mu\nu}-\frac{C_{aZZ}}{4}Z_{\mu\nu}\tilde{Z}^{\mu\nu}-\frac{C_{a\gamma Z}}{2}F_{\mu\nu}\tilde{Z}^{\mu\nu}-\frac{C_{aWW}}{2}W^+_{\mu\nu}\tilde{W}^{-\mu\nu}
$$

## Setting up CalcHEP model with micrOMEGAs
Follow the instructions on the [micrOMEGAs homepage](https://lapth.cnrs.fr/micromegas/). As of micrOMEGAs v5, you can set up the model as follows:
- Go to the micrOMEGAs home directory
- Execute ./newProject my-project-name
- Copy all the .mdl files to the my-project-name/work/models directory
- Go to my-project-name and build the micrOMEGAs code

You can use the provided micromegas.par file as input parameters to micrOMEGAs. Note that you must provide the reciprocal of the ALP decay constant as an input parameter, $\mathrm{finv} = 1/f$
