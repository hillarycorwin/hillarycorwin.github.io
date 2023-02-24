# Preliminaries

1.  **Disturbance (Error) Term**

    1.  The economic theory that consumption is a function of income *C* = *f*(*Y*) is **deterministic**, where *C* represents consumption and *Y* represents income.

    2.  The econometrician adds a disturbance (or error) term so that
        *C* = *f*(*Y*) + *u*, where *u* is the disturbance term. This
        relationship is **stochastic**, having a random probability
        distribution or pattern that may be analyzed statistically but
        may not be predicted precisely. The disturbance term is the
        amount by which an observation differs from its expected value.
        The expected value, being the mean of the entire population, is
        typically unobservable, and hence the statistical error cannot
        be observed either. The disturbance term can be considered the
        net influence of any or all of the following even in a “good"
        model:

        1.  *Omission of the influence of chance events*: events too
            trivial to create omitted variable bias problems can have
            slight, irregular influence.

        2.  *Measurement error*: The dependent variable may not be able
            to be measured accurately because of data collection
            difficulties or it is immeasurable and needs a proxy.

        3.  *Human indeterminacy*: human behavior means that actions
            taken under identical circumstances can differ in some
            random way.

    3.  **Residuals** are *observable estimates* of the unobservable
        statistical error. For example, if we use a sample mean as an
        estimate of the population mean, the residual would be the
        difference between an observed value and the sample mean for any
        given unit. Note that, because of the definition of the sample
        mean, the sum of the residuals within a random sample is
        necessarily zero, and thus the residuals are necessarily not
        independent. The statistical errors, on the other hand, are
        independent, and their sum within the random sample is almost
        surely not zero.

    4.  **Parameters** are unknown constants, which tie the relevant
        variables into an equation. *β* are parameters characterizing
        the function in
        *C* = *β*<sub>1</sub> + *β*<sub>2</sub>*Y* + *u*.

    5.  The existence of the disturbance term makes the calculation of
        these parameters impossible, thus they are **estimated**.

2.  **Estimates and Estimators, Statistics and Sampling Distributions**

    1.  Econometric theory is typically complex enough that it requires
        more than one parameter, and these are estimated together in a
        vector in which *β*<sub>1</sub>...*β*<sub>*k*</sub> are elements
        of a *β* vector.

    2.  Econometric theory focuses not on the estimate itself, but on
        the **estimator**—the algebraic function of a potential sample
        of data; once the sample is drawn, this function creates a
        numerical estimate (the outcome of the estimator process).

    3.  *Sample (descriptive) statistic:* a numerical summary of the
        sample observations drawn from the population of interest

    4.  *Test Statistic:* provides another way to understand the
        characteristics of population or the data generation process
        (ex: hypothesis test: can test null hypothesis - A test
        statistic is calculated by some formula, such as t-statistic,
        and we can use this test statistic to infer the population
        parameter in a probabilistic fashion.) We can use estimators to
        estimate the coefficients of interest that best represent the
        data generation process in the population. These estimated
        coefficients can be considered test statistics.

    5.  *Probability Density Function:* A function that map the values
        of a random variable into the space of probabilities.

    6.  *Sampling Distribution*: The probability distribution of an
        estimator over all possible sample outcomes. This means that
        envisioning we can draw infinite number of samples; and, from
        each sample if we follow the same estimation procedure, use the
        same formula (estimator) to calculate our estimates, and have
        the same sample size, then we can arrange these guesses into
        probability distributions. We can envision drawing one sample
        after another sample, from each sample calculating the value of
        our guess (estimate for the population parameter), and arranging
        these guesses in the form of distribution. Since different
        samples may contain different information about the population
        parameters, the value for an estimator and for a test statistic
        could vary from samples to samples. If doing sampling infinite
        times, then these values can form a distribution.

3.  **Central Limit Theorem and the Law of Large Numbers**

    -   *Central Limit Theorem*: the distribution of sample means
        approximates a normal distribution as the sample size increases
        to infinity, regardless of population distribution shape.

    -   *Law of Large Numbers*: If you repeat an experiment
        independently a large number of times and average the result,
        what you obtain should be close to the expected value. For
        i.i.d. random variables with a finite expected value, the
        probability limit will be the expected value.

4.  **Models and Methods**

    -   *Model*: A model is simplification of reality. In statistics, a
        model for a finite number of random variables is a joint
        probability distribution of the random variables. Random
        variables are functions that map observations into the space of
        numerical values. A random variable is discrete when the values
        are either countable or finite. A continuous random variable, in
        contrast, has uncountable and infinite values. Probability
        distribution, more precisely a probability density function (for
        discrete random variables it is sometimes called probability
        mass function), is a function that maps values of a random
        variable into the space of probabilities ranging from 0 to 1.  
        when there are an infinite number of random variables, a
        statistical model is a data generation process that produces the
        random variables. An infinite number of random variables are
        usually, if not always, considered to follow an independent and
        identical probability distribution. Put simply, random variables
        have identical PDFs and the PDFs are independent with each
        other. Note that a statistical model is purely theoretical; it
        can be constructed without any empirical data.

    -   *Method*: A method is a way to estimate a statistical model
        based on empirical data. Thus, a statistical method is
        estimation. To estimate a statistical model, we first need to
        find parameters of interest. A parameter is a characteristic of
        a statistical model. For instance, a mean of normal distribution
        is a parameter that represents the central tendency of the PDF.
        Once we specify parameters of interest, we then need to find
        statistics that can be used as estimators. A statistic is a
        summary of data. A sample average, for instance, represents the
        central tendency of data. When we use a statistic to estimate a
        parameter of interest, the statistic is called an estimator. To
        identify an estimator, it should have desirable characteristics,
        such as unbiasedness and efficiency.

# Criteria for Estimators

A preferred estimator is one that most closely satisfies criteria along
several dimensions:

1.  ***Unbiasedness***: An estimator is unbiased if the sampling
    distribution of *β*<sup>\*</sup> is equal to *β*–that is, if
    *E*(*β*<sup>\*</sup>) = *β*. Bias is the difference between
    *E*(*β*<sup>\*</sup>) and *β*.

2.  ***Efficiency***: Smaller sampling variance is preferable because it
    is more likely that a given estimate is closer to the true *β*. It
    is impossible to determine mathematically which estimate has the
    smallest variance, therefore the assumption is often added that the
    estimator should be a *linear* function the observations on the DV.
    This allows for the efficient estimator to be determined
    mathematically. The estimator that is *linear*, *unbiased*, and has
    the *minimum variance* among all linear unbiased estimators is BLUE,
    the best linear unbiased estimator. (The multivariate case is harder
    to determine BLUE because the variance of *β̂* becomes the
    variance-covariance matrix of *β̂*.)

3.  ***Mean Square Error***: there can be tradeoffs between unbiasedness
    and efficiency. There may be a more efficient but somewhat biased
    estimator that produces estimates closer to the true *β* more often
    than a less efficient unbiased estimator. MSE can help resolve this
    tradeoff *if a best unbiased criterion cannot produce estimates with
    small variances*, as is the case with multicollinearity. *The MSE
    criterion minimizes the weighted average of the biases and its
    variance* using the square of the bias.

4.  ***Consistency**/Asymptotic Properties*: if the asymptotic
    distribution of *β̂* becomes concentrated on a value, k, then
    *p**l**i**m**β̂* = *k*, and k is the probability limit of *β̂*. If
    *p**l**i**m**β̂* = *β*, then *β̂* is consistent. If *β̂* is consistent
    and its asymptotic variation is lower than that of all other
    consistent estimators, then *β̂* is asymptotically efficient.
    Consistency is, crudely, the large-sample equivalent of MSE since a
    consistent estimator at its limit can have zero bias and zero
    variance.

5.  *Maximum Likelihood*: The idea that the sample is more likely to
    have come from a “real world" characterized by one set of parameter
    values than any other set. *β*<sup>*M**L**E*</sup> gives the
    greatest probability of obtaining the observed data. The MLE is the
    pair of values *μ*<sup>*M**L**E*</sup> and
    (*σ*<sup>2</sup>)<sup>*M**L**E*</sup> that creates the greatest
    probability of obtaining the observed data.

6.  *Least squares*: subtracting the estimated value of the independent
    variable, *ŷ*, from the actual values *y* yields the *residual*,
    (*y* − *ŷ*). A preferred estimator will minimize a weighted sum of
    these residuals, although there may be theoretical reasons for using
    different weights (choosing to weight equally, to drop outliers, to
    only consider some values...). The most popular is to *minimize the
    sum of squared residuals*, which the *ordinary least squares (OLS)*
    estimator does. Minimizing the sum of squared errors DOES NOT say
    anything specific about the relationship of the estimator to the
    true parameter value of *β*! Accounting for too many unique features
    of a sample can cause the estimator to lose general validity such
    that if the estimator were to be applied to a new sample, poor
    estimates would result.

7.  *Highest *R*<sup>2</sup>*: *R*<sup>2</sup> is the *coefficient of
    determination*, which is meant to represent the proportion of the
    variation in the dependent variable “explained" by variation in the
    independent variables. In linear OLS, the “total variation" of the
    dependent variable can be decomposed into “explained" (the sum of
    squared deviations of the estimated values of the dependent variable
    around their mean) and “unexplained" variation (the sum of squared
    residuals). *R*<sup>2</sup> is calculated as a ratio of the
    explained variation to the total variation. Because OLS minimizes
    the sum of squared residuals, it automatically maximizes
    *R*<sup>2</sup>. *R*<sup>2</sup> maximization is thus identical to
    the least squares criterion.

8.  *Monte Carlo*: Simulation exercise designed to shed light on the
    small-sample properties of competing estimators for a given
    estimation problem. Used when small-sample properties cannot be
    derived theoretically, or as a supplement to theoretical
    derivations. Allows direct exploration of sampling distributions
    through simulation. Steps: (1) model the data-generating
    process, (2) generate artificial datasets, (3) create estimates of
    the data using the estimator, (4) use these estimates to assess the
    estimator’s sampling distribution.

# The Classical Linear Regression Model: Assumptions, Violations, and Fixes

## Gauss-Markov Assumptions in a Linear Regression Model

The Gauss-Markov Theorem relates to the finite-sample properties of the
Ordinary Least Squares estimators and states that, under a set of
assumptions, OLS is the best unbiased linear estimator. That is, OLS is
the most efficient (has lowest variance) among all unbiased linear
estimators. This is the case if the following assumptions are met:
linearity, full-rank, strict exogeneity, and spherical error variance.
The Gauss-Markov Theorem does not have a normality of disturbances
assumption and does not specify the asymptotic properties of OLS. These
are useful concepts for weighing the costs and benefits of using OLS
against other estimators and for hypothesis testing. Note that the
normality assumption is discussed below due to its importance in
hypothesis testing, but is an element of the Classical Linear Model
assumptions rather than the Gauss-Markov assumptions. If the normality
assumption is met, then the CLM assumptions hold and OLS is the best
unbiased estimator—that is, OLS has the lowest variance of all unbiased
estimators, not just linear ones.

-   **(1) Linear in Parameters:**  
    <span
    style="color: red">*y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X* + *u*</span>  
    <span
    style="color: red">*β* = (*X*′*X*)<sup>−1</sup>(*X*′*Y*)</span>

    -   The dependent variable *y* is a linear function of a specific
        set of IVs *X*, an intercept *β*<sub>0</sub> and error term *u*
        which represents factors other than *X* that affect *y*.

    -   Linearity implies that a one-unit change in *x* has the same
        effect on *y*, regardless of the initial value of *x*.

    -   In a linear regression model, the regression model must be
        *linear in parameters*, though it may not be linear in
        variables.

    -   **Correct Specification**: There is no *specification bias* or
        specification error.

    -   Violations:

        -   <span style="color: red">Nonlinearity in Parameters/Wrong
            functional form</span>: Specification Bias

            -   *Consequences*:  
                **Omits the non-linear functional form and includes
                irrelevant linear functional form**. Biased
                coefficients. Difficult to predict whether this biases
                coefficients toward or away from an extreme value, thus
                increasing either the probability of type I or type II
                error.

            -   *Fixes*:  
                **Model transformations:** it is sometimes possible to
                transform a nonlinear function into a linear function
                using transformations such as the logarithmic
                transformation. In these cases, one can induce linearity
                from a seemingly-nonlinear function like the
                Cobb-Douglas prediction function with multiplicative
                error term.  
                **Maximum Likelihood and nonlinear models:** Some
                models, such as the constant elasticity of substitution
                function or Cobb-Douglass production function with
                additive error, are fundamentally nonlinear and *cannot
                be transformed into linear functions*. These cannot be
                accurately modeled using OLS. Accurate estimation
                requires Nonlinear Regression or Maximum Likelihood
                (MLE).

