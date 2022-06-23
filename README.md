# MLOPs-Primer

Way to scale up tests in the Recommenders repository

In Recommenders, we run daily around 400 tests in CPU, GPU, and Spark environments that require one or several GPU machines to be up 24/7. Another problem is that the tests need to be sequential, and when there are multiple developers working simultaneously, there is a queue of tests that can take hours. Our new development works in parallel with the help of AzureML, which distributes the tests to different computes. From ~9h, we have managed to bring the end-to-end time down to ~40min and reduce the computing costs to less than half. In addition to the new test infrastructure, I would explain our test platform which includes uncommon systems like ML performance tests and a two-level branch system. 

The MLOps test platform of Recommenders is one of the most sophisticated platforms that we have at Microsoft. 




