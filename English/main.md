---
title: 'Quantum Mechanics'
author:
- 'Wikipedia'
date: 'May 16th, 2020'
abstract:
- 'Quantum mechanics is, at least at first glance and at least in part, a mathematical machine for predicting the behaviors of microscopic particles — or, at least, of the measuring instruments we use to explore those behaviors — and in that capacity, it is spectacularly successful: in terms of power and precision, head and shoulders above any theory we have ever had. Mathematically, the theory is well understood; we know what its parts are, how they are put together, and why, in the mechanical sense (i.e., in a sense that can be answered by describing the internal grinding of gear against gear), the whole thing performs the way it does, how the information that gets fed in at one end is converted into what comes out the other. The question of what kind of a world it describes, however, is controversial; there is very little agreement, among physicists and among philosophers, about what the world is like according to quantum mechanics. Minimally interpreted, the theory describes a set of facts about the way the microscopic world impinges on the macroscopic one, how it affects our measuring instruments, described in everyday language or the language of classical mechanics. Disagreement centers on the question of what a microscopic world, which affects our apparatuses in the prescribed manner, is, or even could be, like intrinsically; or how those apparatuses could themselves be built out of microscopic parts of the sort the theory describes.'
output:
    pdf_document:
        pdf_engine: 'pdflatex'
        path: './main.pdf'
        includes:
            in_header: 'header.tex'
            before_body: 'doc_prefix.tex'
            after_body: 'doc_suffix.tex'
        pandoc_args:
        - '--filter=pandoc-crossref'
        - '--filter=pandoc-citeproc'
documentclass: 'report'
classoption:
- 'twoside'
- 'openright'
papersize: 'a4'
geometry:
- 'left=1.5in'
- 'right=1in'
- 'top=1.2in'
- 'bottom=1.2in'
fontenc: 'T1'
fontsize: '11pt'
mainfont: NewComputerModern
mainfontoptions:
- 'Extension=.otf'
- 'UprightFont=NewCM10-Regular'
- 'BoldFont=NewCM10-Bold'
- 'ItalicFont=NewCM10-Italic'
- 'BoldItalicFont=NewCM10-BoldItalic'
linestretch: '1.5'
indent: true
toc: true
#numbersections: true
#hyperrefoptions:
#- 'linktoc=all'
bibliography:
- 'refs/bibliography.bib'
csl: 'refs/american-physics-society.csl'
export_on_save:
    pandoc: true
---

# Introduction

Quantum mechanics (QM; also known as quantum physics, quantum theory, the wave mechanical model and matrix mechanics), including quantum field theory, is a fundamental theory in physics. It describes advanced properties of nature on an atomic scale. [@Feynman1964]

Classical physics, the description of physics that existed before the theory of relativity and quantum mechanics, describes many aspects of nature at a. ordinary (macroscopic) scale. Quantum mechanics also explains the aspects of nature at a small (atomic and subatomic) scales.

Most theories in classical physics can be derived from quantum mechanics as an approximation valid at large (macroscopic) scale. Quantum mechanics differs from classical physics in that energy, momentum, angular momentum, and other quantities of a bound system are restricted to discrete values (quantization), objects have characteristics of both particles and waves (wave-particle duality), and there are limits to how accurately the value of a physical quantity can be predicted prior to its measurement, given a complete set of initial conditions (the uncertainty principle).

![The 1927 Solvay Conference in Brussels was the fifth world physics conference.](figures/Solvay_conference_1927.jpg){width=60%}

Quantum mechanics arose gradually, from theories to explain observations which could not be reconciled with classical physics, such as Max Planck's solution in 1900 to the black-body radiation problem, and the correspondence between energy and frequency in Albert Einstein's 1905 paper which explained the photoelectric effect. Early quantum theory was profoundly re-conceived in the mid-1920s by Erwin Schrödinger, Werner Heisenberg, Max Born and others. The modern theory is formulated in various specially developed mathematical formalisms. In one of them, a mathematical function, the wave function, provides information about the probability amplitude of energy, momentum, and other physical properties of a particle.

