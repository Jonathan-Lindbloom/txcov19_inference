# txcov19_inference
A **work-in-progress** model for COVID-19 infections in Texas taking vaccinations into account, built on PyMC3. Forked from the [Priesemann Group's model](https://github.com/Priesemann-Group/covid19_inference).

### Model Features (planned or implemented) ###
* Incorporates vaccination data.
* Instead of using change-points to model time-varying changes in the transmission rate, we use a Gaussian process prior to describe the covariance of the transmission rate in time.
* Hierarchical models.
