# txcov19_inference
A **work-in-progress** model for COVID-19 infections in Texas taking vaccinations into account, built on PyMC3. Forked from the [Priesemann Group's model](https://github.com/Priesemann-Group/covid19_inference).

I currently have a squared exponential kernel implemented, which can be used via cov19_inference.models.lambda_t_gp. Call with inputs mu (recovery rate RV), prior distribution (or constant) for the length scale of the kernel, and the prior distribution (or constant) for the amplitude of the kernel.


### Model Features (implemented) ###
* Instead of using change-points to model time-varying changes in the transmission rate, use a Gaussian process prior to describe the covariance of the effective reproduction number R_t in time.

### Model Features (planned) ###
* Incorporates vaccination data.
* Hierarchical models.