# Methods

Scientific inquiry into the wave nature of light began in the 17th and 18th centuries, when scientists such as Robert Hooke, Christiaan Huygens and Leonhard Euler proposed a wave theory of light based on experimental observations. In 1803, English polymath Thomas Young described the famous double-slit experiment. This experiment played a major role in the general acceptance of the wave theory of light.

In 1838, Michael Faraday discovered cathode rays. These studies were followed by the 1859 statement of the black-body radiation problem by Gustav Kirchhoff, the 1877 suggestion by Ludwig Boltzmann that the energy states of a physical system can be discrete, and the 1900 quantum hypothesis of Max Planck. Planck's hypothesis that energy is radiated and absorbed in discrete "quanta" (or energy packets) precisely matched the observed patterns of black-body radiation.

In 1896, Wilhelm Wien empirically determined a distribution law of black-body radiation, called Wien's law. Ludwig Boltzmann independently arrived at this result by considerations of Maxwell's equations. However, it was valid only at high frequencies and underestimated the radiance at low frequencies.

The foundations of quantum mechanics were established during the first half of the 20th century by Max Planck, Niels Bohr, Werner Heisenberg, Louis de Broglie, Arthur Compton, Albert Einstein, Erwin Schrödinger, Max Born, John von Neumann, Paul Dirac, Enrico Fermi, Wolfgang Pauli, Max von Laue, Freeman Dyson, David Hilbert, Wilhelm Wien, Satyendra Nath Bose, Arnold Sommerfeld, and others. The Copenhagen interpretation of Niels Bohr became widely accepted.

Max Planck corrected this model using Boltzmann's statistical interpretation of thermodynamics and proposed what is now called Planck's law, which led to the development of quantum mechanics. After Planck's solution in 1900 to the black-body radiation problem (reported 1859), Albert Einstein offered a quantum-based explanation of the photoelectric effect (1905, reported 1887). Around 1900–1910, the atomic theory but not the corpuscular theory of light first came to be widely accepted as scientific fact; these latter theories can be considered quantum theories of matter and electromagnetic radiation, respectively. However, the photon theory was not widely accepted until about 1915. Even until Einstein's Nobel Prize, Niels Bohr did not believe in the photon.

Among the first to study quantum phenomena were Arthur Compton, C. V. Raman, and Pieter Zeeman, each of whom has a quantum effect named after him. Robert Andrews Millikan studied the photoelectric effect experimentally, and Albert Einstein developed a theory for it. At the same time, Ernest Rutherford experimentally discovered the nuclear model of the atom, and Niels Bohr developed a theory of atomic structure, confirmed by the experiments of Henry Moseley. In 1913, Peter Debye extended Bohr's theory by introducing elliptical orbits, a concept also introduced by Arnold Sommerfeld. This phase is known as old quantum theory.