-   **(2) Spherical Error Variance/Disturbances have Uniform Variance
    and are Uncorrelated:**

    -   <span
        style="color: red">*V**a**r*(*u*\|*X*) = *σ*<sup>2</sup>*I*<sub>*n*</sub></span>

    -   **No Autocorrelation Between the Disturbances:** Given any two
        *X* values, *X*<sub>*i*</sub> and *X*<sub>*j*</sub>(*i*≠*j*),
        the correlation between any two *u*<sub>*i*</sub> and
        *u*<sub>*j*</sub> is zero. In short, the observations are
        sampled independently.  
        <span
        style="color: red">*c**o**v*(*u*<sub>*i*</sub>,*u*<sub>*j*</sub>\|*X*<sub>*i*</sub>,*X*<sub>*j*</sub>) = 0</span>

    -   **Homoskedasticity or Constant Variance of *u*<sub>*i*</sub>**:
        The variance of the error, or disturbance, term is the same
        regardless of the value of *X*.  
        <span
        style="color: red">*v**a**r*(*u*<sub>*i*</sub>) = *E*\[*u*<sub>*i*</sub>−*E*(*u*<sub>*i*</sub>\|*X*<sub>*i*</sub>)\]<sup>2</sup></span>  
        which equals
        *E*(*u*<sub>*i*</sub><sup>2</sup>\|*X*<sub>*i*</sub>) because of
        assumption 3, and which equals
        *E*(*u*<sub>*i*</sub><sup>2</sup>), if *X*<sub>*i*</sub> are
        nonstochastic, which equals *σ*<sup>2</sup>

    -   **Violations**:

    -   <span style="color: red">Heteroskedasticity</span>: Inefficiency

        -   *Consequences*:  
            Inefficiency, no longer minimum variance:
            *β*<sup>*O**L**S*</sup> is still linear, unbiased, and
            consistent. But *OLS is neither BLUE nor asymptotically
            efficient among consistent and asymptotically normal
            estimators*. This is because OLS does not make use of the
            information contained in the variability of the DV and
            assigns equal weight to each observation.  
            Bias of *v**a**r*(*β*<sup>*O**L**S*</sup>) means that if
            heteroskdasticity is disregarded in OLS the variance will be
            over or underestimated (depending on relationship between X
            and *σ*<sup>2</sup>), thus whatever conclusions we draw from
            confidence intervals or *t* or *F* tests may be
            misleading.  
            Especially problematic in cross-sectional data due to
            fundamental differences between types in observations (i.e.
            very rich and poor countries in the same dataset)

        -   *Fixes*:  
            **Weighted Least Squares:** special case of GLS for
            heteroskedasticity; solves inefficiency and non-minimum
            variance issues, making WLS BLUE. OLS uses equal weights on
            residual sum of squares whereas WLS uses weighted RSS so
            that obs from populations with larger *σ*<sub>*i*</sub> are
            weighted less than populations with smaller
            *σ*<sub>*i*</sub> Used to adjust for a known form of
            heteroskedasticity, where each squared residual is weighted
            by the inverse of the (estimated) variance of the error. Use
            WLS if the heteroskedastic variances
            *σ*<sub>*i*</sub><sup>2</sup> are known.  
            **White-Robust Standard Error:** Solution for bias of the
            variance, but not efficiency. In practice, the true
            *σ*<sub>*i*</sub><sup>2</sup> are rarely known. RSE gives
            consistent (asymptotically valid) estimates of the variances
            and covariances in the presence of heteroskedasticity.
            Large-sample procedure and estimators less efficient than
            methods that use transformed data.  
            **Transformed Data:** transforming the data (taking squares,
            roots, logs...) if the error variance is proportional to X
            or a function of X can induce homoskedasticity, restoring
            BLUE property to OLS if other assumptions are met.

    -   <span style="color: red">Autocorrelation</span>: Inefficiency

        -   *Test*: Runs test, Breusch-Godfrey Test; *ρ* estimated using
            C-O iterative procedure.

        -   *Consequences*:  
            Inefficiency, no longer minimum variance:
            *β*<sup>*O**L**S*</sup> still linear-unbiased, consistent.  
            OLS assumes the disturbance term relating to any observation
            is not influenced by the disturbance term relating to any
            other observation. If there is dependence, there is
            autocorrelation.  
            This (serial correlation) typically biases OLS estimates of
            the error variance toward zero and understates the standard
            error. Higher risk of type I error, increasing the
            probability that we incorrectly reject the null hypothesis
            (although the variance can also be biased in the opposite
            direction). As a result, the usual *t, F,* and $\\Chi^2$
            tests cannot be legitimately applied.  
            Spatial autocorrelation occurs in cross-sectional data,
            although **serial correlation in time series data** is more
            prevalent, especially if the time between observations is
            short.

        -   *Fixes*:  
            **Correct model specification:** ensure correct functional
            form and no omitted variables as mis-specification can
            appear to be autocorrelation.  
            **Generalized Least Squares (GLS) - Prais-Winsten
            transformation**: Solution to pure autocorrelation depends
            on knowledge about the nature of interdependence among the
            disturbances. If the coefficient of the first-order
            autocorrelation *ρ* is *known*, one can multiply a lagged
            standard OLS equation by *ρ* and subtract this from the
            standard OLS equation, resulting in a generalized difference
            equation and apply OLS to the transformed (now in difference
            form) variables. OLS will now be BLUE.  
            **FGLS**: Solution when *ρ* is *unknown* and must first be
            *estimated*. This is a two-step methods in which the unknown
            *ρ* is estimated and then used to transform the variables to
            estimate the generalized difference equation. Because the
            coefficients are estimated, FGLS will not necessarily be
            BLUE, especially in small samples. These will perform better
            asymptotically, but in small samples one has to be careful
            in interpreting estimated results and OLS might be superior
            if the sample size is small and *ρ* \< 0.3. (Cochrane-Orcutt
            procedure: regress Y on X, generate residuals, regress
            residuals on lagged residuals to produce an estimate of *ρ*,
            transform Y and X using *ρ*, and regress transformed Y\* on
            X\*. Repeat until convergence.)  
            **HAC Standard Errors:** Extension of White’s robust
            standard errors. HAC procedure corrects OLS standard errors
            in presence of *both* heteroskedasticity and
            autocorrelation. As with robust standard errors, this is a
            large-sample procedure and estimators are less efficient
            than those that use transformed data.

-   **(3) Full Rank:**

    -   <span style="color: red">*r**a**n**k*(*X*) = *K* ≥ *N*</span>

    -   **The nature of X variables**: The *X* values in given sample
        must not all be the same (there must be variation in the *X*
        values). Furthermore, there can be no **outliers** in the values
        of the *X* variable.  
        *v**a**r*(*X*) \> 0

    -   **The number of observations *n* must be greater than the number
        of parameters to be estimated:** alternatively, the number of
        observations must be greater than the number of explanatory
        variables.  
        *r**a**n**k*(*X*) = *K* ≥ *N*

    -   **No collinearity or no multicollinearity**: There can be no
        exact collinearity between the *X* variables. None of the
        regressors can be written as an *exact* linear combination of
        the remaining regressors in the model. None of the K columns of
        X can be expressed as a linear combination of the other columns
        of X.

    -   Violations:

    -   <span style="color: red">**Perfect multicollinearity**</span>:
        Indeterminate Regression

        -   *Consequences*:  
            A column of X is linearly dependent on the vectors in other
            columns. OLS will be indeterminate. Because we do not have
            OLS estimates, the bias and efficiency are not well-defined.

        -   *Fixes*:  
            Most likely to occur when one includes a dummy variable for
            every region or for every cross-sectional unit in a fixed
            effects model or when one x is an alternative measure of
            another x (i.e. measuring area in square kilometers and
            square miles, or including regional dummy variables for all
            regions). In either of these cases, one of the variables
            needs to be dropped and this can be done without introducing
            omitted variable bias.

    -   <span style="color: red">**High multicollinearity**</span>: High
        *R*<sup>2</sup> with no/few significant coefficients

        -   *Test*: Variation Inflation Factor

        -   *Consequences*:  
            Not a violation of the assumption, but a practical issue.
            OLS is only relatively efficient compared to other
            estimators, but can exhibit absolute inefficiency due to
            high standard error. Hypothesis testing cannot be conducted
            with perfect collinearity; with high multicollinearity,
            *R*<sup>2</sup> can be very high, but also with high
            p-values for the X variables so that nothing is significant.

        -   *Fixes*:  
            One option is to drop a highly-collinear variable, but this
            may lead to omitted variable bias and model
            misspecification, a far greater sin. Increase observations
            if possible.

    -   <span style="color: red">Insufficient variability in
        regressors</span>: Indeterminate Regression

    -   <span style="color: red">Sample observations less than the
        number of regressors</span>: Indeterminate Regression

-   **(4) Strict Exogeneity: Expected Error is Zero and Strict
    Independence**

    -   <span
        style="color: red">$x_i \\protect\\mathpalette{\\protect\\independenT}{\\perp}u_i$</span>

    -   **Fixed X Values or X Values Independent of the Error Term**:
        Values taken by the regressor *X* may be considered fixed in
        repeated samples (the case of fixed regressor, which rarely
        holds outside of experimental settings) or they may be sampled
        along with the dependent variable *Y* (the case of stochastic
        regressor, which is a weaker but more frequently satisfied
        assumption).

        -   In the latter case, it is assumed that the *X* variable(s)
            and the error term are independent.

        -   The relaxed version, in which
            *c**o**r*(*X*<sub>*i*</sub>,*u*<sub>*i*</sub>) = 0 grants
            only asymptotic unbiasedness and consistency.

        -   *c**o**v*(*X*<sub>*i*</sub>,*u*<sub>*i*</sub>) = 0

        -   Most important assumption, without which *β̂* is biased and
            unreliable.

    -   **Fixed-X Assumption**: X is fixed in repeated samples

        -   from (3) -\> Unconditional exogeneity: *E*(*u*) = 0

        -   from (4) -\> Unconditional spherical error variance:
            *V**a**r*(*u*) = *σ*<sup>2</sup>*I*<sub>*n*</sub>

    -   **Random-sample Assumption**: X is stochastic, sampled along
        with Y

        -   from (3) -\> Weak exogeneity:
            *E*(*u*<sub>*i*</sub>\|*x*<sub>*i*</sub>) = 0 for
            *i* = 1, …, *n*

        -   from (4) -\> Weak non-autocorrelation:
            *E*(*u*<sub>*i*</sub><sup>2</sup>\|*x*<sub>*i*</sub>) = *σ*<sup>2</sup> \> 0
            for *i* = 1, …, *n*

-   **Unconditional Zero Mean**

    -   <span style="color: red">*E*(*u*) = 0</span>

    -   The expected value of the disturbance term is zero.

    -   As long as the intercept *β*<sub>0</sub> is included in the
        equation, nothing is lost by assuming that the average value of
        *u* in the population is zero, because *we can always redefine
        the intercept to make *E*(*u*) = 0*. As a result, this is a
        relatively trivial assumption.

    -   (Regression through the origin should only be used with caution
        if there are strong theoretical reasons for doing so. In these
        models the sum of the residuals is non-zero, potentially
        rendering the *R*<sup>2</sup> meaningless.)

-   **Strict Exogeneity**

    -   <span style="color: red">*E*(*u*\|*X*) = *E*(*u*)</span>

    -   The more crucial assumption is that the average value of *u*
        does not depend on the value of *x*.

    -   The average value of the unobservables is the same across all
        slices of the population determined by the value *x* and that
        the common average is necessarily equal to the average of *u*
        over the entire population.

    -   When this assumption is met, *u* is *mean independent* of *x*.

-   **Zero Conditional Mean**

    -   <span style="color: red">*E*(*u*\|*X*) = 0</span>

    -   If we combine the *unconditional zero mean* <span
        style="color: red">*E*(*u*) = 0</span> and *strict exogeneity*
        <span style="color: red">*E*(*u*\|*X*) = *E*(*u*)</span>
        assumptions, we obtain the *zero conditional mean assumption*,
        <span style="color: red">*E*(*u*\|*X*) = 0</span>.

    -   Given the value of *X*, the mean, or expected, value of the
        random disturbance term *u* is zero.

-   **Violations:**

-   <span style="color: red">Nonzero mean of *u*</span>: Biased
    Intercept

    -   *Consequences*: The disturbance may have a non-zero mean because
        of systematically positive or negative errors of measurement in
        calculating the dependent variable. OLS forces the error term
        into zero mean, mimicking the assumption, so its violation is
        non-obvious. If violated, only intercept will be biased.

    -   *Fixes*: The biased intercept is often welcomed, since for
        prediction purposes we would want to incorporate the mean of the
        error term into the prediction. Nevertheless, *be skeptical
        about intercept accuracy*. No bias is created by an unnecessary
        intercept, and the intercept can alleviate bias if a relevant
        explanatory variable is omitted.

