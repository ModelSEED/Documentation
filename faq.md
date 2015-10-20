#FAQ

##### What is the ModelSEED?

ModelSEED is a free, open-source web application for the reconstruction, exploration, comparison, and analysis of metabolic models.  The UI is built primarily on the web service (<a href="https://github.com/ModelSEED/ProbModelSEED" target="_blank">ModelSEED-Pro</a>).  Users can acess the services by creating or using their current <a href="http://rast.nmpdr.org/" target="_blank">RAST</a> or <a href="https://www.patricbrc.org/portal/portal/patric/Home">PATRIC</a> accounts.


##### Which browsers are supported?

We strive to support all evergreen browsers (Chrome, Firefox, Safari and IE10+).  For the best performance, we recommend using <a href="https://www.google.com/chrome/browser/desktop/">Chrome</a>.  Please <a href="https://github.com/ModelSEED/ModelSEED-UI/issues">submit an issue</a> or <a href="mailto:nconrad@anl.gov">email</a> us if you encounter any issues.


##### What resources from the original ModelSEED are used?

Behind the scenes, the steps in pipeline for model reconstruction remain the same as the original ModelSEED. Read more in the paper <a href="http://www.nature.com/nbt/journal/v28/n9/full/nbt.1672.html" target="_blank">here</a>.  However, changes were introduced to the gapfilling algorithm and relevant data that supports model reconstruction was updated. These changes are listed in detail in the section "What has changed?".

Addtionally, you'll notice better performance, more options, and flexibility.


##### What has changed?

1. The assigment of ModelSEED biomass reactions works differently. Biomass reaction content is constant for both gram positive and gram negative templates.
2. The mappings of roles to reactions were changed/upadated, as have the functional roles annotated by <a href="http://rast.nmpdr.org/" target="_blank">RAST</a> in <a href="http://pubseed.theseed.org/" target="_blank">SEED</a> genomes itself. Addtional information on RAST and SEED resources is available <a href="http://nar.oxfordjournals.org/content/early/2013/11/29/nar.gkt1226.full">here</a>.
3. The ModelSEED utilizes an updated biochemistry.  Please see the [ModelSEEDDatabase](https://github.com/ModelSEED/ProbModelSEED) for the latest biochemistry. [More documentation coming soon]
4. The gapfilling algorithm has changed in that the alorithmn is now a LP (Linear Program) optimization problem, instead of a MILP (Mixed Integer Linear Program) optimization problem.  This change substantially reduces the run time of gapfilling. Our method implementation is similar to the one described in <a href="http://www.biomedcentral.com/1471-2105/15/225" target="_blank">here</a>.
5. FBA simulations run with flux minimization (<a href="http://msb.embopress.org/content/6/1/390" target="_blank">pFBA</a>) by default.


##### What are the new features introduced in the new version of the ModelSEED?

1. Introducing the ability to reconstruct genome-scale metabolic models for Plant Genomes. This new feature is the result of integrating the efforts conducted by the <a href="http://bioseed.mcs.anl.gov/~seaver/FIG/seedviewer.cgi?page=PlantSEED" target="_blank">PlantSEED</a> team into the ModelSEED. Details on the methodologies applied for reconstruction of models for Plant Genomes can be found <a href="http://www.pnas.org/content/111/26/9645.full" target="_blank">here</a>.
2. Media editing. Users can now edit existing media formulations in the ModelSEED databse or create their own media formulations.
3. Model editing tools are also being developed, allowing users to quickly edit models directly in the website.
4. Heatmap tools are being created for the comparison of models and FBA simulation results.