According to Planck, each energy element (E) is proportional to its frequency (\(\nu\)): \[E=h\nu,\] {#eq:photon-energy} where h is Planck's constant.

Planck cautiously insisted that this was only an aspect of the processes of absorption and emission of radiation and was not the physical reality of the radiation. In fact, he considered his quantum hypothesis a mathematical trick to get the right answer rather than a sizable discovery. However, in 1905 Albert Einstein interpreted Planck's quantum hypothesis realistically and used it to explain the photoelectric effect, in which shining light on certain materials can eject electrons from the material. Einstein won the 1921 Nobel Prize in Physics for this work.

Einstein further developed this idea to show that an electromagnetic wave such as light could also be described as a particle (later called the photon), with a discrete amount of energy that depends on its frequency. In his paper “On the Quantum Theory of Radiation,” Einstein expanded on the interaction between energy and matter to explain the absorption and emission of energy by atoms. Although overshadowed at the time by his general theory of relativity, this paper articulated the mechanism underlying the stimulated emission of radiation, which became the basis of the laser.

In the mid-1920s, quantum mechanics was developed to become the standard formulation for atomic physics. In the summer of 1925, Bohr and Heisenberg published results that closed the old quantum theory. Due to their particle-like behavior in certain processes and measurements, light quanta came to be called photons (1926). In 1926 Erwin Schrödinger suggested a partial differential equation for the wave functions of particles like electrons. And when effectively restricted to a finite region, this equation allowed only certain modes, corresponding to discrete quantum states – whose properties turned out to be exactly the same as implied by matrix mechanics. Einstein's simple postulation spurred a flurry of debate, theorizing, and testing. Thus, the entire field of quantum physics emerged, leading to its wider acceptance at the Fifth Solvay Conference in 1927.

It was found that subatomic particles and electromagnetic waves are neither simply particle nor wave but have certain properties of each. This originated the concept of wave–particle duality.

By 1930, quantum mechanics had been further unified and formalized by David Hilbert, Paul Dirac and John von Neumann with greater emphasis on measurement, the statistical nature of our knowledge of reality, and philosophical speculation about the 'observer'. It has since permeated many disciplines, including quantum chemistry, quantum electronics, quantum optics, and quantum information science. It also provides a useful framework for many features of the modern periodic table of elements, and describes the behaviors of atoms during chemical bonding and the flow of electrons in computer semiconductors, and therefore plays a crucial role in many modern technologies. Its speculative modern developments include string theory and quantum gravity theory.

While quantum mechanics was constructed to describe the world of the very small, it is also needed to explain some macroscopic phenomena such as superconductors and superfluids.

The word quantum derives from the Latin, meaning "how great" or "how much". In quantum mechanics, it refers to a discrete unit assigned to certain physical quantities such as the energy of an atom at rest (see Figure 1). The discovery that particles are discrete packets of energy with wave-like properties led to the branch of physics dealing with atomic and subatomic systems which is today called quantum mechanics. It underlies the mathematical framework of many fields of physics and chemistry, including condensed matter physics, solid-state physics, atomic physics, molecular physics, computational physics, computational chemistry, quantum chemistry, particle physics, nuclear chemistry, and nuclear physics. Some fundamental aspects of the theory are still actively studied.

Quantum mechanics is essential for understanding the behavior of systems at atomic length scales and smaller. If the physical nature of an atom were solely described by classical mechanics, electrons would not orbit the nucleus, since orbiting electrons emit radiation (due to circular motion) and so would quickly lose energy and collide with the nucleus. This framework was unable to explain the stability of atoms. Instead, electrons remain in an uncertain, non-deterministic, smeared, probabilistic wave–particle orbital about the nucleus, defying the traditional assumptions of classical mechanics and electromagnetism.

Quantum mechanics was initially developed to provide a better explanation and description of the atom, especially the differences in the spectra of light emitted by different isotopes of the same chemical element, as well as subatomic particles. In short, the quantum-mechanical atomic model has succeeded spectacularly in the realm where classical mechanics and electromagnetism falter.

Broadly speaking, quantum mechanics incorporates four classes of phenomena for which classical physics cannot account:

* quantization of certain physical properties
* quantum entanglement
* principle of uncertainty
* wave–particle duality

# Results

In the mathematically rigorous formulation of quantum mechanics developed by Paul Dirac, David Hilbert, John von Neumann, and Hermann Weyl, the possible states of a quantum mechanical system are symbolized as unit vectors (called state vectors). Formally, these vectors are elements of a complex separable Hilbert space – variously called the state space or the associated Hilbert space of the system – that is well defined up to a complex number of norm 1 (the phase factor). In other words, the possible states are points in the projective space of a Hilbert space, usually called the complex projective space. The exact nature of this Hilbert space is dependent on the system – for example, the state space for position and momentum states is the space of square-integrable functions, while the state space for the spin of a single proton is just the product of two complex planes. Each observable is represented by a maximally Hermitian (precisely: by a self-adjoint) linear operator acting on the state space. Each eigenstate of an observable corresponds to an eigenvector of the operator, and the associated eigenvalue corresponds to the value of the observable in that eigenstate. If the operator's spectrum is discrete, the observable can attain only those discrete eigenvalues.

In the formalism of quantum mechanics, the state of a system at a given time is described by a complex wave function, also referred to as state vector in a complex vector space. This abstract mathematical object allows for the calculation of probabilities of outcomes of concrete experiments. For example, it allows one to compute the probability of finding an electron in a particular region around the nucleus at a particular time. Contrary to classical mechanics, one can never make simultaneous predictions of conjugate variables, such as position and momentum, to arbitrary precision. For instance, electrons may be considered (to a certain probability) to be located somewhere within a given region of space, but with their exact positions unknown. Contours of constant probability density, often referred to as "clouds", may be drawn around the nucleus of an atom to conceptualize where the electron might be located with the most probability. Heisenberg's uncertainty principle quantifies the inability to precisely locate the particle given its conjugate momentum.

According to one interpretation, as the result of a measurement, the wave function containing the probability information for a system collapses from a given initial state to a particular eigenstate. The possible results of a measurement are the eigenvalues of the operator representing the observable – which explains the choice of Hermitian operators, for which all the eigenvalues are real. The probability distribution of an observable in a given state can be found by computing the spectral decomposition of the corresponding operator. Heisenberg's uncertainty principle is represented by the statement that the operators corresponding to certain observables do not commute.

![Wavefunctions of the electron in a hydrogen atom at different energy levels. Quantum mechanics cannot predict the exact location of a particle in space, only the probability of finding it at different locations. The brighter areas represent a higher probability of finding the electron.](figures/Hydrogen_Density_Plots.png){width=60%}

The probabilistic nature of quantum mechanics thus stems from the act of measurement. This is one of the most difficult aspects of quantum systems to understand. It was the central topic in the famous Bohr–Einstein debates, in which the two scientists attempted to clarify these fundamental principles by way of thought experiments. In the decades after the formulation of quantum mechanics, the question of what constitutes a "measurement" has been extensively studied. Newer interpretations of quantum mechanics have been formulated that do away with the concept of "wave function collapse" (see, for example, the relative state interpretation). The basic idea is that when a quantum system interacts with a measuring apparatus, their respective wave functions become entangled, so that the original quantum system ceases to exist as an independent entity. For details, see the article on measurement in quantum mechanics.

Generally, quantum mechanics does not assign definite values. Instead, it makes a prediction using a probability distribution; that is, it describes the probability of obtaining the possible outcomes from measuring an observable. Often these results are skewed by many causes, such as dense probability clouds. Probability clouds are approximate (but better than the Bohr model) whereby electron location is given by a probability function, the wave function eigenvalue, such that the probability is the squared modulus of the complex amplitude, or quantum state nuclear attraction. Naturally, these probabilities will depend on the quantum state at the "instant" of the measurement. Hence, uncertainty is involved in the value. There are, however, certain states that are associated with a definite value of a particular observable. These are known as eigenstates of the observable ("eigen" can be translated from German as meaning "inherent" or "characteristic").

In the everyday world, it is natural and intuitive to think of everything (every observable) as being in an eigenstate. Everything appears to have a definite position, a definite momentum, a definite energy, and a definite time of occurrence. However, quantum mechanics does not pinpoint the exact values of a particle's position and momentum (since they are conjugate pairs) or its energy and time (since they too are conjugate pairs). Rather, it provides only a range of probabilities in which that particle might be given its momentum and momentum probability. Therefore, it is helpful to use different words to describe states having uncertain values and states having definite values (eigenstates).

Usually, a system will not be in an eigenstate of the observable (particle) we are interested in. However, if one measures the observable, the wave function will instantaneously be an eigenstate (or "generalized" eigenstate) of that observable. This process is known as wave function collapse, a controversial and much-debated process that involves expanding the system under study to include the measurement device. If one knows the corresponding wave function at the instant before the measurement, one will be able to compute the probability of the wave function collapsing into each of the possible eigenstates.

For example, the free particle in the previous example will usually have a wave function that is a wave packet centered around some mean position x0 (neither an eigenstate of position nor of momentum). When one measures the position of the particle, it is impossible to predict with certainty the result. It is probable, but not certain, that it will be near x0, where the amplitude of the wave function is large. After the measurement is performed, having obtained some result x, the wave function collapses into a position eigenstate centered at x.

The time evolution of a quantum state is described by the Schrödinger equation, in which the Hamiltonian (the operator corresponding to the total energy of the system) generates the time evolution. The time evolution of wave functions is deterministic in the sense that – given a wave function at an initial time – it makes a definite prediction of what the wave function will be at any later time.

During a measurement, on the other hand, the change of the initial wave function into another, later wave function is not deterministic, it is unpredictable (i.e., random). A time-evolution simulation can be seen here.

Wave functions change as time progresses. The Schrödinger equation describes how wave functions change in time, playing a role similar to Newton's second law in classical mechanics. The Schrödinger equation, applied to the aforementioned example of the free particle, predicts that the center of a wave packet will move through space at a constant velocity (like a classical particle with no forces acting on it). However, the wave packet will also spread out as time progresses, which means that the position becomes more uncertain with time. This also has the effect of turning a position eigenstate (which can be thought of as an infinitely sharp wave packet) into a broadened wave packet that no longer represents a (definite, certain) position eigenstate.

Some wave functions produce probability distributions that are constant, or independent of time – such as when in a stationary state of definite energy, time vanishes in the absolute square of the wave function (this is the basis for the energy-time uncertainty principle). Many systems that are treated dynamically in classical mechanics are described by such "static" wave functions. For example, a single electron in an unexcited atom is pictured classically as a particle moving in a circular trajectory around the atomic nucleus, whereas in quantum mechanics, it is described by a static, spherically symmetric wave function surrounding the nucleus (however, only the lowest angular momentum states, labeled s, are spherically symmetric.)

The Schrödinger equation acts on the entire probability amplitude, not merely its absolute value. Whereas the absolute value of the probability amplitude encodes information about probabilities, its phase encodes information about the interference between quantum states. This gives rise to the "wave-like" behavior of quantum states.

Analytic solutions of the Schrödinger equation are known for very few relatively simple model Hamiltonians including the quantum harmonic oscillator, the particle in a box, the dihydrogen cation, and the hydrogen atom. Even the helium atom – which contains just two electrons – has defied all attempts at a fully analytic treatment.

However, there are techniques for finding approximate solutions. One method, called perturbation theory, uses the analytic result for a simple quantum mechanical model to create a result for a related but more complicated model by (for example) the addition of a weak potential energy. Another method is called "semi-classical equation of motion", which applies to systems for which quantum mechanics produces only small deviations from classical behavior. These deviations can then be computed based on the classical motion. This approach is particularly important in the field of quantum chaos.

# Conclusion

Since its inception, the many counter-intuitive aspects and results of quantum mechanics have provoked strong philosophical debates and many interpretations. Even fundamental issues, such as Max Born's basic rules about probability amplitudes and probability distributions, took decades to be appreciated by society and many leading scientists. Richard Feynman once said, "I think I can safely say that nobody understands quantum mechanics." According to Steven Weinberg, "There is now in my opinion no entirely satisfactory interpretation of quantum mechanics."

The Copenhagen interpretation – due largely to Niels Bohr and Werner Heisenberg – remains most widely accepted some 75 years after its enunciation. According to this interpretation, the probabilistic nature of quantum mechanics is not a temporary feature which will eventually be replaced by a deterministic theory, but is instead a final renunciation of the classical idea of "causality". It also states that any well-defined application of the quantum mechanical formalism must always make reference to the experimental arrangement, due to the conjugate nature of evidence obtained under different experimental situations.

Albert Einstein, himself one of the founders of quantum theory, did not accept some of the more philosophical or metaphysical interpretations of quantum mechanics, such as rejection of determinism and of causality. He famously said about this, "God does not play with dice". He rejected the concept that the state of a physical system depends on the experimental arrangement for its measurement. He held that a state of nature occurs in its own right, regardless of whether or how it might be observed. That view is supported by the currently accepted definition of a quantum state, which does not depend on the configuration space for its representation, that is to say, manner of observation. Einstein also believed that underlying quantum mechanics must be a theory that thoroughly and directly expresses the rule against action at a distance; in other words, he insisted on the principle of locality. He considered, but rejected on theoretical grounds, a particular proposal for hidden variables to obviate the indeterminism or acausality of quantum mechanical measurement. He believed that quantum mechanics was a currently valid but not a permanently definitive theory for quantum phenomena. He thought its future replacement would require profound conceptual advances, and would not come quickly or easily. The Bohr-Einstein debates provide a vibrant critique of the Copenhagen Interpretation from an epistemological point of view. In arguing for his views, he produced a series of objections, of which the most famous has become known as the Einstein–Podolsky–Rosen paradox.

John Bell showed that this EPR paradox led to experimentally testable differences between quantum mechanics and theories that rely on added hidden variables. Experiments confirmed the accuracy of quantum mechanics, thereby showing that quantum mechanics cannot be improved upon by addition of hidden variables. Alain Aspect's experiments in 1982 and many later experiments definitively verified quantum entanglement. Entanglement, as demonstrated in Bell-type experiments, does not violate causality, since it does not involve transfer of information. By the early 1980s, experiments had shown that such inequalities were indeed violated in practice – so that there were in fact correlations of the kind suggested by quantum mechanics. At first these just seemed like isolated esoteric effects, but by the mid-1990s, they were being codified in the field of quantum information theory, and led to constructions with names like quantum cryptography and quantum teleportation. Quantum cryptography is proposed for use in high-security applications in banking and government.

The Everett many-worlds interpretation, formulated in 1956, holds that all the possibilities described by quantum theory simultaneously occur in a multiverse composed of mostly independent parallel universes. This is not accomplished by introducing a "new axiom" to quantum mechanics, but by removing the axiom of the collapse of the wave packet. All possible consistent states of the measured system and the measuring apparatus (including the observer) are present in a real physical – not just formally mathematical, as in other interpretations – quantum superposition. Such a superposition of consistent state combinations of different systems is called an entangled state. While the multiverse is deterministic, we perceive non-deterministic behavior governed by probabilities, because we can only observe the universe (i.e., the consistent state contribution to the aforementioned superposition) that we, as observers, inhabit. Everett's interpretation is perfectly consistent with John Bell's experiments and makes them intuitively understandable. However, according to the theory of quantum decoherence, these "parallel universes" will never be accessible to us. The inaccessibility can be understood as follows: once a measurement is done, the measured system becomes entangled with both the physicist who measured it and a huge number of other particles, some of which are photons flying away at the speed of light towards the other end of the universe. In order to prove that the wave function did not collapse, one would have to bring all these particles back and measure them again, together with the system that was originally measured. Not only is this completely impractical, but even if one could theoretically do this, it would have to destroy any evidence that the original measurement took place (including the physicist's memory).

In light of the Bell tests, Cramer in 1986 formulated his transactional interpretation which is unique in providing a physical explanation for the Born rule. Relational quantum mechanics appeared in the late 1990s as the modern derivative of the Copenhagen Interpretation.

# Reference
