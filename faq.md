#FAQ

##### What is the ModelSEED?

ModelSEED is a web application for the reconstruction, exploration, comparison, and analysis of metabolic models.  The UI is built primarily on the web service [ModelSEED-Pro](https://github.com/ModelSEED/ProbModelSEED).


##### Which browsers are supported?

We strive to support all evergreen browsers (Chrome, Firefox, Safari and IE10+).  For the best performance, we recommend using <a href="https://www.google.com/chrome/browser/desktop/">Chrome</a>.  Please <a href="https://github.com/ModelSEED/ModelSEED-UI/issues">submit an issue</a> or <a href="mailto:nconrad@anl.gov">email</a> us if you encounter any issues.


##### What has been upgraded?

1. The new ModelSEED biomass works differently in that biomass equations are constant for the gram positive and gram negative templates.
2. The mappings of roles to reactions has changed, as have the roles annotated by SEED itself
3. The ModelSEED utilizes a new biochemistry.  Please see the [ModelSEEDDatabase](https://github.com/ModelSEED/ProbModelSEED) for the latest biochemistry. [More documentation coming]
4. The gapfilling algorithm has changed in that the alorithmn is now a LP (Linear Program) optimization problem, instead of MILP (Mixed Integer Linear Program) optimization problem.  This allows for "fast" formulation.  Although it is possible to have a different solutions, this is uncommon.



