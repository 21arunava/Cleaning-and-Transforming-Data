# Cleaning-and-Transforming-Data
I have used tools in Azure Machine Learning Studio along with R Jupyter Notebook to integrate, clean and transform data.

I have tried my best to ingest, join, and manipulate the
automobile price data using the built-in modules in Azure ML. The built-in modules in Azure ML provide
an easy to use approach to performing some of the most common data transformations, and if one
intends to use an Azure ML experiment to build and publish a predictive web service, one should
generally try to use the built-in modules wherever possible as they are re-configured for production
automatically as part of the web service creation process.

One can use custom scripts to perform the same operations supported by the built-in modules, and in
some cases it is possible to write scripts to make data transformations that are not readily supported by the
built-in modules. However, one should be cautious when using custom code in an experiment that one
intends to publish as a predictive web service – especially if the web service will be required to work with
single row inputs. During the web service creation process, Azure ML converts built-in modules that
perform aggregation operations on multiple rows so that they will work with single rows in production
based on statistical constants derived from training data in the experiment. This conversion cannot be
automated for custom code.

