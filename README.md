Goal:

Create a 'fresh start' terraform-based MarkLogic Deployment Engine that can operate in a uniform way across hybrid cloud boudaries.

FAQs:

Why target MarkLogic?
  MarkLogic is a mature multi-model database that has been battle tested in huge applications for more than a decade.
  see Defining Data-Driven Software Development https://info.marklogic.com/defining-data-driven-software-development-oreilly.html?type=PD&publisher=Oreilly
  see Building On Multi-Model Databases http://info.marklogic.com/rs/371-XVQ-609/images/building-on-multi-model-databases.pdf
  See Inside MarkLogic Server https://www.marklogic.com/resources/inside-marklogic-server/

Why not target XYZ (instead of MarkLogic)
  First, the approach taken here is actually pretty generic (by design) and could be applied to deployment of other tools.
  Second, MarkLogic checks A LOT of the boxes (see Why target MarkLogic?).
  IF one uses generic deployment methods AND one needs XYZ, add it!

Why a fresh start?
  Resources are available today that were NOT available as the existing tools were built.
  Less integrated MarkLogic components allow better integration with other parts of an application.

Why are 'less integrated' components better?
  Since every application domain is different and pre-built components limit flexibility.

Background:

The MarkLogic approachs (in increasing abstraction):
  MarkLogic Installation Guide: https://docs.marklogic.com/guide/installation.pdf
  On Linux: https://developer.marklogic.com/download
  On Docker: https://hub.docker.com/_/marklogic
  On Mac: https://developer.marklogic.com/download
  On Windows: https://developer.marklogic.com/download
  On Azure: https://www.marklogic.com/resources/deploy-on-azure/
  On AWS (with Managed Cloud): https://docs.marklogic.com/guide/ec2/overview
  DataHub Service: https://www.marklogic.com/product/data-hub-service/ offers the most advanced cluster features now.

Managed Cloud features (from https://cdn1.marklogic.com/wp-content/uploads/2018/01/2017_MLW_LON_Moving-to-the-Cloud.pdf):
  Automatic handling of changes in Amazon EC2 instance hostnames (External FQDNs)
  Automatic placement and management of data, to insure that nothing is lost on transient (EBS) volumes
  Automatic restarting and reconfiguring of failed nodes in a cluster
  "Pausing" of entire clusters, while maintaining all configuration and data

DataHub Service features (from https://www.marklogic.com/blog/introducing-marklogic-data-hub-service/):
  - A scalable MarkLogic cluster 'inside'
  - DataHub functionality: https://github.com/marklogic/marklogic-data-hub
  - As a Service (aaS)
 