-   <span style="color: red">Simultaneity</span>: Biased and
    inconsistent

    -   *Test*: Hausman Specification Test

    -   *Consequences*: In the presence of endogenous variables, the
        regressor will be correlated with the disturbance term. As a
        result, the OLS estimator will be not only biased but also
        inconsistent: even given an infinite sample, OLS estimators will
        never converge to the true population values. Bias and
        inconsistency also mean that efficiency comparisons are wrong.
        So hypothesis tests and inferences will be incorrect as well.

    -   *Fixes*: **Simultaneous equation models** jointly determine two
        or more endogenous variables, where each endogenous variable can
        be a function of other endogenous variables as well as of
        exogenous variables and an error term. **2SLS** uses an
        instrumental variable in a first stage equation that predicts
        and endogenous Y but is uncorrelated with the error term. If the
        correlation between the instrument and the endogenous X variable
        is sufficiently high, the instrument is strong and can be used
        to estimate the causal effect of X on Y while side-stepping
        endogeneity. The estimates obtained from well-specified 2SLS
        models will be consistent, but may not satisfy small sample
        properties such as unbiasedness and minimum variance, so use
        caution in small sample inference.

-   <span style="color: red">Errors in Variables</span>: Biased and
    inconsistent

    -   **Classic errors in variables assumption** is that the
        measurement error *e* is uncorrelated with the *unobserved*
        explanatory variable:
        *c**o**v*(*x*<sub>1</sub><sup>\*</sup>,*e*<sub>*i*</sub>) = 0.
        The observed measure is the sum of the true explanatory variable
        and measurement error:
        *x* = *x*<sub>1</sub><sup>\*</sup> + *e*<sub>*i*</sub>. This
        implies that
        *c**o**v*(*x*<sub>1</sub>,*e*<sub>1</sub>) = *E*(*x*<sub>1</sub>+*e*<sub>1</sub>) = *E*(*x*<sub>1</sub><sup>\*</sup>+*e*<sub>1</sub>) + *E*(*e*<sub>1</sub><sup>2</sup>) = 0 + *σ*<sub>*e*</sub><sup>2</sup> = *σ*<sub>*e*</sub><sup>2</sup>,
        therefore the covariance is equal to the variance of the
        measurement error. *Because the measurement error appears in
        both the incorrectly measured dependent variable and the
        disturbance term, the estimating equation has a u that is
        contemporaneously correlated with an x, and as a result OLS will
        be biased and inconsistent.*

    -   *Consequences*:  
        **Measurement errors of y:** less precise but unbiased estimate
        of *β*<sub>1</sub><sup>*O**L**S*</sup>. Where *ỹ* = *y* + *u*,
        substituting this into the OLS yields
        *ỹ* = *α* + *β**X* + *ϵ* + *u*.  
        **Measurement errors of x in a simple linear regression model**:
        OLS regression of y on x gives a biased and inconsistent
        estimator. The direction of the bias depends on the correlation
        between the error and the regressor: Positive measurement error
        correlation leads to a downward coeffcient estimate. Negative
        measurement error leads to upwardly biased coeffcients. Even if
        the measurement error in the explanatory variable has mean zero,
        is uncorrelated with the true dependent and independent
        variables and with the equation error, *the measurement error
        becomes part of the error term in the regression equation thus
        creating endogeneity bias*.  
        (1) We want to estimate a model: *y* = *β**X* + *ϵ*  
        (2) But we only have data for x with measurement error:
        *x̃* = *x* + *u*  
        Substituting (2) into (1):
        $y=\\beta(\\tilde{x}-u)+\\epsilon=y_i=\\textcolor{red}{\\beta \\tilde{x}+(\\epsilon-\\beta u)}$  
        **Measurement errors of x in a multiple regression model**: Bias
        depends on correlation between accurately-measured and
        ill-measured x variables and can be positive or negative. In the
        special case that the x with measurement error is uncorrelated
        with the other x variables, the parameters for the remaining
        variables will remain consistent. Generally, measurement error
        in a single variable causes inconsistency in all estimators. The
        sizes and directions of the biases are not easily derived.

    -   *Fixes*:  
        **Measurement error in y**: measurement error is accounted for
        in the disturbance term of the regression model. Measure it as
        well as possible and use as close of proxies as possible if
        necessary.  
        **Measurement error in x**: Get better data or use an
        instrumental variable model (2SLS), where the instrument *z* and
        its measurement error *e*<sub>*z*</sub> must be uncorrelated
        with the error term *u* and also the measurement error for x
        *e*<sub>*x*</sub>. The instrument *z* may then be used as an
        instrument for *x̃* to get consistent estimates.

-   <span style="color: red">Wrong Regressors</span>: Biased and
    inconsistent

    -   *Consequences*:  
        **Omission of a relevant independent variable (underfitting)**:
        Biased coefficients; for hypothesis testing, higher type I or II
        error depending on direction of bias.  
        **Inclusion of an irrelevant independent variable
        (overfitting)**: OLS estimator remains unbiased and consistent,
        but the parameters estimated by the model will have higher
        variances and be less efficient.

    -   *Fixes*:  
        **Omitted Variable Bias:** Include theoretically-relevant
        variables or suitable proxies whenever possible. Use fixed
        effects or first differencing to mitigate time-constant omitted
        variables. Use instrumental variable models for time-varying
        omitted variables that are correlated with the explanatory
        variables. **Irrelevant Variables:** Don’t garbage can
        regression.

**(CLM 5) Normality of Disturbance Term**

-   Note we cannot make an inferences or probability statements under
    the Gauss-Markov Theorem assumptions, because the GMT says nothing
    about the probability distributions of anything. This is where the
    addition of an assumption about normality of the disturbance term
    becomes useful.

-   If errors are not normally distributed but the Gauss-Markov
    assumptions are met, the OLS estimators will be BLUE.

-   In order to perform statistical inference, we need to know the full
    sampling distribution of the *β̂*. Even under the Gauss-Markov
    assumptions, the distribution of *β̂* can have virtually any shape.

-   To make the sampling distributions of the *β̂* tractable, we assume
    that the unobserved error is *normally distributed* in the
    population.  
    <span style="color: red">(*u*\|*X*)∼ *N*(*μ*,*Σ*)</span>, where
    *μ* = 0 and *Σ* = *σ*<sup>2</sup>

-   The argument for assuming normality of the disturbances is that,
    because *u* is the sum of many different unobserved factors
    affecting y, we can invoke the central limit theorem to conclude
    that *u* has an approximate normal distribution as the sample size
    goes to infinity. This is, however, an empirical matter that can be
    tested, so don’t just assume normality.

-   *The argument for asymptotic normality is not necessarily true! It
    is extremely convenient to assume normality, but there exists little
    justification for this assumption. The distribution of errors may
    not be asymptotically normal. Several tests for normality exist, and
    the consequences of non-normality can be serious, since hypothesis
    testing and interval estimation cannot be undertaken meaningfully.
    Faced with non-normality, two options: normality may be approximated
    using transformations of the data, or we can use robust estimators.*

-   *Under normality,
    $\\hat{\\beta}\_1, \\hat{\\beta}\_2, \\dots, \\hat{\\beta_n}$ are
    distributed independently of *σ̂*<sup>2</sup> and are BUE (have
    minimum variance in the entire class of unbiased estimators, whether
    linear or not.)*

