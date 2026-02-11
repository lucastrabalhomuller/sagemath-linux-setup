# Installing SageMath (Conda Environment)

This text describes the complete installation of SageMath on Linux using Conda
(Miniforge). The installation is performed inside an isolated environment, which
avoids conflicts with system packages and ensures full reproducibility across
different machines.

After installing Miniforge, Conda is not initialized automatically. For this
reason, each new terminal session must explicitly load Conda before it can be
used. This is done by sourcing the Conda initialization script located inside
the Miniforge installation directory.

Run the following command in the terminal:

```bash
source ~/miniforge3/etc/profile.d/conda.sh
```

After loading Conda, verify that it is available by checking its version:

```bash
conda --version
```

Once Conda is available, SageMath can be installed using the conda-forge
repository. SageMath is distributed in Conda under the package name sage.
For stability and long-term compatibility, Python version 3.10 is used.

Create a new Conda environment named sage and install SageMath using a single
command:

```bash
conda create -n sage python=3.10 sage
```

This command creates an isolated Conda environment called sage, installs
Python 3.10 inside it, and installs the full SageMath distribution along with
all required dependencies. The installation process may take several minutes,
as SageMath is a large scientific software package.

After the installation finishes, the environment must be activated before
SageMath can be used. Activate the environment with:

```bash
conda activate sage
```

Once activated, the terminal prompt should indicate that the sage environment
is active, typically by showing (sage) at the beginning of the prompt.

To confirm that SageMath was installed correctly, check its version:

```bash
sage --version
```

A successful installation will produce output similar to the following:

SageMath version 10.5
Using Python 3.10.x


At this point, SageMath is fully installed, functional, and ready to be used
for symbolic and numerical scientific computations.
