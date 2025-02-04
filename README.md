# Proposal for a new SMEFT basis

The goal of this proposal is to establish an altenative to the Warsaw basis for the Standard Model Effective Theory (SMEFT), where some of the operators are replaced by others. The proposed changes are the following:

$O_{lequ}^{(3)}$
================

**Proposed alternative:** $O_{\ell uqe}=(\bar \ell^i u)\epsilon_{ij}(\bar q^j e)$

**Reasons:**

- Tensor operators are kwnon to cause problems with $\gamma_5$ in NDR. While the issue can be solved by using the BHMV scheme, there is no reason a priori to prefer the scalar operator over the tensor. The scalar operator also give simpler Dirac traces, also for BHMV, when performing calculations with this operator.

- The only Standard Model (SM) extension where this operator is generated at tree-level involves rank-2 antysimmetric Lorentz tensor for which, to the best of my knowledge, a renormalizable Lagrangian is not known. Instead, the operator $O_{luqe}$ is generated at tree-level by the scalar extensions $(\boldsymbol{3},\boldsymbol{2},7/6)$. Instead of $O_{\ell uqe}$, one could also use $O_{\ell q^ce^cu}=(\bar\ell \epsilon q^{c})(\bar e^c u)$, which is generated at tree level by the $S_1$ leptoquark. However, the use of $O_{luqe}$ is preferred due to the absence of charge conjugation in the operator. When Fierzing either $O_{luqe}$ or $O_{\ell q^ce^cu}$ into $O_{lequ}^{(3)}$ one has to introduce an evanescent shifts which are ambigous in NDR [[2211.09144]](https://arxiv.org/abs/2211.09144). The ambiguity is further translated to matrix element computations with this operator. 


$O_{\varphi \square}$
======================

**Proposed alternative:** $O_{DH}=(H^\dagger H)[(D_\mu H)^\dagger (D^\mu H)]$

**Reasons:**

- It seems strange to have an operator that is a linear combination with some of the terms proportional to the equations of motion (when expanding the derivatives). It would be preferable to have at most one derivate acting on a field whenever possible.

- This form of the operator aligns better with geometric extensions of the SMEFT.

- Operators such as $O_{\varphi \square}$, involving derivatives on products of fields, are not generated by any existing basis tools.


Operators containing field-strenght tensors
===========================================

**Proposed change:** Include a factor of the gauge coupling per field-strength tensor in the operator.

**Reasons:**

- In any matching and/or running result, field-strength tensors get accompanied by gauge couplings.

- It makes the perturbative couting more transparent. This becomes especially relevant in Monte Carlo tools and in evolution-matrix calculations for Renormalization Group running.


Operators with triplet (or octet) currents
==========================================

**Proposed change:** Remove the generator products in favor of cross-term singlet contractions. E.g. instead of $O_{qq}^{(3)}$ write $O_{qq}^\prime=(\bar q^i \gamma_\mu q^j) (\bar q^j \gamma^\mu q^i)$ and analogusly for the rest.

**Reasons:**

- It makes SU(2) and color algebra simpler.

- There is no phenomenological reason for prefering one form over the other.