-   What the normality assumption gets us for hypothesis testing:

    -   (*n*−2)(*σ̂*<sup>2</sup>/*σ*<sup>2</sup>) is distributed as the
        *χ*<sup>2</sup> distribution, with (*n*−2)*d**f*. Allows us to
        draw inferences about the true *σ*<sup>2</sup> from the
        estimated.

    -   $\\hat{\\beta_1}$ and $\\hat{\\beta_2}$ are distributed
        independently of *σ̂*<sup>2</sup>

    -   The t statistics have t distributions under the null hypothesis.

    -   We use t statistics to test hypotheses about a single parameter
        against one- or two-sided alternatives, using one- or two-tailed
        tests, respectively. The most common null hypothesis is H0:
        *β*<sub>*j*</sub> = 0, but we sometimes want to test other
        values of *β*<sub>*j*</sub> under H0.

    -   Confidence intervals can be constructed for each
        *β*<sub>*j*</sub>. These CIs can be used to test any null
        hypothesis concerning *β*<sub>*j*</sub> against a two-sided
        alternative.

-   **Violations, Consequences, and Fixes:**

    -   <span style="color: red">Non-normality of Disturbances</span>:
        If violated, OLS will still be BLUE. If holds, OLS is BUE. If
        the errors
        *u*<sub>1</sub>, *u*<sub>2</sub>, …, *u*<sub>*n*</sub> are
        random draws from some distribution other than the normal, the
        *β*<sub>*j*</sub> j will not be normally distributed, which
        means that the t statistics will not have t distributions and
        the F statistics will not have F distributions. This is a
        potentially serious problem because our inference hinges on
        being able to obtain critical values or p-values from the t or F
        distributions. Non-normality can sometimes be fixed by
        increasing sample size (CLT). If increasing the sample size does
        not result in normality, then sometimes variable transformations
        can generate normality. Otherwise, use robust estimators.

# Previous Comp Questions Organized by Topic

## Sampling Distributions

-   The normal distribution is commonly seen as especially central to
    statistical modeling and analysis. Why and how is that? What are its
    properties and its relations to other common distributions? (Fall
    2013)

-   What is a sampling distribution? Describe the sampling distributions
    of the two following estimators: (1) the mean of N independent draws
    from a normal distribution and (2) the sample proportion of N draws
    (where N is large) from a population with some proportion (p) of 1’s
    and (1-p) of 0’s (assume the population is extremely large and can
    be treated as infinite; use asymptotic approximations for the
    distribution of the estimator as appropriate, justifying your
    decisions). Discuss what you view as the most important properties
    in general that the sampling distribution of an estimator can have.
    Discuss how the sampling distribution of an estimator relates to
    hypothesis testing? (Spring 2015)

-   What is the sampling distribution of an estimator? How does it play
    a role in inference and hypothesis testing? Define and briefly
    discuss three properties an estimator can have, being sure to focus
    on how each relates to the sampling distribution. (Fall 2016, Fall
    2017)

**Gauss-Markov and Estimator Properties**

-   For each statement, indicate whether it is true or false and briefly
    justify your answer. (Note: each letter part should be considered
    separately) (Spring 2019)

    1.  Consider *θ̂* and *θ̃* to be unbiased estimators of population
        parameter *θ*. If these estimators are applied to the same
        sample, they should generate the same estimate.

    2.  An unbiased estimator is one that closely approximates the
        parameter.

    3.  If *X*<sub>1</sub>, *X*<sub>2</sub>, …, *X*<sub>*n*</sub> is a
        random sample from a population with *E*\[*X*\] = *μ*, then
        *Σ*<sub>*i* = 1</sub><sup>*n*</sup>(*X*<sub>*i*</sub>−*μ*) = 0.

    4.  In random sampling from a population whose expectation is
        *E*\[*Y*\] = *μ*, the expression
        *Σ*<sub>*i* = 1</sub><sup>*n*</sup>(*Y*<sub>*i*</sub>−*Ȳ*)<sup>2</sup>
        is greater than or equal to the expression
        *Σ*<sub>*i* = 1</sub><sup>*n*</sup>(*Y*<sub>*i*</sub>−*μ*)<sup>2</sup>,
        because the sample mean *Ȳ* is only an estimate of the
        population mean *μ*.

    5.  If, instead of a sample, we are able to collect a full census of
        the data of interest then there is no uncertainty in our
        estimates; the empirical distribution is the population
        distribution.

-   What are the classical assumptions accompanying OLS estimation of a
    linear additive regression model? Consider each in isolation. What
    does each get us—i.e., what would be the cost of its failing? Which,
    if any, are equally necessary for any estimator of his model, not
    just OLS? When is each likeliest to be violated? What, in brief, can
    be done about each? (Spring 2017)

-   What is the Gauss-Markov Theorem? Define each and every
    statistically relevant term in the statement of the theorem. Discuss
    the assumptions of the theorem. Be specific about the critical role
    each assumption plays in the conclusion of the theorem as well as
    what can be done to preserve the conclusion if each assumption is
    violated. (Fall 2017)

-   State the Gauss-Markov Theorem. Explain in detail consequences of
    individual violations of each of its assumptions for (i) inference
    and (ii) hypothesis testing. (Fall 2015)

-   How do we conduct estimation and hypothesis testing in the standard
    (frequentist) statistical approach? Name three properties that make
    a good estimator, defining each and giving an example of an
    estimator that has the property. Give an example of a situation
    where we may choose to use an estimator that does not have one of
    the properties you listed and explain why such an estimator may be
    desirable. Explain the steps of testing a hypothesis about the value
    of an unknown parameter. Your answer should include definitions and
    discussions of the sampling distribution and p-value. (Fall 2014)

-   What are the principal desirable statistical properties claimed by
    commonly used estimators? Why are they desirable? Be sure to
    distinguish between finite-sample and asymptotic properties. What
    are the relationships between the properties? Are some more
    fundamental than others? More desirable than others? Describe the
    properties that at least three formally distinct estimators can
    claim under their respective classical assumptions. (Fall 2013)

## Assumptions’ Violations and How to Address Them

-   Define the linearity assumption of the classical linear regression
    model (CLRM). Provide an example of a model that meets the
    requirements of the linearity assumption and one that does not,
    explaining the difference between the two. What are the consequences
    of violating the linearity assumption? How is the linearity
    assumption not as strict as it might seem? (Note: this question asks
    about linearity assumption related to the functional form of the
    CLRM, not the linearity of the typical estimator used to estimate
    its parameters.) (Spring 2019)

-   Two of the primary assumptions of the standard linear regression
    model involve linearity and additivity. Explain how each of these
    two things plays an important role in regression. Under what
    circumstances might non-linearity or non-additivity arise and how
    can the linear regression model accommodate these issues, if at all?
    (Fall 2018)

-   Define perfect collinearity and imperfect but problematic
    collinearity in the context of linear regression models, in both
    sample and population. What can cause them? What are their effects?
    What if anything can be done about them? (Spring 2019)

-   What is multicollinearity? What are the statistical implications of
    multicollinearity in a linear regression model? List three possible
    ways you might handle multicollinearity and the conditions under
    which each method would be most appropriate. (Spring 2018)

-   Imagine a linear regression model with some dependent variable Y
    predicted by one independent variable X, with standard setup and
    assumptions including an estimated slope and intercept, independent
    normal homoscedastic errors, etc. How would your estimates be
    affected by each of the following situations? (Treat each one
    separately.): (Spring 2018)

    1.  Your dependent variable is measured with error. You can assume
        this is “white noise”error, i.e., observed Y equals the true Y
        plus some iid normal noise independent of both X and the model’s
        error term.

    2.  Your independent variable is measured with error. You can assume
        this is “white noise” error, i.e., observed X equals the true
        Xplus some iid normal noise independent of both the true X and
        the model’s error term.

    3.  X is measured with error as in (2) above but there also is
        another independent variable (call it Z) that is measured
        without error included as a predictor in addition to (noisy) X.

-   What is the “non-spherical disturbances” problem in regression
    analysis? Describe the problem and explain how it can be corrected
    in mathematical terms. (Spring 2017)

-   Assume you have estimated a standard linear regression via OLS
    predicting y with several x variables (x1, x2, etc). For each of the
    following possible issues, describe the impact on your inferences
    and what can be done (if anything) to correct the problem(s): (a)
    you have left out some predictor (call it z) that has an effect on
    y; (b) the errors are not normally distributed; and (c) the errors
    do not have the same variance across observations.

    Imagine that you believe the true data generating process for some
    dependent variable of interest is of the form y=b0+b1\*x1 + b2\*x2
    +e where under this true model, the standard linear model
    assumptions are thought to hold. Under each of the following three
    estimation situations, describe: (a) any potential problems with
    standard estimates of the coefficients and hypothesis tests
    involving them including when these problems will occur and how
    severe they may be; (b) what (if any) measures can be taken to
    address these issues.

    In empirical social science research, we rarely have measures of all
    of the things that could conceivably affect our dependent variable.
    Therefore, we make do with simplified models, often acknowledging
    that they are imperfect and may ignore one or more explanatory
    variables. What are the consequences of omitting an independent
    variable from a linear regression model? Illustrate your arguments
    with an example, in which the “true” model includes two predictors
    X1 and X2, but in which you estimate a model including only X1,
    leaving X2 out of your analysis. Under what circumstances will this
    produce problematic results? Under what circumstances will the
    estimates in your fitted model still be useful and informative? In
    an experiment (or natural experiment) where X1 is randomly (or as-if
    randomly) assigned, how would your answer change? (Spring 2017)

## Hypothesis Testing and P-Value

-   Define statistical significance (in its standard frequentist form).
    Define substantive significance. Discuss the differences between
    these two concepts. Give an example (real or hypothetical) of
    statistical significance without substantive significance. Give an
    example (real or hypothetical) of substantive significance without
    statistical significance. (Spring 2018)

-   In recent years, a large amount of attention has been paid in the
    social sciences to problems with the “standard” approach to null
    hypothesis significance testing (NHST). Several critiques have been
    raised, including the possibility that scholars may try a large
    number of model specifications, including interactions or subgroup
    analyses, but report only a subset of these. Scholars may even come
    up with post-hoc theories after seeing that they obtain
    statistically significant results for a particular group or in a
    particular situation, presenting these theories as if they were
    arrived at before data were analyzed. Explain the problems that can
    result from the type of researcher behavior described above. What,
    in your view, is the best response (or set of responses) to these
    issues? (Fall 2018)

-   In 2016, the American Statistical Association (ASA) issued a
    statement on p-values entitled “The ASA’s Statement on p-Values:
    Contexts, Process, and Purpose.” The statement lists the following
    six “principles”: (…) Do you agree or disagree with these
    “principles”? Explain. (Fall, 2017)

-   Recently, there have been several prominent critiques raised about
    the use of null hypothesis significance testing and p values in
    applied research. Describe the basic framework of hypothesis
    testing, being sure to carefully define null and alternative
    hypotheses and p values. What does a p value alone tell you about
    the size of an effect? If researchers try out multiple models (or
    multiple hypotheses altogether) and publish only so-called
    “significant findings,” is this problematic? In what ways? (Spring
    2017)

-   Discuss the general procedure for testing hypotheses in the standard
    (frequentist) framework. Comment on the difference between
    substantive and statistical significance, giving at least one
    example, which can be made up or based on actual research. How
    should researchers think about testing multiple hypotheses? For
    example, if a researcher tests a large number of separate hypotheses
    and rejects only a few, should she conclude that those few
    hypotheses are in fact false with a high degree of confidence?
    (Spring 2016)

## Interaction Term

-   Assume you have estimated the following linear regression model in
    which Y and X1 are continuous while X2 is binary (0 or 1):
    *Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*X*<sub>2</sub> + *β*<sub>3</sub>*X*<sub>1</sub>*X*<sub>2</sub> + *ϵ*
    where all the standard linear regression model assumptions hold.
    (Spring 2018)

    1.  How would you describe the relationship between X1 and y?

    2.  If you can reject the null hypothesis that *β*<sub>1</sub>
        equals zero, what does this tell you?

    3.  If you can reject the null hypothesis that *β*<sub>2</sub>
        equals zero, what does this tell you?

    4.  If you can reject the null hypothesis that *β*<sub>3</sub>
        equals zero, what does this tell you?

    5.  If you cannot reject the null hypothesis that *β*<sub>2</sub>
        equals zero, can X2be excluded from the model? Why or why not?
        (Be specific about the implications of your choice.)

    6.  How do your answers to parts (a) through (d) above change if
        *X*<sub>2</sub> is continuous instead of binary?

-   Consider a linear regression model of the form:
    (*Y* = *β*<sub>0</sub> + *β*<sub>1</sub>*X*<sub>1</sub> + *β*<sub>2</sub>*Z*<sub>*i*</sub> + *β*<sub>3</sub>*X*<sub>1</sub>*Z*<sub>*i*</sub> + *ϵ*),
    where *ϵ*<sub>*i*</sub> is independent normal with mean zero and
    variance *σ*<sup>2</sup>. Discuss the interpretation of each of the
    estimated coefficients including the intercept. How would one test
    whether the effect of x on y depends on the level of z? What would
    it mean to leave out z (or x) from this model but leave in the
    intercept and the x \* z term? Is this generally a good idea?
    (Spring 2016)

-   Interaction terms allow for useful elaboration of regression models
    in many situations. Describe in the basic linear regression model
    how interaction terms work and how they should be interpreted,
    writing out the standard formulation of a regression specification
    with two predictors and an interaction term between them. What is
    the meaning of so-called “main effect” coefficients and of
    “interaction term” coefficient in this model? What part(s) of the
    regression output would one look at to assess whether there exists
    an interactive relationship? Give an example of a theory or
    hypothesis in which an interaction term would be appropriate and
    describe how one would interpret the estimated coefficients from a
    model using appropriate data. (Fall 2015)

## Methods of Estimation (OLS, GLS, MLE)

-   What is generalized least squares (GLS)? To what sorts of models is
    it appropriate? How in each of at least two models of your choice,
    would you implement it? (Be specific.) Why, for these models, is GLS
    superior in principle to OLS? Why might it not always be superior in
    practice? (Fall 2014-Fall 2017)

-   What is weighted least squares (WLS) When would WLS be preferable to
    OLS when estimating a regression model? What are the drawbacks to
    using WLS? When might OLS be preferable? Are there any alternatives
    to WLS that seek to address similar issues? (Fall 2018)

-   In statistics, what is a model, what is a method, and what are their
    roles in statistical inference? Discuss at least two methods and
    apply them to a model in your discussion. (Spring 2015)

-   Describe and compare least squares and maximum likelihood
    estimation. What is the general principle of each? What statistical
    properties can each generally claim, under classical assumptions?
    What are those assumptions? Name and describe some varieties of each
    (think of prefatory adjectives like “ordinary" for least squares),
    noting the sort(s) of model(s) for which each is appropriate. Take a
    model that could reasonably be estimated by one variety of least
    squares and by at least one variety of maximum likelihood. What
    issues are involved in choosing between them? (Fall 2013)

# Study Guide to Previous Comp Questions

**Sampling Distributions**

-   What is a sampling distribution?

-   What role does the sampling distribution play in inference and
    hypothesis testing?

-   Define and discuss three properties an estimator can have, focusing
    on how each relates to the sampling distribution.

-   What are the most important properties in general that the sampling
    distribution of an estimator can have?

-   What is the normal distribution? Why is it important? What are its
    properties compared to other common distributions?

    -   Why is it important?

    -   What are its properties compared to other common distributions?

    -   Describe the sampling distributions of (1) the mean of N
        independent draws from a normal distribution and (2) the sample
        proportion of N draws (where N is large) from a population with
        some proportion (p) of 1’s and (1-p) of 0’s. Assume the
        populaiton is extremely large and can be treated as infinite.

**Gauss-Markov Theorem, Estimator Properties, Assumptions, Violations,
and Remedies**

-   State the Gauss-Markov Theorem and define each term used.

-   Discuss each of the assumptions of the Gauss-Markov Theorem.

-   For each assumption, discuss common violations and the consequences
    of the violation for inference and for hypothesis testing.

-   For each violation, discuss potential remedies, if any exist, and
    when each would be preferable to OLS.

<!-- -->

-   State the Gauss-Markov Theorem and define each term used.

-   Discuss each of the assumptions of the Gauss-Markov Theorem.

-   For each assumption, discuss common violations and the consequences
    of the violation for inference and for hypothesis testing.

-   For each violation, discuss potential remedies, if any exist, and
    when each would be preferable to OLS.

**Hypothesis Testing and P-Value**

-   Define statistical significance in the standard (frequentist) form.

-   Define substantive significance.

-   Give an example of statistical significance without substantive
    significance.

-   Give an example of substantive significance without statistical
    significance.

-   Explain the problems with only publishing significant results and of
    generating post-hoc theories after trying many models (including
    subgroup analyses) and only reporting those with statistically
    significant results. What is the best response or set of responses
    to these issues?

-   What does a p-value alone tell you about the size of an effect?

-   How should researchers think about testing multiple hypotheses? (For
    example, if a researcher tests a large number of separate hypotheses
    and rejects only a few, should she conclude that those few
    hypotheses are in fact false with a high degree of confidence?)

**Interaction Term**

-   Discuss the interpretation of each of the estimated coefficients
    including the intercept.

-   Discuss the rejection of the null hypothesis for each of the
    coefficients.

-   Discuss the implications of dropping one of the variables from the
    model, but keeping the interaction in the model.

-   Discuss the implications of dropping the interaction from the model.

**Methods of Estimation (OLS, GLS, MLE, 2SLS)**

-   What is a model, and what is a method?

-   Describe OLS, GLS (including fGLS and WLS), MLE, and 2SLS. For which
    models is each appropriate and how do you choose between them?

# Answers to Past Comp Questions

## GLS, WLS Questions

*What is generalized least squares (GLS)? To what sorts of models is it
appropriate? How in each of at least two models of your choice, would
you implement it? (Be specific.) Why, for these models, is GLS superior
in principle to OLS? Why might it not always be superior in practice?
AND What is weighted least squares (WLS)? When would WLS be preferable
to OLS when estimating a regression model? What are the drawbacks to
using WLS? When might OLS be preferable? Are there any alternatives to
WLS that seek to address similar issues?*

The Gauss-Markov theorem (GMT) defines the finite-sample properties of
the ordinary least squares (OLS) in the classical linear regression
model (CLRM). The GMT states that the OLS estimator will be the best
linear unbiased estimator (BLUE) if a set of assumptions are met. "Best"
means that OLS will be the most efficient (have the lowest variance)
among all unbiased linear estimators, and unbiasedness means that in
expectations the parameters estimated by OLS will be equal to the
population parameters. This requires four assumptions to be met:

1.  Linearity in Parameters \[*Y* = *α* + *X**β* + *ϵ* and
    *β̂*<sub>*O**L**S*</sub> = (*X*′*X*)<sup>−1</sup>*X*′*Y*\]

2.  Full Rank \[*R**a**n**k*(*X*) = *K*\]

3.  Strict Exogeneity
    \[$X\\protect\\mathpalette{\\protect\\independenT}{\\perp}Y$\]

4.  Spherical Error Variance \[*E*(*ϵ*) = 0,
    *V**a**r*(*ϵ*) = *σ*<sub>*ϵ*</sub><sup>2</sup>,
    *C**o**v*(*ϵ*<sub>*i*</sub>,*ϵ*<sub>*j*</sub>) = 0\]

Assuming the first three assumptions are met, OLS will be an unbiased
linear estimator. If the fourth assumption is also met, then OLS will be
the BLUE.

If the fourth assumption is violated, then OLS will no longer be BLUE
because spherical error variance is required for efficiency. If the
spherical error variance assumption is violated, then a generalized
least squares estimator will be the BLUE. This is because GLS uses
information about error variance to transform the equations, restoring
constant error variance and allowing OLS to be used on the transformed
equations which will then be the BLUE. (Note that for the duration of
this answer, I assume that assumptions 1-3 are met and focus on specific
violations and fixes of the spherical error variance assumption.) The
spherical error variance assumption is violated in the presence of
heteroskedasticity or autocorrelation. Both of these problems are
common, so it is important to correct for these patterns in the
residuals.

Heteroskedasticity occurs when there is uneven variance in the
observations at different levels of the X variables. For example, if we
look at the relationship between income (X) and savings (Y), then we
will see that the error variance at low levels of X is relatively small.
This is because people with low income have less expendible income and
thus less flexibility to choose how to spend or save their money. Due to
a high ratio of minimum living expenses to income, only a small
percentage of a low-income individual’s income can be saved, so their
savings is generally low. This is not true of high-income earners. At
high income levels, there is greater flexibility in how an individual
spends his money. A high-income person must spend a relatively small
percentage of his income in order to pay for basic needs. This leaves a
large amount of discretionary income, which can either be saved or
spent. Individuals with higher incomes will thereby have a much larger
variance in savings. This pattern will cause heteroskedasticity in the
error variance. The benefit of GLS techniques is that they can take into
account information about the error variance and use it to transform a
regression to introduce constant error variances. For
heteroskedasticity, a specific variant of GLS is particularly useful:
weighted least squares (WLS).

They key difference between OLS and WLS, as the name suggests, is how
the estimator weights the residual sum of squares. WLS minimizes a
weighted residual sum of squares
\[*Σ**w*<sub>*i*</sub>*û*<sub>*i*</sub><sup>2</sup> = *Σ**w*<sub>*i*</sub>(*Y*−*β̂*<sub>1</sub><sup>\*</sup>−*β̂*<sub>2</sub><sup>\*</sup>*X*<sub>*i*</sub>)<sup>2</sup>,
where $w_i=\\frac{1}{\\sigma^2_i}\]$, while OLS minimizes an unweighted
residual sum of squares
\[*Σ**û*<sub>*i*</sub><sup>2</sup>=*Σ*(*Y*−*β̂*<sub>1</sub>−*β̂*<sub>2</sub>*X*<sub>*i*</sub>)<sup>2</sup>\].
In order to use WLS, we must know the heteroskedastic variances,
*σ*<sub>*i*</sub><sup>2</sup>. If we know this, we can then take the
linear regression model
\[*Y*<sub>*i*</sub>=*β*<sub>0</sub>+*β*<sub>1</sub>*X*<sub>*i*</sub>+*u*<sub>*i*</sub>\]
which is mathematically equivalent to
\[*Y*<sub>*i*</sub> = *β*<sub>0</sub>*X*<sub>0*i*</sub> + *β*<sub>1</sub>*X*<sub>*i*</sub> + *u*<sub>*i*</sub>
where *X*<sub>0*i*</sub> = 1∀*i*\], and divide both sides of
\[*Y*<sub>*i*</sub>=*β*<sub>0</sub>*X*<sub>0*i*</sub>+*β*<sub>1</sub>*X*<sub>*i*</sub>+*u*<sub>*i*</sub>\]
by *σ*<sub>*i*</sub>, yielding
$\[\\frac{Y_i}{\\sigma_i}=\\beta_0 \\frac{X\_{0i}}{\\sigma_i}+\\beta_1 \\frac{X_i}{\\sigma_i}+\\frac{u_i}{\\sigma_i}\]$.
Rewriting this as transformed variables for simplicity yields
\[*Y*<sub>*i*</sub><sup>\*</sup>=*β*<sub>0</sub><sup>\*</sup>*X*<sub>0*i*</sub><sup>\*</sup>+*β*<sub>1</sub>*X*<sub>*i*</sub><sup>\*</sup>+*u*<sub>*i*</sub><sup>\*</sup>\].
By weighting the error term by the known *σ*<sub>*i*</sub><sup>2</sup>,
this transformation has altered the non-spherical error variance in
\[*Y*<sub>*i*</sub>=*β*<sub>0</sub>+*β*<sub>1</sub>*X*<sub>*i*</sub>+*u*<sub>*i*</sub>\]
into a constant error variance, as shown below:  
$Var(u_i^\*)=E(u_i^\*)^2=E(\\frac{u_i}{\\sigma_i})^2$  
$=(\\frac{1}{\\sigma^2_i})E(u_i^2)$ since *σ*<sub>*i*</sub><sup>2</sup>
is known,  
$=(\\frac{1}{\\sigma^2_i})(\\sigma_i^2)$ since
*E*(*u*<sub>*i*</sub><sup>2</sup>) = *σ*<sub>*i*</sub><sup>2</sup>  
 = 1  
Thus, the transformed equation
\[*Y*<sub>*i*</sub><sup>\*</sup>=*β*<sub>0</sub><sup>\*</sup>*X*<sub>0*i*</sub><sup>\*</sup>+*β*<sub>1</sub>*X*<sub>*i*</sub><sup>\*</sup>+*u*<sub>*i*</sub><sup>\*</sup>\]
meets the GMT assumptions, and the WLS will provide efficient estimates.
WLS is able to improve on the efficiency of OLS because it assigns a
weight $\\frac{1}{\\sigma^2_i}$ to each observation, weighting
observations from populations with high *σ*<sub>*i*</sub><sup>2</sup>
less and observations with low *σ*<sub>*i*</sub><sup>2</sup> more. This
keeps populations with higher variance from dominating the WLS estimates
in the same way that they would an OLS estimate. Using OLS instead of
WLS will result hypothesis testing that has an increased probability of
type II error because of the overly large variances.

If *σ*<sub>*i*</sub><sup>2</sup> is unknown, as is often the case, one
option is to transform the variables in the OLS by using square root,
square, or logarithmic transformations of the data in an attempt to
decrease the weight of outliers and other observations with high
variance. This may limit the difference in variance at various levels of
X, greatly reducing the problem of heteroskedasticity and limiting the
inefficiency of the OLS estimator. Another option is to use White’s
robust standard errors, which do not eliminate the problem of
inefficiency, but result in unbiased estimates of the variance, which
will improve the performance of OLS in inference.

Autocorrelation occurs when there is interdependence among the
disturbances, and can be spatial or temporal in nature. Serial
correlation in time series data is especially common, and most typically
occurs when observations are collected frequently due to patterns of
cyclicality or trends. Similarly, spatial autocorrelation can occur due
to diffusion between neighboring units. In the presence of
autocorrelation, if we know the coefficient of first-order
autocorrelation (*ρ*), then we can use GLS which will be the BLUE.
Assume we have a two-variable regression model
\[*Y*<sub>*t*</sub>=*β*<sub>1</sub>+*β*<sub>2</sub>*X*<sub>*t*</sub>+*u*<sub>*t*</sub>\]
with first-order autocorrelation
\[*u*<sub>*t*</sub>=*ρ**u*<sub>*t* − 1</sub>+*ϵ*<sub>*t*</sub>,−1,*ρ*\<1\]
and that we know the coefficient of first-order autocorrelation, *ρ*. If
we take the lagged model
\[*Y*<sub>*t* − 1</sub>=*β*<sub>1</sub>+*β*<sub>2</sub>*X*<sub>*t* − 1</sub>+*u*<sub>*t* − 1</sub>\]
and multiply both sides by the known *ρ*
\[*ρ**Y*<sub>*t* − 1</sub>=*ρ**β*<sub>1</sub>+*ρ**β*<sub>2</sub>*X*<sub>*t* − 1</sub>+*ρ**u*<sub>*t* − 1</sub>\],
then we can subtract this equation from the regression model
\[*Y*<sub>*t*</sub> − *ρ**Y*<sub>*t* − 1</sub> = *β*<sub>1</sub>(1−*ρ*) + *β*<sub>2</sub>(*X*<sub>*t*</sub>−*ρ**X*<sub>*t* − 1</sub>) + *ϵ*<sub>*t*</sub>,
where *ϵ*<sub>*t*</sub> = *u*<sub>*t*</sub> − *ρ**u*<sub>*t* − 1</sub>\]
yielding a transformed model
\[*Y*<sub>*t*</sub><sup>\*</sup>=*β*<sub>1</sub><sup>\*</sup>+*β*<sub>2</sub><sup>\*</sup>*X*<sub>*t*</sub><sup>\*</sup>=*ϵ*<sub>*t*</sub>\].
The error term in the last two equations now satisfies the usual OLS
assumptions. Thus, we can use GLS and it will be the BLUE.

The previous example assumes that rho is known. If rho is unknown, which
is common, then we can use feasible generalized least squares (FGLS) to
estimate the rho. Because FGLS is using an estimate of rho rather than
the true rho, the resulting estimator will be asymptotically efficient
and consistent, but may not be BLUE. Thus, unless autocorrelation is
very high or there is a large sample, FGLS may not perform as well as
the somewhat-inefficient OLS. As such, FGLS should be used with caution.
The most common way of estimating rho in FGLS is the Cochrane-Orcutt
iterative procedure in which we begin with (i) an estimated *ρ* and use
it to estimate regression coefficients by GLS, and (ii) given the
regression coefficients, we estimate *ρ*. This procedure is iterated
until convergence is reached, yielding an estimated *ρ̂* which can be
used in the place of the true rho in the already-described GLS procedure
that will have desirable asymptotic properties, but may not be BLUE and
thus can be more problematic than OLS in small samples.

## OLS Assumptions, Violations, Fixes

*What are classical assumptions accompanying OLS estimation of a linear
additive regression model? What does each get us? (What is cost of
failing?) Which are equally necessary for any estimator of the model,
not just OLS? Which is likeliest to be violated? What can be done about
each violation?*

The Gauss-Markov Theorem (GMT) defines the finite-sample properties of
the OLS estimator. If the GMT assumptions are met, then the OLS
estimator will be the best linear unbiased estimator (BLUE). This means
that OLS will have the lowest variance among all linear unbiased
estimators, where unbiased indicates that the expected value of the OLS
parameter estimates is equal to the population parameter. These are both
desirable properties for an estimator.

The GMT assumptions are:  
(1) Linearity in parameters *Y* = *X**β* + *ϵ* and
*β̂*<sub>*O**L**S*</sub> = (*X*′*X*)<sup>−1</sup>*X*′*Y*  
(2) Full Rank *r**a**n**k*(*X*) = *K* ≥ *N*  
(3) Spherical Error Variance
*V**a**r*(*u*\|*X*) = *σ*<sub>*ϵ*</sub><sup>2</sup>*I*<sub>*n*</sub>,
(no autocorrelation
*c**o**v*(*u*<sub>*i*</sub>,*u*<sub>*j*</sub>\|*X*<sub>*i*</sub>,*X*<sub>*j*</sub>) = 0,
and no heteroskedasticity
*V**a**r*(*u*<sub>*i*</sub>) = *E*\[*u*<sub>*i*</sub>−*E*(*u*<sub>*i*</sub>\|*X*<sub>*i*</sub>)\]<sup>2</sup>)  
(4) Strict Exogeneity
$x_i \\protect\\mathpalette{\\protect\\independenT}{\\perp}\\epsilon_i$
(X fixed in repeated observations or stochastic and
*c**o**v*(*X*<sub>*i*</sub>,*u*<sub>*i*</sub>) = 0, zero conditional
mean *E*(*u*\|*X*) = 0, strict exogeneity *E*(*u*\|*X*) = *E*(*u*))

\(1\) Linearity in Parameters

The linearity in parameters assumption defines the functional form of
the models that OLS is appropriate to estimate. The linearity assumption
states that the equation must be linear in parameters (not linear in
variables). This means that the parameters in the equation must be
linear and additive, as shown in \[A.1.1\] (for example, the model
cannot be exponential as shown in the Cobb-Douglas Production Function
with additive error in \[A.1.5\]). Linearity in parameters provides
simple interpretation of parameter estimates. The coefficients can be
interpreted as the change in Y for each unit change in X. Linearity also
facilitates comparison of efficiency between estimators. In the case of
intrinsically non-linear models, as shown in \[A.1.5\], non-linear
regression of maximum likelihood estimation (MLE) should be used.
Estimating this equation using any linear model will result in biased
coefficients, as the relevant functional form has been omitted and an
irrelevant functional form has been used. In the case of intrinsically
linear regression models that are expressed in a non-linear fashion,
transformations can be used in order for the model to be additive and
linear, as is the case with the Cobb-Douglas production function with
multiplicative error, shown in \[A.1.6\]. Taking the natural log of both
sides of the equation yields \[A.1.7\], which can be estimated using
OLS. The linearity in parameters function is crucial, but violations are
comparatively rare and can be addressed using transformations or by
using different estimators. This is an important requirement for any
linear estimator and its violation can lead to serious specification
bias, but violations can generally be handled by using nonlinear
regression, MLE, or by transforming the model.

\(2\) Full Rank

The full rank assumption is also very important. Violations of full rank
mean that the OLS estimation will be indeterminate. This is, therefore,
more of a technical requirement for estimation than it is an assumption
required for OLS to be BLUE. Full rank requires there to be variation in
the regressors, requires there to be more observations than regressors,
and requires that no regressor can be an exact linear expression of any
other regressor or set of regressors. The requirements that variables
must vary and that there need to be more observations than regressors
are fairly straightforward. If these fail, then there is simply no way
to determine the slope coefficients due to insufficient information. The
requirement that no regressor can be an exact linear expression of any
other regressor or set of regressors is better known as no perfect
collinearity or no perfect multicollinearity. This is more likely to be
violated than the first two, but is straightforward to fix.

The two reasons we would typically run across perfect collinearity or
perfect multicollinearity are: for perfect collinearity, one x variable
is simply an alternative measure of another x variable (i.e. area in
square miles and area in square kilometers); for perfect
multicollinearity, we have fallen into the "dummy variable trap", which
occurs when we are interested in controlling for or estimating the
relationship between a categorical variable and the regressand (for
example, we have created dummy variables for each of the following
regions: north, south, east, and west) and instead of including all but
one and using the omitted category as a baseline, we have included all
four dummy variables, resulting in multicollinearity. The answer to both
these problems is to drop one of the variables.

In the first example, no omitted variable bias will be introduced
because we are simply eliminating two versions of the same information.
For the second example, excluding the last dummy variable results in a
saturated model. Imperfect but problematic multicollinearity (where
multiple X variables are highly correlated), is often included under
this assumption, but is not a violation of the Gauss-Markov Theorem. In
the presence of imperfect but problematic multicollinearity, the OLS
will still be BLUE, but the results may be difficult to interpret: there
may be a high *R*<sup>2</sup> with very high p-values for some or all of
the explanatory variables. In this case, caution should be used before
dropping highly-collinear variables as this can introduce omitted
variable bias, which is a far greater sin. Note that full rank is a
requirement for any estimator: violations of full rank leave slope
coefficients undefined.

\(3\) Spherical Error Variance

The spherical error variance assumption is required for OLS to be BLUE.
If it is violated, OLS will still be unbiased, but will no longer be the
most efficient among all linear unbiased estimators. This assumption is
most frequently violated in the presence of heteroskedasticity or
autocorrelation. Heteroskedasticity happens when the variance changes
between different X values. An example of this would be if we were
interested in measuring the relationship between income (X) and savings
(Y). Individuals with low income typically spend a greater percentage of
their income on basic necessities and thus have very little flexibility
in their spending and savings habits. This means that at low X values
there will be low variance. Individuals with high incomes only need to
spend a small percentage of their income on basic necessities, leaving
these individuals with more flexibility in how they spend or save their
money. We should expect the variance on savings to be much higher at
higher levels of X. There are a few ways to deal with
heteroskedasticity. The first is to attempt to transform the variables
to limit the differences in variance. This can sometimes result in more
uniform error variance, restoring homoskedasticity to the data and
making OLS the BLUE. If we have information about the variance and know
*σ*<sub>*i*</sub><sup>2</sup>, then we can use a specific type of
generalized least squares (GLS) called weighted least squares (WLS),
which will be the BLUE. Weighted least squares minimizes a weighted
residual sum of squares using the inverse of the known
*σ*<sub>*i*</sub><sup>2</sup> as the weight. Thus, WLS weights
observations from populations with high variance lower and weights
observations from populations with low variance higher than OLS, which
minimizes an unweighted (uniformly weighted) residual sum of squares. By
taking this additional information into account, WLS is able to provide
efficient estimates, making it the BLUE under heteroskedasticty.
Finally, we can use the White robust standard errors, which do not solve
the problem of efficiency, but will provide unbiased estimates of the
standard error, thereby greatly reducing though not alltogether solving
the problems with using OLS for inference in the presence of
heteroskedasticity.

Autocorrelation can be spatial (cross-sectional) or temporal
(time-series) in nature. Autocorrelation occurs when there is
interdependence among the disturbance term between observations or
within observations over time. Returning to the example of income and
savings, the consumption habits of a neighbor may affect the consumption
habits of an individual (i.e. if the neighbor buys a new car, the
individual might feel the need to compete by buying a new car himself),
causing spatial autocorrelation between the neighbors. Consumption and
savings habits in an individual may also follow trends or be cyclical in
nature. If we are collecting weekly data on an individual, we are likely
to notice a sharp decline in savings for the several weeks leading up to
Christmas and then attempts to correct for this spending in the
subsequent months by saving more, which would be serial correlation. If
tests suggest that there is autocorrelation in the data, it is important
to first make sure that this is because of pure autocorrelation and not
due to model misspecification such as the wrong functional form or
omitted variables before moving on. In these cases, what appears to be
autocorrelation is actually model misspecification, which is a much
bigger problem than autocorrelation and which has different solutions.

GLS also provides a simple solution for autocorrelation if the
coefficient of first-order autocorrelation (rho) is known. Here, GLS can
use rho to weight a lagged regression which, if subtracted from the
unlagged regression can restore the desireable properties to the error
term, thus making GLS the BLUE. If rho is unknown, it can be estimated
and used in a feasible generalized least squares (FGLS) estimator. The
rho is typically estimated using an iterative procedure in which (i) rho
is estimated and used to estimate the regression coefficients, and (ii)
the estimated regression coefficients from (i) are used to estimate the
rho. This procedure is repeated until convergeance is achieved. The
problem with using FGLS is that the rho is estimated, and since we are
using an estimate rather than the true rho the estimator is only
consistent and asymptotically efficient. Its small sample properties are
unknown. Thus, FGLS should be used with caution in small samples, and
unless autocorrelation is very high, the OLS estimator is likely to be a
better choice for small samples. In addition to GLS and FGLS, we can use
HAC robust standard errors, which are quite similar to White’s robust
standard errors, but are robust to both heteroskedasticity and
autocorrelation. Still other options for addressing autocorrelation are
to use spatial or time-series regression techniques that take the
sources of autoregression into account.

\(4\) Strict Exogeneity

The strict exogeneity assumption takes multiple forms. At the extreme is
the fixed X assumption, which assumes that the independent variables are
fixed in repeated sampling. This rarely holds outside of tightly
controlled experimental settings, so it is generally relaxed to a
stochastic X assumption which requires the X variables are independent
of the error term. This is still a very strong assumption. This is also
one of the most important assumption of OLS, because violations of
strict exogeneity result in biased coefficients. These biases can not
only be large but can also render OLS inconsistent–that is, as the
number of observations increase to infinity, the probability limit of
the estimated parameter will never converge on the population parameter.
This is also an important Gauss-Markov assumption because it is often
violated, even in its relaxed form. There are several causes of
violations of strict exogeneity that are both common and lead to biased
parameter estimates. These include (1) errors in variables, (2)
simultaneity, and (3) omitted confound variables. A much less
problematic violation is if there is a nonzero conditional mean of the
disturbance term. This simply leads to a biased intercept, which is much
less problematic because the parameter estimations will still be
unbiased.

(4.1) Errors in Variables  
Errors in variables refers to errors in the measurement of variables in
the data. This is less problematic when the dependent variable is
measured with error–in this case, OLS will be less precise than it would
be if Y had been measured without error, but the disturbance term
accounts for measurement error in the dependent variable. Errors in the
measurement of X variables are far more problematic and will cause
violations of the strict exogeneity assumption. This is because if an X
variable is measured with error, then the classic error in variables
problem occurs. In this case, even if the true unobserved x variable is
uncorrelated with the error term, this is no longer the case when
observations of that x are measured with error. The observed x variable
x\*, can be written as x\*=x+e where "x" is the unobserved true value of
x, "x\*" is the observed x with measurement error, and "e" is the error
in measurement. If we attempt to estimate the linear regression model
y=bx+u (where y is the dependent variable, b is the parameter estimate
for the x variable, and u is the disturbance term) using the bad-x, we
are actually estimating y=bx\*+u. By substitution, we get y=b(x+e)+u,
and moving e to the error term, we get y=bx+(u+be). Thus, when x is
measured with error, it is automatically correlated with the disturbance
term and the parameter estimate will be biased and inconsistent. In a
multiple regression model, if the bad-x is correlated with other x
variables then the parameter estimates will also be biased. Worse, this
will also be true of most estimators. The solution to this is to use an
instrumental variable that is highly correlated with the x, only causes
y through x, and is uncorrelated with the error term. This will yield
unbiased estimates, but is hardly a trivial matter. Finding strong and
exogenous instruments is exceedingly difficult.

(4.2) Simultaneity  
Simultaneity occurs when y and x are mutually determined, as occurs with
supply and demand. OLS cannot account for this relationship in the data,
but this can be solved by using simultaneous equation model, such as the
two-stage least squares estimator, which, again, requires a good
instrument.

(4.3) Wrong Regressors  
Including irrelevant regressors is a comparatively trivial problem. This
can decrease the precision of our estimates by lowering the efficiency
compared to the same OLS with only the irrelevant regressor left out.
However, the estimator will still be unbiased and consistent.

Omitting relevant independent variables is a much bigger problem. This
will result in biased coefficients. A confound is a variable that causes
both y and x. Include all theoretically-relevant variables if possible,
but this is not possible with unobservable confounds and if confounds
are measured with error, then we return to the errors-in-variables
problem. Fixed effects estimations can be used if panel data are
available to eliminate unobservable time-invariant confounds, but this
precludes the estimation of the relationship between time-invariant x
variables of theoretical interest and y. Instrumental variable models
can be used to isolate the relationship between x and y if a suitable
instrument can be found.

Strict exogeneity is perhaps the hardest assumption to satisfy, the
solutions that require instrumental variables are quite difficult to
achieve. The worst of these problems will carry over to other estimators
as well, unless valid instruments are found.

## Point Estimation, Interval Estimation, and Hypothesis Testing

*How do we conduct estimation and hypothesis testing in the standard
(frequentist) statistical approach?*

-   We draw a sample of *x*<sub>1</sub>, …, *x*<sub>*n*</sub>, which are
    generated from an underlying probability density function (PDF). We
    typically assume the observations are identically and independently
    distributed, and thus have a single PDF. Use the observations to
    estimate the value of a parameter in the population PDF.

-   For instance, when *x*<sub>1</sub>, …, *x*<sub>*n*</sub> follow a
    normal distribution with mean *μ* and variance *σ*<sup>2</sup>, we
    would like to estimate the parameter *μ* using the observations
    *x*<sub>1</sub>, …, *x*<sub>*n*</sub>.

-   Construct an estimator: an algebraic function of sample data that
    creates a numerical estimation of a parameter (a simple example
    would be to use the sample average of
    *x*<sub>1</sub>, …, *x*<sub>*n*</sub> as an estimator of the
    parameter *μ*.)

*Name three properties that make a good estimator, defining each and
giving an example of an estimator that has the property.*

-   *Unbiasedness*: An estimator is unbiased if the sampling
    distribution of the estimated parameter *β*<sup>\*</sup> is equal to
    the true population parameter *β*. Formally defined,
    *E*(*β*<sup>\*</sup>) = *β*. Bias is the difference between
    *E*(*β*<sup>\*</sup>) and *β*.

-   *Efficiency*: Efficiency is related to the size of the sampling
    variance and is a property that is relative to alternative
    estimators. Smaller sampling variance of an estimator is preferable
    to larger sampling variance because it is more likely that any given
    estimate from a more efficient estimator will be closer to the true
    *β* than an estimate from a less efficient estimator. Formally,
    *V**a**r*(*β̂*) ≤ *V**a**r*(*β̃*), where $\\hat{beta}$ is an estimator
    of interest and *β̃* is an alternative estimator. Absolute efficiency
    measured by *V**a**r*(*β̂*) is not a property of an estimator. In
    conventional terms, efficiency ensures the reliability of an
    estimator.

-   *Consistency and Asymptotic Efficiency*: If the asymptotic
    distribution of *β̂* becomes concentrated on a value *k*, then
    *p**l**i**m*(*β̂*) = *k*, which states that *k* is the probability
    limit of *β̂*. If *p**l**i**m*(*β̂* = *β*, then the estimator is
    consistent. While unbiasedness and efficiency relate to the small
    sample properties of an estimator, consistency and asymptotic
    efficiency are their respective infinite sample property analogs.

*Give an example of a situation where we may choose to use an estimator
that does not have one of the properties you listed and explain why such
an estimator may be desirable.*

-   The estimator that offers the best linear unbiased estimate (BLUE)
    of the parameter is the estimator that offers the minimum variance
    among all unbiased linear estimators, and this is often the
    preferred estimator because of these properties. There can be
    circumstances in which one might prefer not to use the BLUE
    estimator. This may occur when there is a substantial tradeoff
    between unbiasedness and efficiency, as is the case when the *best
    unbiased criterion cannot produce estimates with small variance*.

-   For example, there may be an estimator which is *somewhat biased but
    more efficient* than the estimator that provides the best (linear)
    unbiased estimate. In this case, the biased but efficient estimator
    may be more likely in any given sample to give an estimate closer to
    the true population parameter than an unbiased but inefficient
    estimator. In this case, the somewhat biased estimator with low
    variance may be preferable. The tradeoffs between bias and
    efficiency can be navigated by using the mean square error, which
    minimizes the weighted average of the bias and its variance using
    the square of the bias.

-   When the Gauss-Markov assumptions are met, OLS possesses all of
    these properties. GLS estimators (including FGLS and WLS) possess
    the consistency and asymptotic efficiency properties, but will not
    necessarily be the BLUE, especially with low sample sizes. As a
    result, these estimators may be preferable to OLS when the spherical
    error variance assumption is violated due to autocorrelation or
    heteroskedacity that renders the OLS estimator highly inefficient.
    Under small sample sizes, however, even an inefficient OLS might be
    preferable.

*Explain the steps of testing a hypothesis about the value of an unknown
parameter. Your answer should include definitions and discussions of the
sampling distribution and p-value.*

-   Two types of estimation: point and interval.

    -   Point estimation: estimation that produces a single value, which
        I have discussed above.

    -   Interval estimation: we would like to know a confidence
        interval, an interval that contains a parameter with a certain
        frequency. To construct a confidence interval, we need to
        know (1) the variance of an estimator and (2) the probability
        distribution of the estimator (sampling distribution): the
        distribution of statistics in an infinite number of samples.

    -   The sampling distribution can be derived from probability
        distributions of observations or asymptotically using the
        central limit theorem.

    -   If we know that the observations follow a normal distribution,
        the sum of normally distributed variables is also normally
        distributed, and the sampling distribution of the sample average
        is *N*(*μ*,*σ*<sup>2</sup>/*n*). Even when we do not know the
        underlying probability distribution, the central limit theorem
        states that the sample average follows a normal distribution
        when we have an infinite number of observations. Thus, we can
        assess the asymptotic sampling distribution of an estimator.

    -   Once we have a sampling distribution, we can construct a
        confidence interval. A confidence interval is an interval that
        contains a certain probability density in the sampling
        distribution.

    -   Confidence interval is often preferable, since the null
        hypothesis can often be a straw man.

-   In a hypothesis test, we compare null and alternative hypotheses. In
    the simplest format (Fisher test), we examine a p-value, a
    probability that a test statistic takes equal or more extreme values
    than what is observed given a null hypothesis. If the p-value is
    lower than a pre-specified threshold, the null hypothesis is highly
    incompatible with data, and thus we reject the null and accept the
    alternative hypothesis. In this procedure, a sampling distribution
    of a test statistic is essential; without it we cannot calculate the
    p-value.

-   A p-value is essentially the CDF of a sampling distribution of a
    test statistic. A test statistic usually contains an estimator and a
    parameter, and the value of a parameter is given by a null
    hypothesis. As a result, the sampling distribution of a test
    statistic is a direct function of the sampling distribution of an
    estimator. Thus, the sampling distribution of an estimator provides
    the sampling distribution of a test statistic given a null
    hypothesis, which in turn provides a p-value.

-   Consider the above example of a normal distribution. A null
    hypothesis is mu=0, and the alternative hypothesis is that mu is not
    zero. The test statistic is the z statistic, assuming
    *σ*<sup>2</sup> is known. Because
    $\\overline{Y} \\sim N(0,\\sigma^2$ given the null hypothesis, the z
    statistic follows the standard normal distribution. Thus, we can
    calculate the probability that the test statistic takes equal or
    more extreme values than what is observed. For instance, when
    $\\overline{Y}=10$, the p-value is the density of the standard
    normal distribution over 10 to positive infinity. When
    *σ*<sup>2</sup> is unknown, we can insert the empirical estimate
    \[A2-6\] to the test statistic. In a finite sample, the test
    statistic follows the t distribution. In an infinite sample, the
    test statistic still follows the standard normal distribution. We
    then can calculate the p-values.

-   In hypothesis testing, we aim to make a decision about two competing
    hypotheses. We first need to specify two mutually exclusive
    hypotheses. A *null hypothesis* is a baseline hypothesis while an
    *alternative hypothesis* is the hypothesis of interest. We can
    either reject the null hypothesis in favor of the alternative
    hypothesis or we can fail to reject the null hypothesis. These
    determinations are made at a pre-determined threshold. In hypothesis
    testing, it is usually convenient transform an estimator to a test
    statistic whose probability distribution is well known.

-   In the Fisher test, we examine a p-value, a probability that we
    obtain equal or more extreme values of a test statistic than what is
    observed. When a p-value is lower than a pre-specified threshold,
    the null hypothesis is unlikely to be compatible with data, and thus
    we reject the null hypothesis. In our example, the test statistic is
    a z statistic that follows a standard normal distribution. If the z
    statistic takes an extreme value and thus the probability density is
    sufficiently small, we reject the null hypothesis.

-   The Neyman-Pearson test is similar to the Fisher test, but its
    procedure is slightly different. Instead of looking at p-value, we
    construct a rejection region. To construct the rejection region, we
    need to specify the rate of Type I error (an error to reject the
    null when the null is actually true) and find the range of a test
    statistic that minimizes the rate of Type II error (a failure to
    reject the null when the null is actually false). The rate of Type I
    error is called a significance level, while 1 minus the rate of Type
    II error is called power. When the observed test statistic falls
    within the rejection region, we reject the null.

-   Once we conduct a hypothesis test, we can make a decision about
    rejecting or failing to reject the null hypotheses. Note however
    that with the increasing skepticism towards hypothesis tests, the
    best practice is to report the confidence intervals and p-values
    rather than making a decision. Furthermore, confidence intervals and
    p-values must be interpreted with caution. *A confidence interval is
    an interval over a test statistic, not a parameter. A p-value is a
    probability about data not a parameter.* To estimate the intervals
    over parameters and probabilities of hypotheses, we need to conduct
    the Bayesian inference.

-   t-Test

    -   Calculate the sample means from two independent samples, each
        from populations with the same variance.

    -   Hypothesis: two samples are, on average, different (Null
        hypothesis: on average same)

    -   Ask “how unlikely is it that we observe the test statistic in
        the distribution if the null were true?"

    -   Assuming sample means are normal (more likely to hold
        asymptotically due to CLT, so be extra careful in small
        samples), if the value of the test statistic falls in the
        critical region and is thus highly unlikely, then we are
        confident that we can reject the null hypothesis. If the test
        statistic is not in the critical region, then fail to reject the
        null hypothesis.

-   F-test

    -   State the null hypothesis and the alternate hypothesis.

    -   Calculate the F value. The F Value is calculated using the
        formula F = (SSE1 – SSE2 / m) / SSE2 / n-k, where SSE = residual
        sum of squares, m = number of restrictions and k = number of
        independent variables.

    -   Find the F Statistic (the critical value for this test). The F
        statistic formula is: F Statistic = variance of the group means
        / mean of the within group variances.

    -   You can find the F Statistic in the F-Table.

    -   Support or Reject the Null Hypothesis.

## Interactions in a Linear Regression

-   Assume a linear regression model with an interactive term
    *y*<sub>*i*</sub> = *α* + *β**x* + *γ**z* + *δ**x**z* + *ϵ* that
    meets the assumptions of linearity, zero conditional mean, strict
    independence of the error term from the regressors, and spherical
    error variance. In a normal linear regression model, we also assume
    normality of the error term.

-   A linear regression has an interaction term when the effect of an
    independent variable on y is conditional on the value of another
    regressor. For example, the effect of democracy on GDP growth may
    rely on bureaucratic efficiency. That is, democracy alone may not
    accelerate growth, but a democracy with an efficient bureaucracy may
    do so. In this case, we need to use an interaction term to model the
    relationship.

-   The coefficients in a linear interaction model can be interpreted in
    a following way;

    -   *α*: *y*<sub>*i*</sub> when both *x*<sub>*i*</sub> and
        *z*<sub>*i*</sub> are zero;

    -   *β*: change in *y*<sub>*i*</sub> when *x*<sub>*i*</sub>
        increases by one unit and *z*<sub>*i*</sub> is zero;

    -   *γ*: change in *y*<sub>*i*</sub> when *x*<sub>*i*</sub> is zero
        and *z*<sub>*i*</sub> increases by one unit;

    -   *δ*: change in the effect of *x*<sub>*i*</sub> when
        *z*<sub>*i*</sub> increases by one unit, or change in the effect
        of *z*<sub>*i*</sub> when *x*<sub>*i*</sub> increases by one
        unit. The “effect” here is a change in *y*<sub>*i*</sub> when
        *x*<sub>*i*</sub> or *z*<sub>*i*</sub> increases by one unit.

-   The coefficients *β* and *γ* are often mistakenly interpreted as
    “unconditional” effects of *x*<sub>*i*</sub> and *z*<sub>*i*</sub>,
    but this interpretation is clearly incorrect. They represent *the
    effect of an independent variable when another regressor is set to
    zero.*

-   *Effects of x and z*: To understand the effects of *x*<sub>*i*</sub>
    and *z*<sub>*i*</sub>, we can take partial derivatives of the
    right-hand size with respect to *x*<sub>*i*</sub> and
    *z*<sub>*i*</sub>.

    -   The derivatives represent the change in *y*<sub>*i*</sub> when a
        regressor increases by one unit. The first equation shows that a
        unit-increase of *x*<sub>*i*</sub> changes *y*<sub>*i*</sub> by
        *β* + *δ* \* *z*<sub>*i*</sub>, which indicates that the effect
        of *x*<sub>*i*</sub> is conditional on *z*<sub>*i*</sub>. In
        particular, a unit increase of *z*<sub>*i*</sub> changes the
        effect of *x*<sub>*i*</sub> by *δ*. Interestingly, the
        interaction model also indicates the effect of *z*<sub>*i*</sub>
        conditional on *x*<sub>*i*</sub>. A unit increase of
        *z*<sub>*i*</sub> change *y*<sub>*i*</sub> by
        *γ* + *δ* \* *x*<sub>*i*</sub>. Thus, the effect of
        *z*<sub>*i*</sub> is also conditional on *x*<sub>*i*</sub>,
        meaning that a unit increase of *x*<sub>*i*</sub> changes the
        effect of *z*<sub>*i*</sub> by *δ*.

    -   In order to get a concise summary about the effect of
        *x*<sub>*i*</sub> and *z*<sub>*i*</sub>, we can also compute the
        partial effect at mean and the average partial effect. The
        partial effect at mean is the value of the partial derivatives
        when the conditioning variable is set to a sample average. When
        we consider a sample average is not a representative value, we
        can use the average partial effect. To obtain the average
        partial effect, we calculate \[A3-6\] for every individual and
        then compute their average.

    -   Finally, graphical presentation is also useful. For this
        purpose, we can conveniently plot the values of partial
        derivatives versus those of a conditioning variable.

-   *Statistical significance of *δ** Statistical significance of
    estimated *δ* means that we are very unlikely to obtain the estimate
    or more extreme values if population *δ* is zero. Thus, *δ* is
    unlikely to be zero.

    -   A direct implication is that the omission of the interaction
        term leads to the miss-specification of the model and cause the
        bias, which is analogous to the omitted variable bias. For
        instance, when *z*<sub>*i*</sub> positively correlates with
        *x*<sub>*i*</sub> \* *z*<sub>*i*</sub>, delta is positive in an
        interaction model, and an estimate of *γ* is positive in a model
        without the interaction term, the positive coefficient of *γ* is
        actually biased toward positive and thus overstate the
        unconditional effect of *z*<sub>*i*</sub>.

    -   The statistical significance also indicates that the effect of
        *x*<sub>*i*</sub>(*z*<sub>*i*</sub>) is likely to be conditional
        on *z*<sub>*i*</sub>(*x*<sub>*i*</sub>). As the partial
        derivatives in A3-4 shows, the effect of an independent variable
        is conditional on the other regressor only when *δ* is non-zero.
        If *δ* is zero, there exist no conditional effect.

    -   Note however that statistical significance does not guarantee
        existence of substantively large interactive effects. Even if
        *z*<sub>*i*</sub>(*x*<sub>*i*</sub>) only very weakly conditions
        the effect of *x*<sub>*i*</sub>(*z*<sub>*i*</sub>), we can get
        statistical significance of estimated *δ* in a large sample.
        Thus, we need to carefully assess the size of conditional
        effects mobilizing our substantive knowledge.

    -   Statistical significance of estimated *δ* is neither sufficient
        nor necessary for establishing existence of conditional
        effects. (1) Significant *δ* is not necessary, because
        compression can cause a conditioning relationship. Even when *δ*
        is zero and thus there exists no interaction term, compression
        can cause a conditional relationship. (2) Significant *δ* is not
        sufficient, because *the interaction effect can be canceled out
        by compression*. This is rare, but requires us to inspect the
        interactive effect carefully. (3) Statistically significant
        estimates do not mean substantively significant conditional
        relationship.

    -   The corollary is that statistical non-significance of estimated
        *δ* does not guarantee either existence or absence of
        interactive effects. (1) Non-significance does not mean *δ* is
        zero. It simply means we have no sufficient evidence to reject
        the null. (2) Even if *δ* is zero, compression can cause
        conditional relationship. Thus, the p-value is often useless to
        assess the existence of conditional relationship.

## Comparisons of Estimators

-   Compare OLS, GLS (fGLS and WLS), 2SLS, and MLE (Probit and Logit).

-   OLS

    -   *Statistical Properties:* Under the Gauss-Markov Assumptions,
        OLS is the best linear unbiased estimator in the finite sample
        setting, meaning that it has the smallest variance among all
        unbiased linear estimators. Furthermore, if the disturbance term
        follows a normal distribution according to the Classical Linear
        Model assumptions, then the OLS is the best unbiased estimator
        among all estimators, not just linear.

    -   *Classical Assumptions:*

        -   Linearity *y* = *α* + *β**X* + *ϵ*, which specify the
            functional form of the systematic and stochastic variations
            of a dependent variable.

        -   Full Rank *R**a**n**k*(*X*) = *k* ≥ *N*, a technical
            requirement rather than a theoretical assumption. Without
            this requirement, however, X is not invertible and thus OLS
            is not well-defined.

        -   Spherical Error Variance *E*(*ϵ*\|*X*) = *σ*<sup>2</sup>*I*,
            the variances of the error terms should be constant and they
            should have zero covariance. This requires no
            autocorrelation and no heteroskedasticity.

        -   Strict Exogeneity *E*(*ϵ*\|*X*) = *E*(*ϵ*) = 0). There is
            some variability in the strictness of this assumption. The
            strictest interpretation requires fixed x variables, an
            assumption which is unlikely to hold outside of experimental
            settings. In a simple linear regression,
            *c**o**v*(*u*<sub>*i*</sub>,*x*<sub>*i*</sub>) = 0 is
            sufficient.

        -   Plus normality of disturbances *ϵ* ∼ *N*(0,*σ*<sup>2</sup>),
            which is an assumption included in the Classical Linear
            Model but not the Gauss-Markov assumptions, and is needed
            for hypothesis testing because the sample distribution must
            be known in order to conduct accurate hypothesis tests. This
            assumption is most useful in finite samples, and holds more
            often in larger samples due to the central limit theorem and
            the law of large numbers.

    -   *Drawbacks:* The Gauss-Markov assumptions are rarely met in
        full. Violations of the most crucial assumption, strict
        exogeneity, render OLS not only biased but also inconsistent,
        meaning that even in an infinite sample, the estimated
        parameters will never converge on the true population values.
        Strict exogeneity is difficult to demonstrate in observational
        data due to selection bias, simultaneity, measurement error, and
        often-unobservable omitted variables. Furthermore,
        heteroskedasticity is common in cross-sectional data and serial
        correlation is common in time series data, so the spherical
        error variance assumption is also frequently violated. When
        heteroskedasticity and serial correlation are present in the
        data, OLS will still be unbiased, but will be inefficient. If
        the error term is not normally distributed, but is assumed to
        be, then hypothesis testing may be misleading.

    -   *OLS Comparison to GLS*: When the spherical error variance
        assumption is plausible and thus the variance-covariance matrix
        is close to *σ*<sup>2</sup>*I*, OLS and GLS (FGLS and WLS) will
        report very similar results. GLS will be preferable when the
        spherical error variance assumption is implausible and there are
        many observation, as GLS takes into account additional
        information about the error variance in the presence of
        heteroskedasticity or autocorrelation because OLS will no longer
        be the BLUE, either WLS or FGLS will be. This is because
        violation of the spherical error variance assumption decreases
        the relative efficiency of OLS. As long as the spherical error
        variance assumption holds, OLS will be the BLUE and will
        therefore be more useful and informative, especially for small
        samples.

    -   *OLS Comparison to MLE*: If we are only interested in point
        estimations of parameters in a regression model, then OLS, which
        makes no assumptions about the probability distributions of the
        error term, will suffice. If we are interested in estimation and
        inference, then we need to know the underlying probability
        distribution. With the addition of the normality assumption in
        the CLM, OLS estimators of regression coefficients are the
        Maximum Likelihood Estimator (conditional on the explanatory
        variables) and are also the Best Unbiased Estimator. When a
        dependent variable is not normally distributed and is asymmetric
        it violates the assumptions of linear regression. When the
        variable can be transformed (using the log, sqrt, square, etc)
        to an approximately normal distribution, then OLS can still be
        used effectively. However, when *E*(*y*\|*x*) is *not* linear
        and cannot be made linear through transformations (as is the
        case with limited dependent variables), maximum likelihood
        methods become crucial since OLS and GLS are no longer
        applicable. This is because MLE is based on the distribution of
        *y* given *x*.

    -   *OLS Comparison to 2SLS*: 2SLS can be used in circumstances in
        which endogeneity problems are believed to bias OLS. This is the
        case when there are confounds or omitted variables that cannot
        be adequately accounted for, when there is measurement error in
        the explanatory variables, or when there are simultaneity or
        reverse causality problems between the dependent and independent
        variables. Though 2SLS is attractive for its causal inference
        properties, the estimator also has assumptions that are rarely
        met. Using 2SLS requires a strong and exogenous instrumental
        variable—that is, an investigator must find a variable that not
        only strongly predicts the endogenous explanatory variable of
        interest but is also uncorrelated with the error term in the
        original equation. If the instrumental variable is only weakly
        correlated with the endogenous explanatory variable or if there
        is any violation of exogeneity, then the 2SLS approach will
        fail.

-   Generalized Least Squares

    -   Unlike OLS, GLS does not require spherical error variance. The
        variances of the error terms can be non-constant and errors can
        correlate with each other. GLS can produce consistent estimates
        of the variance-covariance matrix of error terms.

        -   *GLS*: Solution to autocorrelation when the coefficient of
            first-order autocorrelation *ρ* is known. Multiplies a
            lagged standard OLS equation by *ρ* and subtract this from
            the standard OLS quation, resulting in a generalized
            difference equation. One can then apply OLS to the
            transformed (now in difference form) equation which will now
            possess the BLUE properties.

        -   *FGLS*: Feasible generalized least squares is the solution
            to autocorrelation when the coefficient of first-order
            autocorrelation *ρ* is unknown and must first be estimated
            (*ρ* is rarely known). This is a two-step method in which
            *ρ* is first estimated and then used to transform the
            variables into the generalized difference equation, as
            discussed above with GLS. FGLS involves an iterative
            procedure to estimate *ρ*. The estimation procedure is as
            follows: (a) Given an estimated variance-covariance matrix,
            compute the GLS estimates; (b) Given the GLS coefficient
            estimates, compute the estimate of the variance-covariance
            matrix. Repeat the iterations until the estimates achieve
            convergence.

        -   *WLS:* Weighted Least Squares is a special case of GLS used
            to obtain efficient estimates under heteroskedasticity.
            Whereas OLS uses equal weights on the residual sum of
            squares whereas, uses weighted RSS so that observations from
            populations with larger *σ*<sub>*i*</sub> are weighted less
            than than populations with smaller *σ*<sub>*i*</sub>. Used
            to adjust for a known form of heteroskedasticity where each
            squared residual is weighted by the inverse of the
            (estimated) variance of the error. Use WLS if the
            heterskedastic variances *σ*<sub>*i*</sub><sup>2</sup> are
            known.

    -   *Statistical Properties*: If *σ*<sub>*i*</sub><sup>2</sup> and
        *ρ* are known, WLS and GLS will be BLUE. FGLS is only
        consistent, asymptotically efficient because *ρ̂* is estimated.

    -   *Drawbacks*: FGLS needs to be used in large samples for
        asymptotic properties to hold. WLS and GLS require us to know
        the *σ*<sub>*i*</sub><sup>2</sup> and *ρ*, respectively, which
        rarely occurs.

-   MLE

    -   Based on the principle that the sample of data at hand is more
        likely to have come from a real world characterized by one set
        of parameter values than from any other set of values. MLE can
        be defined as a method for estimating population parameters
        (such as the mean and variance for Normal, rate (lambda) for
        Poisson, etc.) from sample data such that the probability
        (likelihood) of obtaining the observed data is maximized.
        Whereas OLS minimizes the sum of square errors, MLE maximizes a
        likelihood function. When the Gauss-Markov assumptions are met
        in addition to the CLM assumption of normality of disturbances,
        OLS and MLE will be identical and will be the BUE.

    -   *Statistical Properties:* The strength of MLE is that, under
        correct specification of the density, we would have the
        asymptotically efficient estimators, and we would be able to
        estimate any feature of the conditional distribution. MLE
        provides a unified approach to estimation and is asymptotically
        efficient, consistent, and asymptotically normal: it is
        generally the most efficient estimation procedure in the class
        of estimators that use information on the distribution of the
        endogenous variables given the exogenous variables.

    -   *Drawbacks:* In most cases the MLE estimators are biased and
        inefficient in small samples. There is generally a tradeoff
        between efficiency and robustness. The desirable properties of
        MLE only hold if the model is specified correctly. Maximum
        likelihood estimators are generally inconsistent if any part of
        the specified distribution is misspecified.

-   Two-Stage Least Squares

    -   If the error term is correlated with any independent variable,
        then OLS will be biased and inconsistent. Bias and inconsistency
        also mean that efficiency comparisons are wrong, so hypothesis
        tests and inferences will be incorrect as well. 2SLS can
        generate unbiased estimates. This is particularly useful when
        there are relationships between variables in a regression (i.e.
        confounding variables, measurement error, omitted variable bias,
        simultaneity, reverse causality). That is, instrumental
        variables are used when your variables are related in some way.
        If you have some type of correlation going on between variables
        (e.g. bidirectional correlation), then more common methods like
        ordinary least squares cannot be used because one requirement of
        those methods is that variables are not correlated. As its name
        implies, the 2SLS method uses two stages of least squares
        regressions. In the first stage regression, a set of exogenous
        variables that are correlated with the endogenous independent
        variable but are uncorrelated with the error term are used to
        generate fitted values of the endogenous independent variable.
        These fitted values enter into the second stage equation in the
        place of the endogenous variable, thereby generating consistent
        estimates of the parameters of interest, which OLS is incapable
        of in the presence of endogeneity.

    -   *Statistical Properties*: Consistent and asymptotically
        efficient.

    -   *Classical Assumptions*: The instrumental variable(s) must be
        strongly correlated with the endogenous explanatory variable but
        uncorrelated with the error term.

    -   *Drawbacks*: Finding an instrument that satisfies the exclusion
        restriction and also strongly predicts the endogenous variable
        is exceedingly difficult. Using a weak or endogenous instrument
        can do more harm than good.
