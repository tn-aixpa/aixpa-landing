# AIxPA Project Landing page

## Documentation

[Core platform documentation](https://scc-digitalhub.github.io/docs/)

[AI Toolbox catalog](https://tn-aixpa.github.io/ai-toolbox-catalog/)

## Repository

### Core Platform

1. [platform](https://github.com/tn-aixpa/platform)

Core Platform Community Kubernetes Helm Charts. List of charts and the instructions for deploying the components of the platform on Kubernetes.

2. [dashboard](https://github.com/tn-aixpa/dashboard)

Dashboard is a landing page UI used as an entry point for accessing the different functionality of the platform - management ui, interactive workspaces, datalake UI, etc. 

3. [core](https://github.com/tn-aixpa/core)

Core is central element of the platform, which performs the main data and execution management operations, such as data and artifact management, metadata management, operation execution, service deployment, etc.

4. [console](https://github.com/tn-aixpa/core-console)

Core console is the management user interface on top of Core API.

5. [sdk](https://github.com/tn-aixpa/core-sdk)

Python SDK to perform the management operations from the interactive environments and to support the data/artifact management automation (e.g., data logging, model logging, etc).

Includes a series of submodules for specific extensions:

- [digitalhub-sdk-runtime-python](https://github.com/tn-aixpa/digitalhub-sdk-runtime-python): Python operations and services execution environment
- [digitalhub-sdk-runtime-container](https://github.com/tn-aixpa/digitalhub-sdk-runtime-container): execution environment for arbitrary Docker containers
- [digitalhub-sdk-runtime-modelserve](https://github.com/tn-aixpa/digitalhub-sdk-runtime-modelserve): execution environment for standard AI model serving
- [digitalhub-sdk-runtime-kfp](https://github.com/tn-aixpa/digitalhub-sdk-runtime-kfp): execution environment for Argo Workflow-based pipelines 
- [digitalhub-sdk-runtime-dbt](https://github.com/tn-aixpa/digitalhub-sdk-runtime-dbt): execution environment for DBT-based data transformation operations
- [digitalhub-sdk-runtime-hera](https://github.com/tn-aixpa/digitalhub-sdk-runtime-hera): execution environment for Argo Workflow-based pipelines with Hera DSL 
- [digitalhub-sdk-runtime-flower](https://github.com/tn-aixpa/digitalhub-sdk-runtime-flower): execution environment for Flower FL Federated Learning framework 
- [digitalhub-sdk-wrapper-dbt](https://github.com/tn-aixpa/digitalhub-sdk-wrapper-dbt): supporting library to integrate management SDK with the DBT runtime
- [digitalhub-sdk-wrapper-kfp](https://github.com/tn-aixpa/digitalhub-sdk-wrapper-kfp): supporting library and DSL for the Argo Workflow definition on top of Kubeflow Pipelines SDK
- [digitalhub-sdk-wrapper-hera](https://github.com/tn-aixpa/digitalhub-sdk-wrapper-hera): supporting library and DSL for the Argo Workflow definition on top of Hera SDK

6. [cli](https://github.com/tn-aixpa/digitalhub-cli)

Multiplatform Command-line interface for interacting with the Core management layer.

7. [serverless](https://github.com/tn-aixpa/core-serverless)

Core serverless is the baseline for the execution of the python jobs and services in a container-based serverless mode.

8. [sts](https://github.com/tn-aixpa/db-sts)

A token exchange service to obtain (temporary) database credentials from a web identity via JWT or basic auth. Used by Core to manage credentials for DB storage.

9. [custom images](https://github.com/tn-aixpa/jupyter-notebook-custom-image)

Jupyter Notebook custom image used in the platform as a baseline for interactive environments and for python runtime.

10. [Open Metadata Connector](https://github.com/tn-aixpa/openmetadata-connector)

A custom connector for Open Metadata catalogue platform to extract and populate the catalogue with the entities (datasets, models) from the Core management layer.

11. [Kubernetes Resource Manager](https://github.com/tn-aixpa/kubernetes-resource-manager)

A tool to facilitate the management of Kubernetes resources, both standard (jobs, secrets, deployments, quotas) and custom (defined with custom operators).

12. [Minio K8S Operator](https://github.com/tn-aixpa/minio-operator)

A Kubernetes operator to handle instances of buckets, users and policies on MinIO.

13. [API Gateway K8s Operator](https://github.com/tn-aixpa/apigw-operator)

A Kubernetes operator to launch ingresses (Nginx) for services and applications.

14. [PostgREST K8S Operator](https://github.com/tn-aixpa/postgrest-operator)

A Kubernetes operator to automatically configure and start instances of PostgREST connected to databases running in the same cluster.

15. [Dremio Rest Server K8S Operator](https://github.com/tn-aixpa/dremio-rest-server-operator)

A Kubernetes operator to start instances of Dremio REST server, that is, some Dremio REST Server custom resources. 

17. [Dremio Rest Server](https://github.com/tn-aixpa/dremio-rest-server)

The Dremio REST Server is a Java SpringBoot application that provides a REST API for Dremio using Arrow Flight JDBC driver.

### AI Toolbox Components

1. [Document Classifier](https://github.com/tn-aixpa/document-classifier)

A generic LLM-based document (text) classifier (template)

2. [EuroVoc Classifier](https://github.com/tn-aixpa/eurovoc-classifier)

Multilingual text classifier based on Bert model and fine-tuned on official EU legal documents (from EUR Lex portal).

3. [Family Audit Classifier])(https://github.com/FluveFV/faudit-classifier)

Multiclass sequence classifier based on BERT base italian, fine-tuned on selected corpora from Municipalities's Family Audit plans.
   
4. [Relation Extraction Module](https://github.com/tn-aixpa/redit)

A relation extraction module for Tint. The project makes use of Tint (The Italian NLP Tool) for Natural Language Processing (NLP) in Italian for extracting the relation of entities.

5. [LLM for PA Dialogs](https://github.com/tn-aixpa/llm-pa)

A generic fine-tuned Large Language Model for dialog management for Public Administration, based on LLama-3.1.

6.[Datasets of dialogs for PA LLM](https://github.com/tn-aixpa/llm-pa-dialog-dataset) 

Dataset collected and curated for the creation of the LLM model using a “fine-running” approach necessary to support the chatbot scenario around public services.

7. [RAG Template](https://github.com/tn-aixpa/rag-template)

A generic template for the LangChaing-based RAG services using the platform functionality (template).

8. [LLM Model Fine tuner](https://github.com/tn-aixpa/llm-fine-tuner)

A lightweight framework for fine-tuning Llama-3.1-8B-Instruct, designed for efficient and reproducible training for dialogs around public services.

9. [First AID](https://github.com/tn-aixpa/api-first-AID-AIXPA)

Human-in-the-loop data collection framework for knowledge-driven generation of synthetic dialogues using LLM prompting.

10. [Sentinel Tools](https://github.com/tn-aixpa/sentinel-tools)

A repository of python-based tools and a container for downloading, preproccessing, and logging the ESA satelite data. 

11. [RSDE Tools](https://github.com/tn-aixpa/rsde-tools)

Baseline tool and Docker images for complex processing of the satelite data.

12. [Flood Detection](https://github.com/tn-aixpa/rs-flood-mapping)

A set of analysis tools for the flood detection using remote sensing data.

13. [Deforestation](https://github.com/tn-aixpa/rs-deforestation)

Python implementation for deforestation detection on satellite imagery data.

14. [Landslide Analysis](https://github.com/tn-aixpa/rs-landslide-monitoring)

Pipeline for Landslides detection to detect and monitor ground deformation associated with landslides using Sentinel-1 Level-2A imagery.

15. [EarlyExit Audio Transformer](https://github.com/tn-aixpa/audio-early-exit-transformer)

A wapper service in order to providing an Automatic Speech Recognition (ASR) solution using the Early-Exit implementation.

16. [Audio Speech Recognition fine tuner](https://github.com/tn-aixpa/asr-fine-tuning)

A lightweight framework for fine-tuning speech recognition designed for efficient and reproducible training. The models that follow Whisper fine-tuning, may be directly used for OpenAI-compatible service deployment.

17. [Micromind Adapter](https://github.com/tn-aixpa/micromind-adapter)

A toolkit to integrate efficient image and video processing  [micromind](https://github.com/micromind-toolkit/micromind) toolkit into the platform.

18. [Nefertem](https://github.com/tn-aixpa/nefertem)

A generic library used as a container for for data quality processing functionality.

19. [Digital Twin Model](https://github.com/tn-aixpa/dt-model)

DT Model is Civic-Digital-Twins modeling framework. The framework is designed to support defining digital twins models and evaluating them in simulated environment with varying contextual conditions.
